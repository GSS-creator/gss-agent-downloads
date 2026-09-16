# GSS Agent downloads

Public release artifacts are included in this repository:

- `windows/publish/GSSAgentSetup.exe` — Windows 10/11 and Windows Server installer.
- `linux/publish/GSSAgent` — self-contained Linux x64 executable.

## Windows

Run `GSSAgentSetup.exe` as Administrator. It asks for the GSS account email and
password once, registers the machine, installs the Windows Service, and starts
heartbeats and telemetry automatically.

## Linux

```bash
chmod +x GSSAgent
sudo ./GSSAgent
```

The Linux executable installs and enables a systemd service. Both agents use
the production GSS backend and protect their local device credentials.

For direct public downloads after pushing to GitHub, use the repository paths:

```text
https://raw.githubusercontent.com/GSS-creator/gss-agent-downloads/main/GSSAgentSetup.exe
https://raw.githubusercontent.com/GSS-creator/gss-agent-downloads/main/GSSAgent
```
