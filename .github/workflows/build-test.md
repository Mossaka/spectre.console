---
name: Build and Test Spectre.Console
on:
  workflow_dispatch:
permissions:
  contents: read
engine: copilot
runtimes:
  dotnet:
    version: "8.0"
network:
  firewall: true
  allowed:
    - defaults
    - github
    - nuget.org
    - api.nuget.org
---

# Build and Test Spectre.Console

You are a C# developer. Your task is to build and test the Spectre.Console library.

## Steps

1. First, explore the repository structure to understand the project layout
2. Restore NuGet packages using `dotnet restore`
3. Build the solution using `dotnet build`
4. Run the tests using `dotnet test`
5. Report the results of the build and test

If any step fails, investigate the error and try to resolve it.
