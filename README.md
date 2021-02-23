# GraphQL Asia Workshop 2021

## Deploy Hasura

The fastest and easiest way to try Hasura out is via [Hasura Cloud](https://hasura.io/docs/latest/graphql/cloud/getting-started/index.html#cloud-getting-started).

1. Click on the following button to deploy GraphQL engine on Hasura Cloud including Postgres add-on or using an existing Postgres database:

    [![Deploy to Hasura Cloud](https://graphql-engine-cdn.hasura.io/img/deploy_to_hasura.png)](https://cloud.hasura.io/signup/?pg=workshop&plcmt=github&cta=deploy-to-cloud&tech=default)

2. Open the Hasura console

   Click on the button "Launch console" to open the Hasura console.

## Create schema

Copy the contents of schema.sql and paste into the Data->SQL tab of Hasura Console.

## Configure Auth

Head to [https://hasura.io/jwt-config/](https://hasura.io/jwt-config/) and choose Auth0 provider. Enter the Auth0 domain name as `graphql-tutorials.auth0.com`. Copy the config generated and configure it on the `HASURA_GRAPHQL_JWT_SECRET` env.

## Create Remote Schema

Add the following currency conversion API as a remote schema - https://00e5c.sse.codesandbox.io/graphql

[Sandbox that can be forked](https://codesandbox.io/s/stupefied-mclaren-00e5c?from-embed)
