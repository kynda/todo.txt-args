# Multi-length argument commands for [todotxt-cli]

Collection of commands to replace the built-in commands allowing for variable
argument length

## Install

```
git clone https://github.com/kynda/todo.txt-args.git
ln -s todo.txt-args/p $TODOTXT_ACTIONS_DIR/p
ln -s todo.txt-args/pri $TODOTXT_ACTIONS_DIR/pri
ln -s todo.txt-args/rm $TODOTXT_ACTIONS_DIR/rm
```

## Usage

### `p` or `pri`

```
Usage
  $ todo.sh pri ITEM#[, ITEM#, ITEM#, ...] PRIORITY
    For each ITEM#, calls pri with priority PRIORITY
             
  Examples
    $ todo.sh pri 1 2 3 a
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
