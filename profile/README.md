# PXE.js
A web framework.

### Example
Simple web server that responds with `Hello world` on each request.

```ts
import Server from "@pxe/server";

// Initialize a new server
const app = new Server();

// Add a middleware
app.use(async (ctx, next) => {
    // Set the response to "Hello world"
    ctx.response.body = "Hello world";

    // Run the next middleware
    // End the response if this is the last middleware
    await next();
});

// Listen to port 3000
app.ls(3000);
```

### Basic Features
- Web cookie
- Redirect
- Error handling
- Middlewares
- Typescript support

### Usage
Currently [documentation](https://pxe.vercel.app) is under construction.
Please chat on [Discord](https://discord.gg/BAB6wZhBFc) if you want to ask any question.

[!["Buy Me A Coffee"](https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png)](https://www.buymeacoffee.com/aquapi)
