---
trigger: always_on
---

# Song Creation Workflow

## Git Commands (Windows)
- Always use **WSL1** to execute git commands on Windows
- Example: `wsl git add .` instead of `git add .`

## Creating a New Song

1. **Create a folder** for the song with this naming format:
   ```
   YYYY-MM-DD-song-name
   ```
   Example: `2025-12-16-midnight-dreams`

2. **Pick a descriptive name** for the song (lowercase, hyphen-separated)

3. **Create lyrics file** as `.txt` format inside the folder:
   ```
   {song-name}_v1.txt
   ```
   Example: `midnight-dreams_v1.txt`

## Versioning Lyrics

- **Never modify existing lyrics files** – create a new version instead
- Increment the version number for each revision:
  - `song-name_v1.txt` (first draft)
  - `song-name_v2.txt` (second revision)
  - `song-name_v3.txt` (third revision)

## Folder Structure Example

```
2025-12-16-midnight-dreams/
├── midnight-dreams_v1.txt
├── midnight-dreams_v2.txt
└── midnight-dreams_v3.txt
```

## Quick Reference

| Action | Rule |
|--------|------|
| Git commands | Use WSL1 (`wsl git ...`) |
| New song | Create dated folder: `YYYY-MM-DD-name` |
| Lyrics format | `.txt` files |
| Revisions | New file with `_v{N}.txt` suffix |
| Editing | Never overwrite, always new version |