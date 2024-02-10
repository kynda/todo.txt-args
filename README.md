# Multi-length argument commands for [todotxt-cli]

Collection of commands to replace the built-in commands allowing for variable
argument length and a couple extra useful ones as well.

## Install

```
git clone https://github.com/kynda/todo.txt-args.git
ln -s todo.txt-args/* $TODOTXT_ACTIONS_DIR
```

## Usage

### `gc`

```
Usage
    gc [lsp]"
        generates a textual report of pending and completed tasks in all
        projects and contexts and groups them by the context they belong
        to.
```

### `gp`

```
Usage
    gp [lsp]"
        generates a textual report of pending and completed tasks in all
        projects and contexts and groups them by the context they belong
        to.
```

### `addx`

```
Usage
  $curcmd \"THING I DID +project @context\"
    Add an item and mark it as done in one step
```

### `commit`

```
Usage
    Record all changes in Git repository located at $TODO_DIR.
      If -v argument is provided, only a preview will be shown.
```	

### `edit`

```
Usage
  Open \$TODO_DIR/BASENAME.txt in \$EDITOR.
    If BASENAME is not given, defaults to 'todo'.
```

### `p` or `pri`

```
Usage
  $ todo.sh pri ITEM#[, ITEM#, ITEM#, ...] PRIORITY
    For each ITEM#, calls pri with priority PRIORITY
             
  Examples
    $ todo.sh pri 1 2 3 a
```

### `repeat`

```
Usage
  repeat ITEM#[, ITEM#, ITEM#, ...] PRIORITY
    For each ITEM#, mark done, then add with PRIORITY.
```

### `rm`

```
Usage
  $ todo.sh rm ITEM#{, ITEM#, ITEM#, ...]
    For each ITEM#, calls rm

  Examples
    $ todo.sh rm 1 2 3
```

## License

GPL3

[todotxt-cli]: https://github.com/todotxt/todotxt-cli
