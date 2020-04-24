# simple-basic-http-auth-proxy-vercel

🔐▲ A simple basic HTTP Auth Proxy for Vercel, ideal for adding simple password protection to staging applications.

This project uses [node-http-proxy](https://github.com/http-party/node-http-proxy) inside a serverless function to add
basic password protection to ORIGIN site via HTTP Auth, requiring no code change to the ORIGIN deployment. This is designed
to add simple password protection to deployments during the UAT stage.

## Getting Started

Deploying this project to Vercel Now with the following ENV variables:

+ `ORIGIN`: The URL of your stage deployment, best to point it to a custom domain assigned to the UAT branch.
+ `USERNAME`: The username required to login.
+ `PASSWORD`: The password required to login.

## Local Usage

1. Run `yarn install` to install the require packages.
2. Update `.env` file with values required.
3. Run `now dev`.
