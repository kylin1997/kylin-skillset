# Project Maintenance Rules

## Source of Truth

`skills/learn-anything/` in this project is the only source of truth for the Learn Anything skill.

The installed directory at `~/.codex/skills/learn-anything/` is a derived copy. Never edit or maintain the installed copy directly. Make every change in this project, validate it here, and then reinstall the complete skill directory.

Before installation, confirm that the destination is absent or identical. If it exists and differs, stop and report the differences instead of overwriting it.

After installation, recursively compare the project skill and installed skill. Installation is complete only when they are identical.

Keep `doc/bc.md` as source material and preserve it unless a user explicitly requests changes to that document.
