# GraphQLServer

## How to use this repo

This repository leverages the Hot Chocolate open-source GraphQL server for the Microsoft .NET platform. You can find more information here https://chillicream.com/docs/hotchocolate/v13. The code was crafted using the Hot Chocolate workshop, which is available here https://github.com/ChilliCream/graphql-workshop. Additionally, you can extend your server with more examples from this tutorial. https://www.apollographql.com/tutorials/intro-hotchocolate/01-overview-setup
You can clone and run this repository locally using Visual Studio 2022 Express Edition. https://visualstudio.microsoft.com/vs/express/

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

### Queries / Mutation 

```shell
 query  getSpeakers {
    speakers {
      bio,
      name,
      id
    }
 }
```
 
```shell
 query GetSpeakerNames {
  speakers {
    name
  }
}
```

```shell
mutation AddSpeaker {
  addSpeaker(input: {
    name: "tester"
    bio: "good at unit test"
    webSite: "http://unittest.test" }) {
    speaker {
      id
    }
  }
}
```

## Getting Help

This repo is _not regularly monitored_.

For any questions contact https://vizzon.co.uk/contact/
