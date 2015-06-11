# ctrl-c

This is a way to interrupt remote employees as effectively as you can interrupt in-office employees.

# Dependencies

## Server

- `bash`
- [`httprintf`](https://github.com/ianthehenry/httprintf)
- `coreutils` (`touch`)

## Client

- `bash`
- `curl`
- OS X's `open` command
- `coreutils` (`sleep`)

# Still TODO

- Write an interrupting client (rather than an interrupted client). Currently interruption is two step: `curl -X POST` and `open`ing `appear.in` manually. That should be a script. The current client script should probably be renamed. `ctrl-cd`? `ctrl-d`?
- Use an environment variable for the domain, instead of hardcoding it.
- Add interruption of specific users by name.
