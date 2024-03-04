# Making Typesafe Request Params in Express Types

The blow example we extend our generic `TQuery` with the request signature for `Request`. We are then able to type our handler and pass to the `req` the type that our Request params will contain.

```ts
import express, {
  NextFunction,
  Request,
  RequestHandler,
  Response,
} from "express";
import { Equal, Expect } from "../helpers/type-utils";

const app = express();

const makeTypeSafeGet =
  <TQuery extends Request["query"]>(
    parser: (queryParams: Request["query"]) => TQuery,
    handler: RequestHandler<any, any, any, TQuery>
  ) =>
  (req: Request<any, any, any, TQuery>, res: Response, next: NextFunction) => {
    try {
      parser(req.query);
    } catch (e) {
      res.status(400).send("Invalid query: " + (e as Error).message);
      return;
    }

    return handler(req, res, next);
  };

const getUser = makeTypeSafeGet(
  (query) => {
    if (typeof query.id !== "string") {
      throw new Error("You must pass an id");
    }

    return {
      id: query.id,
    };
  },
  (req, res) => {
    // req.query should be EXACTLY the type returned from
    // the parser above
    type tests = [Expect<Equal<typeof req.query, { id: string }>>];

    res.json({
      id: req.query.id,
      name: "Matt",
    });
  }
);

app.get("/user", getUser);
```

# Override External Libraries

This is useful if you want to create a source of truth and override something a library exports. This is generally regarded as very unsafe but is possible. To do this you need to create a `.d.ts` file and declare the module you are wanting to override.


```ts
declare module "fake-animation-lib-solution" {
  export type AnimatingState =
    | "before-animation"
    | "animating"
    | "after-animation";
  export function getAnimatingState(): AnimatingState;
}
```