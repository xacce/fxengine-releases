# fxengine releases

Signed Windows releases of fxengine, the engine in which agents build game VFX. Sources are private.

Install or update to the latest release (PowerShell):

```powershell
irm https://github.com/xacce/fxengine-releases/releases/latest/download/install.ps1 | iex
```

The engine goes to `%LOCALAPPDATA%\Programs\FxEngine`, joins the user's PATH and installs its skill for the agent runtimes it finds (Claude, Codex). It updates itself from here; every release is signed and checked against the key built into the engine. Agents read the manual with `fxengine guide`. Effects build their behaviors with Rust (`cargo`).
