# AGENTS.md

## Cursor Cloud specific instructions

This is a minimal Git-workflow practice repository containing a single PowerShell script (`refresh-avd-hosts.ps1`). There is no build system, no package manager, no tests, and no services to run.

### Running the script

```bash
pwsh -File refresh-avd-hosts.ps1
```

PowerShell (`pwsh`) is installed from the official GitHub release tarball at `/opt/microsoft/powershell/7/pwsh` (symlinked to `/usr/bin/pwsh`). The update script reinstalls it if missing.

### Notes

- Lines 7-9 of `refresh-avd-hosts.ps1` contain plain-text strings (not valid PowerShell commands) that produce expected "term not recognized" errors at runtime. This is pre-existing in the repo.
- There are no linters, test frameworks, or build steps configured for this repository.
- `apt-get update` may hang in this VM environment; the update script uses a direct tarball download to install PowerShell instead.
