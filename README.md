# Mount Thor public Scoop bucket

Public [Scoop](https://scoop.sh) bucket for the **Mount Thor customer CLI** (`mountthor`) on Windows.

## Install

```powershell
scoop bucket add mountthor https://github.com/Mount-Thor/scoop-bucket
scoop install mountthor
```

That single command adds the bucket and installs the latest binary. Upgrades:

```powershell
scoop update mountthor
```

## Other install channels

- **macOS (Homebrew):** `brew install Mount-Thor/mountthor/mountthor`
- **Linux or non-Homebrew macOS:** `curl -fsSL https://get.mountthor.com/install.sh | sh`
- **Windows (direct PowerShell):** `powershell -c "irm https://get.mountthor.com/install.ps1 | iex"`

## What `mountthor` is

`mountthor` is the customer-facing CLI for [Mount Thor](https://mountthor.com), a neocloud for dedicated Apple silicon Mac fleets. The CLI handles registration, API keys, sessions, customer compute context rendering, bare-metal leases, and VM workflows.

Source: <https://github.com/Mount-Thor/mount-thor/tree/main/operator-tools/mountthor-cli>.

## How this bucket stays current

`bucket/mountthor.json` is auto-committed by the release workflow in [`Mount-Thor/mount-thor`](https://github.com/Mount-Thor/mount-thor) whenever a `mountthor-v*` tag is pushed. Do not hand-edit the manifest — your changes will be overwritten on the next release.
