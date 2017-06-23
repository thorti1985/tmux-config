# tmux-config
My tmux config

# tmux - Tutorial

```bash
# Create new tmux session
tmux new -s <session-name>

# Attach to that session
tmux a -t <session-name>

# Detach from session
Strg-b + d

# Sharing session with sockets (it seems also to work with a "normal" session. So currently I don't know the difference/benefits of using sockets or names)
 1) Create new tmux session with specific socket
    tmux -S /tmp/tmpsocket
 2) Allow access to that socket (step is not always required)
    chmod 777 /tmp/tmpsocket
 3) Attach from other 
    tmux -S /tmp/tmpsocket attach
```
