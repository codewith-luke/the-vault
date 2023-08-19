# Extending Namespaces

https://www.typescriptlang.org/docs/handbook/namespaces.html
https://www.digitalocean.com/community/tutorials/how-to-use-namespaces-in-typescript

Here we declare our global. Then we are extending the NodeJS namespace. Using declaration merging we then take the `ProcessEnv` interface and extend to add our custom env variable

```ts
declare global {
  namespace NodeJS {
    interface ProcessEnv {
      MY_SOLUTION_ENV_VAR: string;
    }
  }
}
```

# Adding to Global Scope Dynamically

```ts
const addAllOfThisToWindow = {
  addSolution: (a: number, b: number) => a + b,
  subtractSolution: (a: number, b: number) => a - b,
  multiplySolution: (a: number, b: number) => a * b,
  divideSolution: (a: number, b: number) => a / b,
};

Object.assign(window, addAllOfThisToWindow);

declare global {
  type StuffToAdd = typeof addAllOfThisToWindow;

  interface Window extends StuffToAdd {}
}
```

The above code uses the interface of `Window` and adds our extra functionality to it. First we have to get the `typeof` of what we want to be able to extend. Then we add to the `Window` interface.