# awesome_config

A configuration for the [awesome](https://awesomewm.org) window manager. The keyboard shortcuts are consistent with those in my [vim configuration](http://MauroCalderara/vim_config) and [tmux configuration](http://MauroCalderara/tmux_config), where possible.

- [Overview](#overview)
- [Installation](#installation)
- [Key sequences](#key sequences)

Overview
---

The configuration uses the `windows key` and vim-style movement keys (`h`=&larr;, `j`=&darr;, `k`=&uarr;, `l`=&rarr;) to navigate windows and move them around. The row above the home row refers to awesome tags (`u`=&darr;, `i`=&uarr;), for multiple screens the brackets are used (`[`=&larr;, `]`=&rarr;). Movements in the respective directions employ the `windows key` + `shift` with the same keys as for navigation.

The configuration has been tested on Ubuntu 16.04.

Installation
---

The configuration can be cloned into `~/.config/awesome`. The actual configuration is in `config.lua` while `rc.lua` is ignored by git. It is recommended that `config.lua` is symlinked to `rc.lua`. The repository includes [cyclefocus](https://github.com/blueyed/awesome-cyclefocus) as a submodule.

Some aspects of the configuration are very user specific
Things to configure (local.lua)
    terminal
    editor
    org-mode launch ('User defined launch')

Key sequences
---

Note: By default 'modkey' is the windows key.

| Task | Key sequence |
| ---- | ------------: |
| Launch command (promptbox) | `modkey + space` |
| Start shell | `modkey + n` |
| User defined launch | `modkey + o` |
| |
| Go to next window | `modkey + l` or `modkey + k` |
| Go to previous window | `modkey + h` or `modkey + j` |
| Close window | `modkey + w` |
| Make window the master | `modkey + Enter` |
| Minimize window | `modkey + d` |
| |
| Cycle through all windows on all tags | `modkey + Tab` |
| Cycle through all minimized windows on current tag\* | ``modkey +  ` `` |
| |
| Swap with next window | `modkey + L` or `modkey + K` |
| Swap with previous window | `modkey + H` or `modkey + J` |
| Toggle floating | `modkey + f` |
| Toggle maximized | `modkey + m` |
| Toggle full screen (hiding menu) | `modkey + f` |
| Toggle stickyness | `modkey + s` |
| |
| Show previous/next tag | `modkey + u/i` |
| Show tag <n> | `modkey + <n>` |
| Toggle tag <n>'s visibility | `modkey + shift + <n>` |
| Move window to previous/next tag | `modkey + shift + u/i` |
| |
| Increase master area | `modkey + ;` or `modkey + /` |
| Decrease master area | `modkey + y` or `modkey + g` |
| Create vertical split | `modkey + shift + \` |
| Remove vertical split | `modkey + \` |
| Create horizontal split | `modkey + shift + -` |
| Remove horizontal split | `modkey + -` |
| Cycle through layouts | `modkey + '` |
| Toggle menu bar visibility | `modkey + t` |
| |
| Configure second display | `XF86Display` |
| Focus on next/right screen | `modkey + ]` |
| Focus on previous/left screen | `modkey + [` |
| Move client to next/right screen | `modkey + shift + ]` |
| Move client to previous/left screen | `modkey + shift + [` |
| |
| Increase volume | `XF86AudioRaiseVolume` |
| Decrease volume | `XF86AudioLowerVolume` |
| Mute | `XF86AudioMute` |
| Make screenshot | `modkey + print` |
| | 
| Restart awesome | `modkey + r` |
| Quite awesome | `modkey + q` |

\* This currently only works if there are non-mimized windows on the current tag.

## Using the mouse

The mouse generally can be used to move windows and set the focus. Windows can be moved in all layouts by dragging them with `modkey + mouse1`. In the floating layout, windows can be resized with `modkey + mouse3`
