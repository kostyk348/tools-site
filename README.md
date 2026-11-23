# tools-site — the landing page for `kostyk348/tools`

Static, single-file landing page for the [tools](https://github.com/kostyk348/tools) repository:
small dependency-free system services for Linux (the tunnel that replays a TLS handshake, the
network read as files, an exactly-once job queue, hash-free deduplication, scheduler jitter
measurement).

## What is here

| File | Role |
|---|---|
| `index.html` | the whole page: markup, styles and scripts inline, no build step, no external assets |
| `.nojekyll` | tells GitHub Pages to serve the files as-is instead of running Jekyll |

Served at <https://kostyk348.github.io/tools-site/> from the repository root.

## Editing

Nothing to build: change `index.html` and push. To look at it locally, open the file directly —

```bash
# from the repository root
xdg-open index.html        # or: start index.html / open index.html
```

or serve the directory if you want the same origin behaviour Pages gives:

```bash
npx --yes serve .
```

Keep the numbers on the page honest: they must match the `tools` README (tool count, what each one
does), because a visitor compares the two pages.
