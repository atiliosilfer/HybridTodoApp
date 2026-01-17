# HybridTodoApp

This repository is a study/demo project based on the YouTube playlist:
https://www.youtube.com/playlist?list=PLdo4fOcmZ0oU6AgjUbyztrhnzGVFuN6ij

> This project is for learning purposes and reproduces concepts from the referenced playlist. It is not intended for production use.

## Overview

`HybridTodoApp` demonstrates a hybrid approach using a .NET MAUI native frontend and a Blazor web frontend that share business logic and components. The solution targets .NET 10.

## Requirements

- .NET 10 SDK
- __Visual Studio 2026__ with workloads for **.NET MAUI** and **ASP.NET/Blazor**
- Android/iOS SDKs if you plan to run mobile targets (optional)
- Git

## How to run

1. Open the solution (`.sln`) in __Visual Studio 2026__.

Blazor (web):
- Set the `HybridTodoApp.WebSite` project as the startup project and start debugging with __F5__ or __Debug > Start Debugging__.
- Or from the CLI:
  - `dotnet run --project HybridTodoApp.WebSite`

MAUI (native):
- Set the `HybridTodoApp` project as the startup project, choose the target platform in the run target selector in __Visual Studio 2026__, and press __F5__.
- The MAUI UI entry is at `HybridTodoApp/MainPage.xaml`.

## Development notes

- Target framework: `net10`.
- Shared logic and models live alongside reusable Blazor components in `HybridTodoApp.Components` to avoid duplication.
