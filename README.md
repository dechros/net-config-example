# net-config-example

Two WPF applications (client and server) exchanging device configuration through XML files in `C:\Ulak`. The server publishes `serverConf.xml` with manufacturer/model/serial fields and the client polls `server.xml` for status and mirrors its own state in `client.xml`.

## Platform

.NET Framework WPF on Windows. Built with Visual Studio (`netconfExample.sln`).

## Layout

```
netconfClient/    WPF client application
nrtconfServer/    WPF server application
netconfExample.sln
```

## Build

Open `netconfExample.sln` in Visual Studio and build both projects, or from a Developer Command Prompt:

```bat
msbuild netconfExample.sln /p:Configuration=Debug
```

## Dependencies

- `Renci.SshNet` (via NuGet `packages/`)
