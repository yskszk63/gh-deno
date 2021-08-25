# gh deno

Simply run deno script github cli extension.

Currently work in progress.

## Install

```bash
gh extension install yskszk63/gh-deno
```

## Example

Run welcome.ts.

```bash
$ gh deno https://deno.land/std/examples/welcome.ts
Welcome to Deno!
```

Implement Plugin.

[yskszk63/gh-deno-example](https://github.com/yskszk63/gh-deno-example)

```bash
#!/bin/bash
set -e

# ensure installed yskszk63/gh-deno.
gh deno --ping > /dev/null 2>&1 || gh extension install yskszk63/gh-deno
exec gh deno 'https://cdn.jsdelivr.net/gh/yskszk63/gh-deno-example/index.ts'
```

## License

MIT

## Author

[yskszk63](https://github.com/yskszk63)
