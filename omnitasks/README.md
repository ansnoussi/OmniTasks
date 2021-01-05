# Omnitasks 📝

This project was generated using [Nx](https://nx.dev). <br>

Nx is a suite of powerful, extensible dev tools that help you develop, test, build, and scale large applications with fully integrated support for modern libraries like Jest, Cypress, ESLint, Storybook, and more.
<br>

Capabilities can be added to this workspace using [official plugins](https://nx.dev/latest/angular/plugins/overview) or [community plugins](https://nx.dev/nx-community).

## Run the application

- **Run the web stack (Express + React)**
I used *concurrently* to achieve this, simply run `npm run web-dev` to run the React app on http://localhost:4200/ and the Express app on http://localhost:3333/api <br>
⚠ *Important* : so that we don't run into any CORS issues while developing, a proxy configuration is set to proxy requests to http://localhost:4200/api to the Express server.
<br>

- **Run a single app**
To run a single app, simply use `npx nx serve my-app`

## Generate an application

Run `npx nx g @nrwl/react:app my-app` to generate an application.

> You can use any of the plugins above to generate applications as well.

When using Nx, you can create multiple applications and libraries in the same workspace.

## Generate a library

Run `npx nx g @nrwl/react:lib my-lib` to generate a library.

> You can also use any of the plugins above to generate libraries as well.

Libraries are sharable across libraries and applications. They can be imported from `@omnitasks/mylib`.

## Understand your workspace

Run `npx nx dep-graph` to see a diagram of the dependencies of your projects.
