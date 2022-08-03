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
3. Run `az --version` to verify Azure CLI version is 2.4 or above.



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