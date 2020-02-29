# rclone

## Commands

- `rclone copy "source:sourcepath" "dest:destpath"`
- `rclone sync "source:path" "dest:path" [flags]`
  - flags: `--create-empty-src-dirs   Create empty source dirs on destination after sync`
- `rclone ls "remote:path" [flags]`
  - `ls` to list size and path of objects only
  - `lsl` to list modification time, size and path of objects only
  - `lsd` to list directories only
  - `lsf` to list objects and directories in easy to parse format
  - `lsjson` to list objects and directories in JSON format
- `rclone tree "remote:path"`

## Flags
- `-n, --dry-run `
- `-P, --progress`

## Reference

- https://rclone.org/
