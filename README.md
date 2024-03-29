# Belp.SDK.PackOnly
An MSBuild SDK for pack-only projects.

## Installation

### Requirements
- A project written in SDK-style. This includes any project for .NET Core(or newer) or .NET 5(or newer).

### Install using an Editor
1. Locate the project file(for example, `Project.csproj`, `Project.fsproj`).
1. Open the project file in an editor.
1. Locate the project's root `<Project>` element.
1. Edit the `Sdk` attribute's value to `Belp.SDK.PackOnly/<VERSION>`. For example, `Sdk="Belp.SDK.PackOnly/1.0.0"`.

## Usage

### Set `TargetFramework`
By default, the target framework is set to .NET Standard 2.0. This can be overriden by defining `<TargetFramework>` under a `<PropertyGroup>`.

### Enable Build
1. Locate the project file(for example, `Project.csproj`, `Project.fsproj`).
1. Open the project file in an editor.
1. Add `<DisableDefaultBuild>false</DisableDefaultBuild>` to a `<PropertyGroup>`.

## Development

### Prerequisites
- Install the .NET 7.0 SDK version 7.0.100 or newer.

### Building with Visual Studio
1. Open `Belp.SDK.PackOnly.sln`.
1. Open the Solution Explorer.
1. Right click on the project `Belp.SDK.PackOnly` in the Solution Explorer.
1. Click on `Pack`.

### Building with .NET CLI
1. Open a terminal in the repository root.
1. Run `dotnet pack`

### Output
By default, the output is located in `src/Belp.SDK.PackOnly/Belp.SDK.PackOnly/bin/Release/`.
