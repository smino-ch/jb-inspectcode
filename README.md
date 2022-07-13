# JB Inspect Issue

## Tree structure

```
jb-inspect
├── App.One
│   └── App.One
│       ├── App.One.csproj
│       ├── Lib.One
│       ├── Program.cs
│       ├── Properties
│       │   └── launchSettings.json
│       ├── appsettings.Development.json
│       ├── appsettings.json
├── Lib.One
│   ├── Class1.cs
│   └── Lib.One.csproj
├── README.md
└── jb-inspect.sln
```

## Command

```
jb inspectcode ./App.One/App.One/App.One.csproj --output=report.xml --build
```

## Output

```
JetBrains Inspect Code 2022.1.2
Running on AMD 64 in 64-bit mode, .NET 6.0.7 under Darwin 21.5.0 Darwin Kernel Version 21.5.0: Tue Apr 26 21:08:22 PDT 2022; root:xnu-8020.121.3~4/RELEASE_X86_64
Warning: Can't get proc info, errno: 3
Using toolset version 17.0 from /usr/local/share/dotnet/sdk/6.0.302
Referenced project 'Lib.One' not found in the solution, switched to output assembly.
Referenced project 'Lib.One' not found in the solution, switched to output assembly.
Analyzing files

Analyzing Lib.One.csproj.nuget.g.props
Analyzing Lib.One.csproj.nuget.g.targets
Analyzing project.nuget.cache
Analyzing App.One.GeneratedMSBuildEditorConfig.editorconfig
Analyzing analysislevel_6_default.editorconfig
Analyzing App.One.csproj
Inspecting Program.cs
Inspecting report.xml
Inspecting Lib.One.csproj.nuget.dgspec.json
Inspecting launchSettings.json
Inspecting appsettings.json
Inspecting appsettings.Development.json
Inspecting project.assets.json
Inspection report was written to /$HOME/src/jb-inspect/App.One/App.One/report.xml
```
