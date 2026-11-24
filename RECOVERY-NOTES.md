# Recovery notes — zhongkao-first-principles

- Source: `/Volumes/Data-A/Projects/中考复习资料书`
- Branch: `recovery-20261124`
- Backup date: 2026-11-24
- This branch is a source-only recovery snapshot from a volume with APFS corruption/zeroed files.

## Excluded all-NUL files
- None detected.

## Excluded large all-NUL candidates (>20MB, first 4KB zero)
- None detected.

## Excluded files over 100MB
- None detected.

## Removed unsafe symlinks
- None detected.

## Secret scan
- No secret-like strings detected.

## Exclusions applied
- `.git`, dependency/build/cache dirs, model/weight dirs, datasets, media/model archives, secrets (`.env`, private keys), and files >100MB were excluded.
- Excluded paths are not recoverable from this branch; see the source volume/snapshot for the originals.
