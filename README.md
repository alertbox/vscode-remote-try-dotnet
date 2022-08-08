# Tryout .NET & C#

[<img align="right" alt=".NET C-sharp" width="128rem" src="https://raw.githubusercontent.com/github/explore/93d8a67084f94b2a444e510199a6e7622e5b09a3/topics/dotnet/dotnet.png" />][dotnet-quickstart]

This template repo serves as a flavor of quick-starter development container for use with [VS Code Remote - Containers][vscode-dev-containers-quickstart] and [GitHub Codespaces][gh-codespaces-quickstart].

> Originally, this dev container was created to tryout .NET development without having to install locally.

[vscode-dev-containers-quickstart]: https://www.youtube.com/playlist?list=PLj6YeMhvp2S5G_X6ZyMc8gfXPMFPg3O31
[gh-codespaces-quickstart]: https://docs.github.com/en/codespaces/getting-started/quickstart
[dotnet-quickstart]: https://www.youtube.com/playlist?list=PLdo4fOcmZ0oUc2ShrReCS7KoBbPEONE0p

### What's in it:

- .NET 6.0 SDK and Runtime
- Azure CLI for publishing and managing cloud resources
- [VS Code Extensions](/.devcontainer/devcontainer.json) for .NET and Azure-related work
- [VS Code Tasks](/.vscode/tasks.json) to build, launch, and debug from source
- [EditorConfig](/.editorconfig) for .NET and C# coding standards
- Git and GitHub CLI for versioning
- ZSH integrated Terminal
- Docker CLI with Compose v2

## Using This Template

If you are completely new to .NET, [Awesome .NET discussion][awesome-list-dotnet] is a good source to start with.

Next, you want to create a copy of this template. It is easy as forking. The repo is marked as a `Template` so you will only have to [Use This Template][gh-use-this] and follow the instructions.

[awesome-list-dotnet]: https://
[gh-use-this]: https://github.com/kosalanuwan/try-dotnet/generate



## Things to Try

First, you want to ensure source code is Reopened in Container. Then you'll be able to work with it like you would locally.

With VS Code:

1. In a terminal, run `dotnet --list-sdks` to verify required versions are installed.
3. Run `gh --version` to verify GitHub CLI is installed.

### Create a minimal api

Next, you would want to create a .net project, say, a minimal web api `test-project` that ships with .net template projects.

With VS Code:

1. Run the `dotnet new` command to create a web api with specific template.
   ```bash
   dotnet new webapi -o test-project \
                     --use-minimal-apis \
                     --language "C#"
   ```
2. Open the launchSettings.json, then change the `test_project` profile to run on port `5000` for HTTP and `5001` for HTTPS.
   ```json
   "profiles": {
     "test_project": {
       // ...
       "applicationUrl": "https://localhost:5001;http://localhost:5000",
       // ...
   }
   ```

### Build and run from source

VS Code is integrated with the Omnisharp Tools to run the web api on the local development computer, in this case, its this dev container.

With VS Code:

1. Press `F5` to start the web api project and call the swagger endpoint. The terminal displays the output from the Debug Console.
2. When the web api executes locally, your favorite browser will launch the https://localhost:5001.
3. Visit https://localhost:5001/swagger
4. Press `Ctrl+C` to stop disconnect the debugger.


## Feedback

If you have any technical problems with GitHub Codespaces or dev containers, you are better off asking [VS Code Support][feedback-channels] directly, since you'll end up getting a much faster response back that way.

[feedback-channels]: https://github.com/microsoft/vscode-dev-containers#contributing-and-feedback


## Contributing

The official repo to contribute would be [@microsoft/vscode-dev-containers][contrib-official-repo].

Have a suggestion or a bug fix? Just open a pull request or an issue. Include the development container with clear and simplest instructions possible.

[contrib-official-repo]: https://github.com/microsoft/vscode-dev-containers#readme


## License

Copyright (c) Kosala Nuwan Perera. All rights reserved.

The source code is license under the [MIT license](LICENSE).