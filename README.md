# [Backstage](https://backstage.io)

This is your newly scaffolded Backstage App, Good Luck!

To start the app, run:

```sh
yarn install
yarn dev
```

## Testing PROD deployment on a local system

1. Create a GitHub App at the user or organization level according to the Backstage documentation.  
For the homepage and callback URL config look [here](https://backstage.io/docs/auth/github/provider#create-an-oauth-app-on-github) and for the permission config look [here](https://backstage.io/docs/integrations/github/github-apps/#app-permissions).
2. Create a GitHub PAT for your user or a user in the organization following the Backstage documentation [here](https://backstage.io/docs/integrations/github/locations/#token-scopes).
3. Copy the `.env.example` to `.env` and enter the generated secrets and tokens and change the GitHub Organisation if need be.

> ℹ Be sure to destroy and start the docker compose container when testing to avoid problems with caching and saved settings that are in the database.
