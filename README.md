# Logseq Git-Sync

> **Warning**
>
> **DEPRECATED**, see new universal [App-Sync](https://github.com/brightdroid/app-sync)


This script can automatically "sync" your Logseq-Graphs with git.

## Preparations

  - Install/extract [Logseq](https://github.com/logseq/logseq) to e.g. `~/Apps/`
  - (optional) add symlink to Logseq in `~/bin/`:
    ```bash
    ln -st ~/bin ~/Apps/Logseq-linux-x64/Logseq
    ```
  - Clone this repo to e.g. `~/Apps/`:
    ```bash
    git clone https://github.com/brightdroid/logseq-sync.git ~/Apps/logseq-sync
    ```
  - Add symlink to `~/bin`:
    ```bash
    ln -st ~/bin ~/Apps/logseq-sync/logseq-sync
    ```

## Usage

After the preparations done use the command `logseq-sync` to open Logseq with all your Graphs.

### Example

Following example manages these Logseq-Graphs:
  - `~/Dokumente/logseq_graph1`
  - `~/Dokumente/logseq_graph2`

```bash
logseq-sync ~/Dokumente/logseq_graph1 ~/Dokumente/logseq_graph2
```

## FAQ

### Logseq not found

In case you didn't add a symlink to Logseq or your `PATH` doesn't contain `~/bin` you can call `logseq-sync` like this:

```bash
logseq-sync -l /path/to/logseq/dir GRAPH...
```
