# Tmux tutorial

Tmux is a powerful terminal multiplexer that allows you to manage multiple terminal sessions within a single window. It’s especially useful for working with remote servers or managing many terminal windows on your local machine.

# How to install tmux

You can install tmux in Ubuntu using this command:

```
sudo apt install tmux
```

Or of you are using mac using:

```
brew install tmux
```

## Starting a new session we start using this command:

```
tmux
```

Alternatively to start a named session we use the command:

```
tmux new-session -s session-name
```

You can attach a session that is already running by using the command:

```
tmux new-session -A session-name
```

## Killing a session

We can kill a specific session by use of command:

```
tmux kill-session -t session-name
```

Or

```
tmux kill-session -t session-name
```

If you want to kill all sessions we use:

```
tmux kill-session -a
```

alternatively we can kill all sessions but specific session, we use:

```
tmux kill-session -a -t specific-name
```

## To preview windows we use the command:

```
Ctrl+b w
```
## We can create a named window when creating a session using the command:

```
tmux new-session -s session-name -n window-name
```
### When already in a window we can create another window using the command

```
Ctrl+b c
```

### Renaming a window

```
Ctrl+b ,
```

### Closing a window

```
Ctrl+b &
```

#### Finally panes are where we can type our code or running a script. To split a pane we use:

```
Ctrl+b %
```

#### Finally splitting a pane horizontally we use the command:

```
Ctrl+b "
```

##### Movement in different panes we use the arrow keys to move either up, down, left or right.
