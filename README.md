# Duplicate File Cleaner

> Recursively scans folders to find duplicate files by content hash and safely moves redundant copies to a trash subfolder.

The bundle zip (**29.6 MB**) is stored in this repository at **`ef9c5453-f550-4d0d-a035-0477a1de0383.zip`**.

This repository is part of the **Forjinn-Desk** MCP bundle collection. An MCP bundle is a self-contained server that a host application launches and communicates with over the MCP (Model Context Protocol) protocol.

## Repo metadata

| Field | Value |
| --- | --- |
| Registry ID | `ef9c5453-f550-4d0d-a035-0477a1de0383` |
| Status in registry | inactive |
| Bundle size | 29.6 MB |
| Distribution | committed to this repo |

## Environment variables

| Variable | Value / note |
| --- | --- |
| _(none)_ | _no required environment variables_ |

## MCP launch configuration

The host replaces `__INSTALL_DIR__` (install dir) and `__PYTHON__` (bundled Python) at runtime.

```json
{
  "command": "__PYTHON__",
  "args": [
    "server.py"
  ]
}
```

## Setup / usage notes

No special setup required. Ensure you have read/write permissions on the folders you want to scan. The trash folder '._duplicates_trash' will be created inside the scanned folder when you delete duplicates.


## Install / usage

1. Get the bundle:
   - download `ef9c5453-f550-4d0d-a035-0477a1de0383.zip` from this repo (Code → Download ZIP, or `git clone`).
2. Extract to your target installation directory (config paths expect contents at the install-dir root).
3. Set the environment variables listed above.
4. Launch using the MCP config JSON (or let a host client manage it automatically).

> Bundles may include vendored runtimes (bundled Python, Node, or native executables). Builds are Windows x64.
