# Make a Wish!

> Working title — we will rename this folder and update this file once the project idea is clear.

## Project idea

A playful browser-based Birthday Cake Maker for creating a personalized digital birthday surprise. Version 2.0 adds seven cake flavors, cream and topping choices, and a layered set of six different-shaped cake picks that can be replaced with presets or one uploaded personal image. See `Design.md` for the full plan.

## How to run it

Open `index.html` in a web browser. For a local preview server, open a terminal inside this folder and run:

```bash
python3 -m http.server 8765
```

Then visit `http://localhost:8765` in your browser.

## Sharing a cake

Use **Create share link** after decorating a cake. The link saves the cake flavor, cream, topping, preset picks, and birthday message in the URL. A friend who opens it sees a fresh cake with lit candles and can click **Make a Wish**.

The optional uploaded picture stays only in the creator's browser, so it is not included in the link. To share a link with friends, the project must be hosted online (for example, with GitHub Pages); a `file://` link only works on the creator's computer.

## What is in this folder?

- `README.md` — the project overview and instructions.
- `Learning-note.md` — a dated record of what I learn and change.
- `Design.md` — the project idea, interaction plan, and scope.
- `index.html` — the complete website. Its HTML, CSS, and JavaScript are kept together for this beginner learning project.
