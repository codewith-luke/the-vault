## Overview

The role of the [HyperRoute](https://starwars.fandom.com/wiki/Hyperspace_route) is to proxy requests from the client and from externals to the various services. 

This will also handle Websocket connections to the messaging service.

In short this is just a simple proxy layer that makes use of OpenAPI and uses OAPI as a codegen. The codegen is just simple wrapper methods and validation around endpoints.

**Tools:**
- [Open API Codegen](https://github.com/deepmap/oapi-codegen)
- Swagger Docs
- [Go Echo](https://echo.labstack.com/)

This is meant to be a simple service where .env will be configured to point to relevant services. The idea of this service is just to play around with the idea of proxies, codegen and OpenAPI.

