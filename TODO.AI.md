# TODO

- `etc/spectrwm.conf:177` — `program[thunar] = mybrowser` is mislabeled:
  the identifier says "thunar" (a file manager) but the command it
  runs is `mybrowser`. Works correctly as a browser launcher, but the
  name is confusing/likely a copy-paste error from a template.
  Found while auditing keybindings; not fixed since renaming touches
  behavior naming beyond this task's scope.
- `etc/spectrwm.conf:192-194` — `program[arcolinux-logout] =
  arcolinux-logout`, bound to `MOD+x` / `Control+Mod1+x`, calls a
  distro-specific script (`arcolinux-logout`) that is not part of
  this project and is likely not installed. The project's own
  `logout-menu` script (already used elsewhere, e.g. via canonical
  `super+alt+ctrl+l`) should probably be substituted. Not fixed here
  since it's an extra/redundant binding (canonical logout is already
  delivered via sxhkd) — flagging so it isn't silently broken.
