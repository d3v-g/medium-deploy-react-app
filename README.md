# medium-deploy-react-app
React app built with Vite, Typescript, with CI/CD pipelines that deploy to Azure App Service.

A step by step guide on how to set up CI/CD using GitHub Actions can be found in my Medium article: [How to deploy a Vite React app to Azure App Service using CI/CD Pipelines(GitHub Actions)](https://medium.com/@janesfrontenddiary/how-to-deploy-a-vite-react-app-to-azure-app-service-using-ci-cd-pipelines-github-actions-1cee30d49ab0)

## How to run
### Prerequisites
- Install Node LTS (v18.16.1 ATTOW)
  
This project is built using Vite and can be run in the following steps:
### Clone the repo
```
git clone https://github.com/d3v-g/medium-deploy-react-app
```
### Install dependencies
```
npm install
```
### Run in development mode
```
npm run dev
```

## CI/CD pipelines
### [main_react-app-linux.yml](.github/workflows/main_react-app-linux.yml)
This workflow runs linting, tests, and builds and deploys application to an Azure App Service running on Linux containers.

### [main_react-app-windows.yml](.github/workflows/main_react-app-windows.yml)
This workflow runs linting, tests, and builds and deploys application to an Azure App Service running on Windows containers.