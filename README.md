# Portrait of Biscuit

A framed vector portrait of a sitting golden retriever, with a museum-style gallery label.
One HTML file, no dependencies, no build step.

## Viewing it

Open `index.html` in any browser. That's the whole thing.

To serve it as a web page, turn on GitHub Pages for this repo
(**Settings → Pages → Branch: `main` / root**) and it will be live at
`https://<username>.github.io/<repo>/`.

## What's in it

- **Hand-authored SVG** — the dog is built from ellipses, rounded rects, and a handful of
  bezier curves. No raster images, so it stays sharp at any size.
- **Theme-aware** — the gallery wall follows the viewer's light/dark preference via
  `prefers-color-scheme`. The painting itself keeps its colors in either light.
- **One bit of motion** — hover the frame and his tail wags. Disabled under
  `prefers-reduced-motion`.

## Tweaking him

All the colors are CSS custom properties at the top of the file. The painting's palette is
separate from the wall's, so you can recolor the dog without touching the theme:

| Variable | What it colors |
| --- | --- |
| `--fur` / `--fur-dark` | coat, ears, tail, haunches |
| `--cream` / `--cream-dim` | chest, paws, muzzle, toe lines |
| `--dark` | nose, eyes, mouth |
| `--tongue` | tongue |
| `--brass` / `--tag` | collar and tag |
| `--wall` / `--ink` | the room around the frame |

Swap `--fur` for a grey and `--cream` for a lighter grey and he's a different dog.
