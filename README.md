# Scoop bucket for envhound

[envhound](https://github.com/michelsalib/envhound) finds which startup file sets each environment
variable, and audits your PATH. On Windows it reads your variables from the registry.

```powershell
scoop bucket add envhound https://github.com/michelsalib/scoop-envhound
scoop install envhound/envhound
```

This installs the standalone `envhound.exe` from the GitHub release. Update with `scoop update envhound`.
For PowerShell completion, add `envhound completion powershell | Out-String | Invoke-Expression` to your
profile.

`bucket/envhound.json` is generated for each release by `scripts/packages.ts` in the envhound repository,
from the release's `SHA256SUMS`.
