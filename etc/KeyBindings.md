## Key Bindings

Source: cross-desktop app/media/lock/screenshot/logout bindings come
from the shared `run_sxhkd` (dfmgr/sxhkd `etc/sxhkdrc`), started by
`etc/autostart.sh`. `etc/spectrwm.conf` holds only spectrwm's own
window-management bindings and a few native extras (see TODO.AI.md
for two pre-existing oddities found while auditing this); `MOD` =
super (default spectrwm modkey).

### Cross-desktop canonical bindings (via dfmgr/sxhkd)

```text
super + Return                   # Open terminal
super + alt + b                  # Open browser
alt + r                          # Open file manager
super + alt + l                  # Lock screen (loginctl lock-session)
Print                            # Screenshot menu
shift + Print                    # Screenshot of a selected region
XF86Audio{RaiseVolume,LowerVolume} # Volume up/down
XF86AudioMute                    # Mute toggle
XF86MonBrightness{Up,Down}       # Brightness down/up
super + alt + ctrl + l           # Logout menu
```

### spectrwm-specific bindings (etc/spectrwm.conf)

```text
MOD + Return / Control+Alt+Return / Control+Alt+KP_Enter / Control+Alt+t / MOD+KP_Enter
                                  # Open terminal (myterminal, extra combos)
MOD + Shift + Return / MOD+Shift+KP_Enter / Control+Alt+B
                                  # Open browser (see TODO.AI.md: labeled "thunar")
MOD + Escape                     # xkill
MOD + Shift + q / MOD + q        # Kill window
MOD + x / Control+Alt+x          # Logout (see TODO.AI.md: arcolinux-logout)
MOD + Shift + s                  # Reload sxhkd (pkill -USR1 -x sxhkd)
MOD + Shift + y                  # Toggle bar
MOD + f                          # Toggle maximize
MOD + Shift + r                  # Restart spectrwm
MOD + equal / MOD + minus        # Grow/shrink window width
MOD + space / MOD + Shift + space # Cycle layout / reset stack
MOD + {Right,Left}                # Next/prev workspace (all)
MOD + {Up,Down}                   # Next/prev workspace
Control+Alt+{Right,Left}          # Next/prev workspace (all)
Control+Alt+{Up,Down}             # Next/prev workspace
MOD + Shift + {Up,Down}           # Swap next/prev window
MOD + Shift + {j,k}               # Swap next/prev window
MOD + Shift + {Left,Right}        # Flip layout
MOD + Shift + t                   # Toggle floating
MOD + Tab / MOD + Shift + Tab     # Focus next/prev window
Alt + Tab / Alt + Shift + Tab     # Focus next/prev window
MOD + u                           # Focus urgent window
MOD + {1-9,0}                     # Switch to workspace N
MOD + Shift + {1-9,0}             # Move window to workspace N
```
