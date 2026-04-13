# macOS

This folder contains the packaged desktop bridge app:

- `RUNLOOM Bridge.app`

## Launch

```bash
open "RUNLOOM Bridge.app"
```

If Gatekeeper blocks the app:

```bash
xattr -dr com.apple.quarantine "RUNLOOM Bridge.app"
open "RUNLOOM Bridge.app"
```

## Health check

Once the app is running, the local bridge should respond on:

- `http://127.0.0.1:8765/health`
- `http://127.0.0.1:8765/api/bridge/health`
