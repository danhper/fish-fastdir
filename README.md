# fish-fastdir

## Installation

### Using [fundle](https://github.com/tuvistavie/fundle) (recommended)

Add

```
fundle plugin 'tuvistavie/fish-fastdir'
```

to your `config.fish` and run `fundle install`.

### Manually

Put `functions/__fastdir_cd_num.fish` and `functions/__fastdir_dirhist.fish` in
your `~/.config/fish/functions` directory, and source `init.fish` on startup.

## Usage

Fish plugin to improve directory navigations.

The following aliases are provided:

* `-`: `cd  -`
* `..`: `cd ..`
* `...`: `cd ../..`
* `....`: `cd ../../..`
* `.....`: `cd ../../../..`
* `1` ~ `9`: Goes to the nth directory in the stack
* `d`: Shows the directory history stack with associated numbers.

  Sample output:

    ```
    1 /home/daniel/.config/fish/fundle/tuvistavie/fish-fastdir
  2 /home/daniel
  3 /home/daniel/Dropbox
  5 /home/daniel/Dropbox/tmp
  4 /usr/local
    ```

In the above output, if you use `2`, the directory will become `/home/daniel`,
and `nextd` will be `/home/daniel/Dropbox`.
