## Basic Commands

Note: The prefix key is `Ctrl+b` by default

- Start new session: `tmux`
- Start new named session: `tmux new -s session_name`
- Attach to existing session: `tmux attach -t session_name`
- List sessions: `tmux ls`
- Kill session: `tmux kill-session -t session_name`
#### Key Bindings
To use these commands, first press the prefix key (Ctrl+b), then release it, and finally press the command key.
These can be changed or further customised from `~/.tmux.conf`
#### Session Management
- Detach from session: `prefix d`
- List sessions: `prefix s`
- Rename session: `prefix $`
#### Window Management
- Create new window: `prefix c`
- Next window: `prefix n`
- Previous window: `prefix p`
- Switch to window by number: `prefix 0-9`
- Rename window: `prefix ,`
- Close current window: `prefix &`
#### Pane Management
- Split pane horizontally: `prefix %`
- Split pane vertically: `prefix "`
- Switch to next pane: `prefix o`
- Switch to pane by direction: `prefix arrow_key`
- Toggle pane zoom: `prefix z`
- Close current pane: `prefix x`
#### Misc
- Enter copy mode: `prefix [`
- Paste from buffer: `prefix ]`
- Show time: `prefix t`
- Show help: `prefix ?`
