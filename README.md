# Installation
[Tmux Installation](https://github.com/tmux/tmux/wiki/Installing)

# Getting Started
[Getting Started](https://github.com/tmux/tmux/wiki/Getting-Started)

# Tmux Commands

## Sessions

### New Session

* `tmux new [-s name] [cmd]` (`:new`) - new session

### Switch Session

* `tmux ls` (`:ls`) - list sessions
* `tmux switch [-t name]` (`:switch`) - switches to an existing session
* `tmux as [id] [-t name]` (`:attach`) - attaches to an existing session
* `<C-a>c` (`:detach`) - detach the currently attached session

### Session Management

* `<C-a>s` - list sessions
* `<C-a>$` - name session

### Close Session

* `tmux kill-session [-t name]` (`:kill-session`)

## Windows

### New Window

* `<C-a>c` (`:neww [-n name] [cmd]`) - new window

### Cursor Movement

* `<C-a>[i]` (`:selectw -t [i]`) - go to window `[i]`
* `<C-a>l` - go to last window
* `<C-a>p` - go to previous window
* `<C-a>n` - go to next window

### Window Management

* `<C-a>T` - rename window
* `<C-a>,` - rename window
* `<C-a>w` - list all windows
* `<C-a>f` - find window by name
* `<C-a>.` - move window to another session (promt)
* `:movew` - move window to next unused number

### Close Window

* `<C-a>&` (`:kill-window`) - kill window

## Panes

### New Pane

* (%) `<C-a>|` (`:splitw [-v] [-p width] [-t focus] [cmd]`) - split current pane vertically
* (") `<C-a>s` (`:splitw -h [-p width] [-t focus] [cmd]`) - split current pane horizontally

### Cursor Movement

* (o) `<C-a><Tab>` (`:selectp -t :.+`) - move cursor to the next pane
* `<C-a><Up>` (`:selectp -U`) - move cursor to the pane above
* `<C-a><Down>` (`:selectp -D`) - move cursor to the pane below
* `<C-a><Left>` (`:selectp -L`) - move cursor to the pane to the left
* `<C-a><Right>` (`:selectp -R`) - move cursor to the pane to the right
* `:selectp [i]` - move cursor to the pane `[i]`

### Panes Management

* (`:swap-pane -U`) - move current pane up
* (`:swap-pane -D`) - move current pane down
* `<C-a>{` (`:swap-pane -L`) - move current pane to the left
* `<C-a>}` (`:swap-pane -R`) - move current pane to the right
* `<C-a>q` - show pane numbers (type number to move cursor)
* `<C-a><Space>` - toggle pane arrangements

### Resize Pane

* `:resize-pane -U [i]` - move horizontal divider up by `[i]` lines
* `:resize-pane -D [i]` - move horizontal divider down by `[i]` lines
* `:resize-pane -L [i]` - move vertical divider left by `[i]` columns
* `:resize-pane -R [i]` - move vertical divider right by `[i]` columns

`resize-pane [-DLRUZ] [-x width] [-y height] [-t target-pane] [adjustment]`

### Close Pane

* `<C-a>x` (`:kill-pane`) - kill current pane

## Misc

* `<C-a>t` - show time
* `<C-a>r` - reload config

# Plugins
[Tmux Plugins](https://github.com/tmux-plugins/tpm)

# References
[Jaime's Guide to Tmux](https://www.barbarianmeetscoding.com/blog/jaimes-guide-to-tmux-the-most-awesome-tool-you-didnt-know-you-needed)
[Tao of Tmux](https://leanpub.com/the-tao-of-tmux/read)
[Starefossen CheatSheet](https://gist.github.com/Starefossen/5955406)

# Acknowledgments
Thanks to anyone who's code/framework/references/examples are used

