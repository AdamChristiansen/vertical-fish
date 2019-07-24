# Vertical

A minimal git-aware prompt for the
[fish](https://github.com/fish-shell/fish-shell) with a definitive vertical
line.

![Screenshot](.image/screenshot.png?raw=true)

## Requirements

* [fish](https://github.com/fish-shell/fish-shell) (v2.7.0 or higher)

## Installation

### [Fisher](https://github.com/jorgebucaran/fisher)

```sh
fisher add AdamChristiansen/vertical-fish
```

## Configuration

The following options can be overridden in `config.fish`. Colors are always
specified as arguments to `set_color`. Any of the following that are not set
will be set to the default value.

**General**

| Option                  | Default | Description                          |
|-------------------------|---------|--------------------------------------|
| `VERTICAL_NORMAL_COLOR` | normal  | The default color.                   |
| `VERTICAL_NEWLINE`      | true    | Inserts a newline before the prompt. |

**Prompt**

| Option                       | Default  | Description       |
|------------------------------|----------|-------------------|
| `VERTICAL_VERT_PROMPT`       | `" "`    | The prompt text.  |
| `VERTICAL_VERT_PROMPT_COLOR` | `yellow` | The prompt color. |

**Vertical Bar**

| Option                     | Default | Description                                       |
|----------------------------|---------|---------------------------------------------------|
| `VERTICAL_VERT_PREFIX`     | `"│"`   | The prompt vertical bar.                          |
| `VERTICAL_VERT_COLOR_GOOD` | `green` | The bar color when the previous command succeeds. |
| `VERTICAL_VERT_COLOR_BAD`  | `red`   | The bar color when the previos command fails.     |

**Directory**

| Option                    | Default       | Description                                                 |
|---------------------------|---------------|-------------------------------------------------------------|
| `VERTICAL_DIR_COLOR`      | `blue --bold` | The directory name color.                                   |
| `VERTICAL_DIR_PREFIX`     | `" "`         | The directory name prefix.                                  |
| `VERTICAL_DIR_TRUNC_GIT`  | `true`        | Shorten directory relative to the root of a git repository. |
| `VERTICAL_DIR_TRUNC_HOME` | `true`        | Replaces `$HOME` with `~`.                                  |

**Git**

| Option                              | Default          | Description                    |
|-------------------------------------|------------------|--------------------------------|
| `VERTICAL_GIT_BRANCH_COLOR`         | `magenta --bold` | Git branch color.              |
| `VERTICAL_GIT_BRANCH_PREFIX`        | `" "`            | Git branch prefix.             |
| `VERTICAL_GIT_SHOW`                 | `true`           | Show git indicator.            |
| `VERTICAL_GIT_STATUS_COLOR`         | `cyan --bold`    | Git status color.              |
| `VERTICAL_GIT_STATUS_PREFIX`        | `" ["`           | Git status prefix.             |
| `VERTICAL_GIT_STATUS_SHOW`          | `true`           | Show the git status indicator. |
| `VERTICAL_GIT_STATUS_SUFFIX`        | `"]"`            | Git status suffix.             |
| `VERTICAL_GIT_STATUS_SYM_ADDED`     | `"+"`            | Git added status symbol.       |
| `VERTICAL_GIT_STATUS_SYM_AHEAD`     | `"↑"`            | Git ahead status symbol.       |
| `VERTICAL_GIT_STATUS_SYM_BEHIND`    | `"↓"`            | Git behind status symbol.      |
| `VERTICAL_GIT_STATUS_SYM_DIVERGED`  | `"⇵"`            | Git diverged status symbol.    |
| `VERTICAL_GIT_STATUS_SYM_DELETED`   | `"-"`            | Git deleted status symbol.     |
| `VERTICAL_GIT_STATUS_SYM_MODIFIED`  | `"!"`            | Git modified status symbol.    |
| `VERTICAL_GIT_STATUS_SYM_RENAMED`   | `"»"`            | Git renamed status symbol.     |
| `VERTICAL_GIT_STATUS_SYM_STASHED`   | `"#"`            | Git stashed status symbol.     |
| `VERTICAL_GIT_STATUS_SYM_UNMERGED`  | `"="`            | Git unmerged status symbol.    |
| `VERTICAL_GIT_STATUS_SYM_UNTRACKED` | `"?"`            | Git untracked status symbol.   |

**Duration**

| Option                     | Default         | Description                                                                            |
|----------------------------|-----------------|----------------------------------------------------------------------------------------|
| `VERTICAL_DURATION_COLOR`  | `yellow --bold` | The duration color.                                                                    |
| `VERTICAL_DURATION_MIN`    | `5000`          | The minimum command duration required to toggle the duration indicator (milliseconds). |
| `VERTICAL_DURATION_PREFIX` | `" "`           | The text before the duration.                                                          |
| `VERTICAL_DURATION_SHOW`   | `true`          | Show the duration indicator.                                                           |

**VI Mode**

| Option                             | Default         | Description                             |
|------------------------------------|-----------------|-----------------------------------------|
| `VERTICAL_VI_MODE_COLOR`           | `yellow --bold` | VI mode color.                          |
| `VERTICAL_VI_MODE_SHOW`            | `true`          | Show VI mode indicators.                |
| `VERTICAL_VI_MODE_SYM_INSERT`      | `""`            | The symbol to show in insert mode.      |
| `VERTICAL_VI_MODE_SYM_NORMAL`      | `"[N] "`        | The symbol to show in normal mode.      |
| `VERTICAL_VI_MODE_SYM_REPLACE_ONE` | `"[R] "`        | The symbol to show in replace one mode. |
| `VERTICAL_VI_MODE_SYM_VISUAL`      | `"[V] "`        | The symbol to show in visual mode.      |