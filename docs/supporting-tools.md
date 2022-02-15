# Supporting tools and services

A `devcontainer.json` file in your project tells tools and services that support the dev container spec how to access (or create) a **development container** with a well-defined tool and runtime stack. 

This document outlines tools and services that currently support this format.

## Remote - Containers

The [**Visual Studio Code Remote - Containers** extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) lets you use a [Docker container](https://docker.com) as a full-featured development environment. It allows you to open any folder inside (or mounted into) a container and take advantage of Visual Studio Code's full feature set.

> **Tip:** If you've already built a container and connected to it, be sure to run **Remote-Containers: Rebuild Container** from the Command Palette (`kbstyle(F1)`) to pick up any changes you make.

## GitHub Codespaces

A [codespace](https://docs.github.com/en/codespaces/overview) is a development environment that's hosted in the cloud. Codespaces run on a variety of VM-based compute options hosted by GitHub.com, which you can configure from 2 core machines up to 32 core machines. You can connect to your codespaces from the browser or locally using Visual Studio Code.

> **Tip:** If you've already built a container and connected to it, be sure to run **Codespaces: Rebuild Container** from the Command Palette (`kbstyle(F1)`) to pick up any changes you make.

## devcontainer CLI

Given the growing number of use cases for dev containers, there is a companion [devcontainer command line interface](https://code.visualstudio.com/docs/remote/devcontainer-cli) (CLI) that can be used independent of the Remote - Containers extension or GitHub Codespaces.

## Schema

You can see the VS Code implementation of the dev container schema [here](https://github.com/microsoft/vscode/blob/main/extensions/configuration-editing/schemas/devContainer.schema.src.json).