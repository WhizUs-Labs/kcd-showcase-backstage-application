# WhizUs [Backstage](https://backstage.io) showcase

This repository contains the Backstage application showcased at KCD Austria 2024 by WhizUs.

## Local development

To start the app, run:

```sh
yarn install
yarn dev
```

## Testing PROD deployment on a local system

1. Create a GitHub App at the user or organization level according to the Backstage documentation.  
For the homepage and callback URL config look [here](https://backstage.io/docs/auth/github/provider#create-an-oauth-app-on-github).
2. Create a GitHub PAT for your user or a user in the organization following the Backstage documentation [here](https://backstage.io/docs/integrations/github/locations/#token-scopes).
3. Copy the `.env.example` to `.env` and enter the generated secrets and tokens and set the GitHub organisation.  
It is highly recommended to save your secrets and tokens to a password manager of your choosing instead of hardcoding the values.
4. Start the application with a `docker compose up`. Add the `--build` flag if you made changes to the application. If you don't want to follow the logs add the `-d` flag.  

> ℹ Be sure to destroy and start the docker compose container when testing to avoid problems with caching and saved settings that are in the database.
