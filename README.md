# Classic Blue 2017 Theme

VSIX project for a Visual Studio 2026-compatible recreation of the Visual Studio 2017 blue theme.

## Build

```powershell
dotnet build .\ClassicBlue2017Theme.csproj -c Release
```

The generated VSIX is written to:

```text
bin\Release\net48\ClassicBlue2017Theme.vsix
```

## Install

Double-click the generated `.vsix`, close Visual Studio when prompted, and complete installation in the VSIX Installer. After restarting Visual Studio, select:

```text
Tools > Options > Environment > General > Color theme > Classic Blue 2017
```

## Customize

Edit `Themes\ClassicBlue2017.vstheme`. The project uses `Microsoft.VisualStudio.VsixColorCompiler` to compile the `.vstheme` into `.pkgdef` during build.

The two categories added for Visual Studio 2026 are:

```text
Shell
ShellInternal
```

These semantic tokens control much of the modern Visual Studio 2026 shell surface.
