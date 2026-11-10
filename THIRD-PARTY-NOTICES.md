# Third-party notices

SerialFlow includes the components below. Each one remains under its own licence. The full licence texts and the
upstream notice files are in the [`licenses/`](licenses/) folder next to this file.

This list matches the files in the published app of **SerialFlow 0.9.0-beta.1** (self-contained, win-x64). It was
checked against the publish folder on 2026-11-09.

## Components

| Component | Version | Licence | Copyright | Project | Texts in `licenses/` |
|---|---|---|---|---|---|
| .NET runtime and WPF (built into the app) | 8.0.31 | MIT | .NET Foundation and Contributors | [dotnet/runtime](https://github.com/dotnet/runtime), [dotnet/wpf](https://github.com/dotnet/wpf) | `MIT-dotnet-runtime.txt`, `MIT-dotnet-wpf.txt`, `THIRD-PARTY-NOTICES-dotnet-runtime-8.0.31.txt`, `THIRD-PARTY-NOTICES-dotnet-wpf-8.0.txt` |
| Microsoft.Extensions.Configuration, Microsoft.Extensions.Configuration.Abstractions, Microsoft.Extensions.Configuration.Binder, Microsoft.Extensions.Configuration.CommandLine, Microsoft.Extensions.Configuration.EnvironmentVariables, Microsoft.Extensions.Configuration.FileExtensions, Microsoft.Extensions.Configuration.Json, Microsoft.Extensions.Configuration.UserSecrets, Microsoft.Extensions.DependencyInjection, Microsoft.Extensions.DependencyInjection.Abstractions, Microsoft.Extensions.Diagnostics, Microsoft.Extensions.Diagnostics.Abstractions, Microsoft.Extensions.FileProviders.Abstractions, Microsoft.Extensions.FileProviders.Physical, Microsoft.Extensions.FileSystemGlobbing, Microsoft.Extensions.Hosting, Microsoft.Extensions.Hosting.Abstractions, Microsoft.Extensions.Logging, Microsoft.Extensions.Logging.Abstractions, Microsoft.Extensions.Logging.Configuration, Microsoft.Extensions.Logging.Console, Microsoft.Extensions.Logging.Debug, Microsoft.Extensions.Logging.EventLog, Microsoft.Extensions.Logging.EventSource, Microsoft.Extensions.Options, Microsoft.Extensions.Options.ConfigurationExtensions, Microsoft.Extensions.Primitives, System.Diagnostics.DiagnosticSource, System.Diagnostics.EventLog, System.IO.Pipelines, System.Text.Encodings.Web, System.Text.Json | 10.0.6 | MIT | .NET Foundation and Contributors | [dotnet/runtime](https://github.com/dotnet/runtime) | `MIT-dotnet-runtime.txt`, `THIRD-PARTY-NOTICES-dotnet-runtime-10.0.6.txt` |
| System.IO.Ports, System.Threading.Channels | 9.0.7 | MIT | .NET Foundation and Contributors | [dotnet/runtime](https://github.com/dotnet/runtime) | `MIT-dotnet-runtime.txt`, `THIRD-PARTY-NOTICES-dotnet-runtime-9.0.7.txt` |
| Microsoft.Extensions.ObjectPool | 9.0.7 | MIT | .NET Foundation and Contributors | [dotnet/aspnetcore](https://github.com/dotnet/aspnetcore) | `MIT-dotnet-aspnetcore.txt`, `THIRD-PARTY-NOTICES-aspnetcore-9.0.7.txt` |
| Microsoft.Data.Sqlite.Core | 9.0.7 | MIT | .NET Foundation and Contributors | [dotnet/efcore](https://github.com/dotnet/efcore) | `MIT-dotnet-efcore.txt` |
| SQLitePCLRaw.bundle_e_sqlite3, SQLitePCLRaw.core, SQLitePCLRaw.lib.e_sqlite3, SQLitePCLRaw.provider.e_sqlite3 | 2.1.10 | Apache-2.0 | SourceGear, LLC | [ericsink/SQLitePCL.raw](https://github.com/ericsink/SQLitePCL.raw) | `Apache-2.0.txt`, `NOTICE-SQLitePCLRaw.txt` |
| SQLite (inside `e_sqlite3.dll`) | 3.46.1 | Public domain | — | [sqlite.org](https://sqlite.org/copyright.html) | `NOTICE-SQLitePCLRaw.txt` |
| System.Reactive | 6.0.1 | MIT | .NET Foundation and Contributors | [dotnet/reactive](https://github.com/dotnet/reactive) | `MIT-dotnet-reactive.txt` |
| CommunityToolkit.Mvvm | 8.4.0 | MIT | .NET Foundation and Contributors | [CommunityToolkit/dotnet](https://github.com/CommunityToolkit/dotnet) | `MIT-CommunityToolkit.txt`, `THIRD-PARTY-NOTICES-CommunityToolkit.txt` |
| Dirkster.AvalonDock, Dirkster.AvalonDock.Themes.VS2013 | 4.72.1 | Ms-PL | — (none stated) | [Dirkster99/AvalonDock](https://github.com/Dirkster99/AvalonDock) | `Ms-PL-AvalonDock.txt` |
| Serilog | 4.3.1 | Apache-2.0 | Serilog Contributors | [serilog/serilog](https://github.com/serilog/serilog) | `Apache-2.0.txt` |
| Serilog.Enrichers.Environment 3.0.1, Serilog.Enrichers.Process 3.0.0, Serilog.Enrichers.Thread 4.0.0, Serilog.Expressions 5.0.0, Serilog.Extensions.Hosting 10.0.0, Serilog.Extensions.Logging 10.0.0, Serilog.Formatting.Compact 3.0.0, Serilog.Sinks.Async 2.1.0, Serilog.Sinks.Console 6.0.0, Serilog.Sinks.Debug 3.0.0, Serilog.Sinks.File 7.0.0 | see name | Apache-2.0 | Serilog Contributors | [github.com/serilog](https://github.com/serilog) | `Apache-2.0.txt` |
| Velopack (library, plus the installer and `Update.exe` it adds) | 0.0.942 | MIT | Caelan Sayler (Velopack Ltd.) | [velopack/velopack](https://github.com/velopack/velopack) | `MIT-Velopack.txt` |
| NuGet.Versioning (used by Velopack) | 6.12.1 | Apache-2.0 | .NET Foundation and Contributors | [NuGet/NuGet.Client](https://github.com/NuGet/NuGet.Client) | `LICENSE-NuGet.txt`, `Apache-2.0.txt` |

## Notes

- **Apache-2.0 NOTICE files:** of the Apache-2.0 components, only SQLitePCL.raw has a `NOTICE` file. It is reproduced
  unchanged as `licenses/NOTICE-SQLitePCLRaw.txt`. Serilog and NuGet.Client have none.
- **Upstream notice files:** the .NET runtime, WPF, ASP.NET Core and the .NET Community Toolkit list the third-party
  code they contain in their own notice files. They are reproduced unchanged, one per version that ships.
- **Not shipped:** the test-only packages (xUnit, FluentAssertions and others) are not part of the app.
- **A copy comes with the app:** this page and the `licenses/` folder are also in the SerialFlow install folder.
