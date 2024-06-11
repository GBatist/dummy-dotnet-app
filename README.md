# dummy-dotnet-app

Hey there! Just a heads up, this dummy app will be used for:

- Creating a project using the CLI instead of relying on Visual Studio automation.
- Getting to know how to use Trivy and Snyk with Github Actions to understand how pipelines work.
- Use a multistage Dockerfile and Chainguard secure .NET images

## Commands

After getting the [SDK installed](https://dotnet.microsoft.com/pt-br/download/dotnet), we can run the following command using the DotNet CLI to create our project:

```bash
dotnet new console -o HelloWorldApp
```

As you can see, we are creating the project as a `console` application. To learn about other types of projects, [check the documentation here](https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-new).

## Misc

To get more information about how to use Chainguard's images [check the documentation here](https://edu.chainguard.dev/chainguard/chainguard-images/reference/dotnet-sdk/).
