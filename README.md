# dwm-build

Custom `dwm 6.5` build with a small set of practical changes on top of upstream.

## Overview

This build keeps the default `dwm` feel, but adds a few workflow changes:

- Fibonacci layouts are included (`spiral` and `dwindle`)
- New windows use `attachaside` behavior instead of always attaching at the head of the stack
- `Print` launches `flameshot gui`
- `Mod+Shift+g` launches `ghostty`

## Layouts

The current layout set is:

- `[]=` tile
- `><>` floating
- `[M]` monocle
- `[@]` spiral
- `[\\]` dwindle

Layout keybindings:

- `Mod+t` sets tile layout
- `Mod+f` sets floating layout
- `Mod+m` sets monocle layout
- `Mod+r` sets spiral layout
- `Mod+Shift+r` sets dwindle layout
- `Mod+Space` cycles the active layout
- `Mod+Shift+Space` toggles floating for the focused window

## Custom keybindings

In addition to the standard `dwm` bindings:

- `Mod+Shift+g` launches `ghostty`
- `Print` launches `flameshot gui`

## Notes

`attachaside` changes how new tiled windows are inserted, which keeps new clients from always taking the top position in the stack.

This build expects `ghostty` and `flameshot` to be installed and available on the `PATH` used by your `dwm` session.
