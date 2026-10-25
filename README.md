# @nouryehia/setup-wizard

Catalogs, installs, and sets up all the tools/artifacts needed to stand up a development environment on a macOS machine. The repo root mirrors `~`: every tracked file (except `.wizard/` and this README) is symlinked to the same path under `~`.

## Usage

Clone this [repo](https://github.com/nouryehia/setup-wizard.git), then from the clone:

```bash
.wizard/setup    # symlink every tracked file into ~
.wizard/revert   # remove those symlinks and restore the original files
```

- 🆕 To add a file, copy it from `~` to the same path in the repo, `git add` it, and run `.wizard/setup`.
- ℹ️ Files already in `~` are moved to `~/.local/state/setup-wizard/backup` before being replaced.
- ⚠️ Symlinks point into the clone, so run `.wizard/revert` before moving or deleting it.

