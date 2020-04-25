# simple-basic-http-auth-proxy-vercel

🔐▲ A simple basic HTTP Auth Proxy for Vercel, ideal for adding simple password protection to staging applications.

This project uses [node-http-proxy](https://github.com/http-party/node-http-proxy) inside a serverless function to add
basic password protection to ORIGIN site via HTTP Auth, requiring no code change to the ORIGIN deployment. This is designed
to add simple password protection to deployments during the UAT stage.

## Getting Started

1. Deploying this project to Vercel Now<br/>[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/bbiHQ/simple-basic-http-auth-proxy-vercel/tree/master/)

2. Adding the following ENV variables for Production:

  + `ORIGIN`: The URL of your stage deployment, best to point it to a custom domain assigned to the UAT branch.
  + `USERNAME`: The username required to login.
  + `PASSWORD`: The password required to login.
  
3. Redeploy app using the updated ENV variables.

## Local Usage

1. Run `yarn install` to install the require packages.
2. Update `.env` file with values required.
3. Run `now dev`.

## Demo

The deployment at https://simple-basic-http-auth-proxy-vercel.now.sh adds password protection around Google search.

Username: williamli

Password: password
