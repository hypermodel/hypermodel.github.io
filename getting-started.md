# Getting Started

This guide will help you to get started with building your first Hyper Model app.

## Pre-requisites

Please install the following applications:

### Python 3.7 (Anaconda)

Link: https://www.anaconda.com/distribution/

If you are using ZSH as your shell you may need to update your `~/.zshrc to include a line like:

> export PATH=/anaconda/bin:\$PATH

Or

> export PATH=/Users/{username}/anaconda/bin:\$PATH

### NodeJS

https://nodejs.org/en/

### Dotnet Core 2.2

https://dotnet.microsoft.com/download/dotnet-core/2.2

## Tooling for improved developer experience

For the best development experience, we recommend that you download and install Visual Studio Code:

https://code.visualstudio.com/

To further improve the development experience we recommend that you also install the following plugins:

- Prettier - Code Formatter
- Python
- YAML
- vscode-proto3

## Verify pre-requisites

In a terminal please run:

> python --version
> (Output should be `Python 3.x.x` or greater)

> node --version
> (Output should be `v10.x.x` or greater)

> dotnet --version
> (Output should be `2.1.xxx` or greater)

# Installing Hyper Model

You can install Hyper Model using the following command:

> dotnet tool install GrowingData.HyperModel.App.Local -g --add-source https://www.myget.org/F/hyper-model/auth/5fded3b1-5d72-40d2-85f9-c7c415095c55/api/v3/index.json

This wil install the `hyper_model` command which will control your local Data Platform.

Verify that Hyper Model has been installed properly:

> hyper_model check

# Create a new Project

In a terminal, change the directory to the path you want to develop in.

> hyper_model project create --name home_credit_risk

This will create a new Hyper Model project `home_credit_risk` in the current path.

> cd home_credit_risk

Now lets run this Hyper Model project

> hyper_model project run

Open a web browser to:

https://localhost:8001/hyper-admin

And explore Hyper Model.
