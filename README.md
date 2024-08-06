# GraphQLServer

## How to use this repo

This repo uses Hot Chocolate open-source GraphQL server for the Microsoft .NET platform https://chillicream.com/docs/hotchocolate/v13 and hot chocolate workshop to craft this code https://github.com/ChilliCream/graphql-workshop
You can also extend your server using more examples here https://www.apollographql.com/tutorials/intro-hotchocolate/01-overview-setup

### Update local setting / run project locally

1) Update database Connection String in GraphQLAppSettings.cs file e.g. Data Source=.\SQLEXPRESS;Initial Catalog=ConferencesDb;Integrated Security=SSPI;

2) Open package manager console and run database initial script

   ```shell
   update-database
   ```
   
4) Build / run
 
```shell
dotnet build
```

```shell
dotnet start
```
The local `graphql server` should be listening on https://localhost:44318/graphql/ 

## Getting Help

This repo is _not regularly monitored_.

For any questions contact https://vizzon.co.uk/contact/
