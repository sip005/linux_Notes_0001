Sure, here's a cheat sheet for tmux, a popular terminal multiplexer that allows you to manage multiple terminal sessions in a single terminal window.

### Basic tmux Commands:

1. **Starting a new session:**
   - `tmux`: Start a new tmux session.
   - `tmux new -s <session-name>`: Start a new session with a specific name.

2. **Detaching and attaching to sessions:**
   - `Ctrl-b d` or `tmux detach`: Detach from the current session.
   - `tmux ls`: List existing sessions.
   - `tmux attach -t <session-name>`: Attach to a specific session.

3. **Managing windows:**
   - `Ctrl-b c` or `tmux new-window`: Create a new window.
   - `Ctrl-b ,` or `tmux rename-window <new-name>`: Rename the current window.
   - `Ctrl-b p` or `Ctrl-b n` or `tmux prev-window` and `tmux next-window`: Navigate between windows.
   - `Ctrl-b &` or `tmux kill-window`: Close the current window.

4. **Splitting panes:**
   - `Ctrl-b %` or `tmux split-window -h`: Split the current pane horizontally.
   - `Ctrl-b "` or `tmux split-window -v`: Split the current pane vertically.
   - `Ctrl-b o` or `tmux select-pane -t :.+` (cycle through panes).

5. **Resizing panes:**
   - `Ctrl-b <resize-key>` (e.g., `Ctrl-b : resize-pane -U`, `Ctrl-b : resize-pane -D`): Resize the current pane.
   - You can use `Ctrl-b ?` to see a list of available resize keys.

6. **Scrolling in panes:**
   - `Ctrl-b [` or `tmux scroll-up`: Enter scroll mode, then use arrow keys or Page Up/Down to scroll.
   - Press `q` to exit scroll mode.

7. **Other useful commands:**
   - `Ctrl-b ?` or `tmux list-keys`: List all tmux key bindings.
   - `Ctrl-b :` or `tmux command-prompt`: Enter a command in the status bar.

### Customizing tmux:

8. **Customizing the tmux configuration:**
   - You can create a `~/.tmux.conf` file to customize your tmux environment with various settings, key bindings, and options.

### Advanced Usage:

9. **Named sessions and windows:**
   - Naming sessions and windows can make it easier to manage multiple sessions and windows.

10. **Session management:**
    - `tmux kill-session -t <session-name>`: Terminate a specific session.
    - `tmux switch-client -n`: Cycle through clients attached to the current session.

11. **Copy mode:**
    - `Ctrl-b [` to enter copy mode (as mentioned earlier) or use `tmux copy-mode`.
    - In copy mode, you can search for text, copy, and paste.

12. **Custom key bindings:**
    - You can customize key bindings in your `~/.tmux.conf` file to suit your preferences.

This cheat sheet should help you get started with tmux. Remember that tmux is highly customizable, so you can adapt it to your workflow and preferences.
