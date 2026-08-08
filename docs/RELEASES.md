# Releases

Presence Manager is distributed as **compiled binaries** through GitHub Releases. The source code is not public.

## Versioning

Releases follow a simple **semantic versioning** scheme:

```
v1.0.0
v1.1.0
v1.2.0
```

- **Major** (`x.0.0`) — significant changes or breaking changes.
- **Minor** (`0.x.0`) — new features that keep backward compatibility.
- **Patch** (`0.0.x`) — bug fixes and small improvements.

## Release contents

Each release must contain:

- **Title** — e.g. `v1.0.0 — First public release`.
- **Summary** — 1–2 sentences describing what changed for the user.
- **Changelog** — a list of changes, additions and fixes (see `docs/CHANGELOG.md`).
- **Requirements** — Windows version, Discord Desktop, and any other requirement.
- **Download files** — the compiled binaries (a `.zip` archive with `PresenceManager.exe` and its required files is recommended for the portable version).
- **Installation instructions** — how to install/update when necessary.

## What is published

Only compiled files go into a release:

- ✅ Executables and required runtime files (portable zip)
- ✅ Release notes / changelog

## What is never published

- ❌ Source code (`.cs`, `.xaml`, `.csproj`, solution files)
- ❌ Secrets, credentials, tokens or personal files
- ❌ Debug builds or temporary build artifacts (`bin/`, `obj/`, `.vs/`)
- ❌ Personal configuration files (the developer's own `%AppData%\PresenceManager` content)
