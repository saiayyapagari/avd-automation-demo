# AGENTS.md

## Cursor Cloud specific instructions

This is a minimal demo repository containing a single PowerShell script (`refresh-avd-hosts.ps1`) used for practicing Git workflows. There is no build system, package manager, test framework, or linter.

### Running the script

```
pwsh -File refresh-avd-hosts.ps1
```

PowerShell Core (`pwsh`) must be installed. The update script handles this automatically. Lines 7-9 of the script contain bare text (not valid PowerShell) that produce non-fatal `CommandNotFoundException` errors — this is expected and part of the existing repo content.

### Notes

- There are no dependencies, no build step, no tests, and no lint configuration.
- The entire codebase is two files: `README.md` and `refresh-avd-hosts.ps1`.
