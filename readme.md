# Remix Azure Static Web Application

<img src="./images/remix.png?raw=true" alt="Remix logo" width="100" height="100">
<img src="./images/static-web-apps.png?raw=true" alt="Azure Static Web Apps logo" width="125" height="auto">

This repo is a starter for a basic [Remix](https://www.remix.run/) web application deployed to [Azure Static Web Apps (SWA)](https://azurestaticwebapps.dev/).

It consists a top level node workspace containing the following:
- `web`: Basic remix application, configured to build remix server to `../api/build`.
- `api`: An Azure function to handle http request for remix routes.

The basic Remix web application and Azure Function request handler is based on [this repository by Jeff Emery](https://github.com/JeffEmery/remix-client-azure), with minor modifications.  See the respective README in the subdirectories for more information.

## Getting Started

### Prerequisites:
- Node version 16
  - You may run into [this issue](https://github.com/Azure/static-web-apps-cli/issues/367) on Mac with other versions.
- Azure Functions for local development
  - [Visual Studio Code](https://code.visualstudio.com/) and [Azure Functions](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-azurefunctions) VS Code extension
  - or [Azure Functions Core Tools](https://learn.microsoft.com/en-us/azure/azure-functions/functions-run-local?tabs=v4%2Cmacos%2Ccsharp%2Cportal%2Cbash)

### Steps:
1. Clone this repository to your local environment.
2. `npm install`
3. `npm run build`
4. `npm run start`

### Codespace

This repo has a dev container. This means if you open it inside a GitHub Codespace, or using VS Code with the remote containers extension, it will be opened inside a container with all the dependencies already installed.

## From Scratch

If you're looking to create something similar from scratch, see the README for the `web` subdirectory or [this repository by Jeff Emery](https://github.com/JeffEmery/remix-client-azure).