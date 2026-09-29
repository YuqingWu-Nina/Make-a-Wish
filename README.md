# Make a Wish! — Birthday Cake Maker

## Project overview

**Make a Wish!** is a small browser-based birthday-cake maker. I made it as a playful, personal interaction rather than a realistic baking tool: a user builds a cake, adds cake picks and a message, then turns it into a small birthday moment.

My original idea was simple: **When someone personalizes a birthday cake and makes a wish, the experience should feel like creating and opening a small digital birthday surprise.** I kept the project in one `index.html` file so I could focus on learning how HTML, CSS, and JavaScript work together in one complete interaction.

Live demo: Add GitHub Pages URL after publishing.

## Core interaction

1. Choose a cake flavor, cream flavor, and topping style.
2. Choose one of six fixed cake-pick spots, then select a preset pick or customize a number or banner.
3. Optionally upload one local image to replace the selected cake pick.
4. Write a short birthday message.
5. Select **Make a Wish** to turn off the candles, show confetti, and reveal the message.
6. Select **Create share link** to generate a front-end-only mock recipient link. Opening the mock link shows a darker recipient-preview experience with lit candles.
7. In that preview, the recipient selects **Blow Out the Candles**. The scene brightens, confetti falls, and the saved message appears.

## How to run

Open `index.html` directly in a modern web browser.

For a local preview server, open Terminal in this project folder and run:

```bash
python3 -m http.server 8765
```

Then open [http://localhost:8765](http://localhost:8765) in a browser.

## AI process

I used Codex as an AI coding partner. It helped translate my visual and interaction requests into HTML, CSS, and JavaScript, but I made the decisions about the project direction, what felt too crowded, and what should remain honest about the project's limits.

Representative prompts or prompt summaries from my process:

- Build a small birthday-cake maker with local photo upload, a message, candles, confetti, and a reset action.
- Fix the cake-pick sticks so they appear inserted behind the cream instead of floating on top of it.
- Recompose the six picks into a tighter central celebration cluster, then simplify the balloon and cat designs when they did not look clear enough.
- Turn the idea of a real shareable cake link into a clearly labeled mock recipient preview because this project has no backend or accounts.

AI suggested implementation approaches and helped revise code. I decided which visual direction to keep, asked for more precise changes when the cake or topper layout did not match my intention, and chose not to present the mock link as a real sharing service.

## Testing and revisions

| What I expected | What happened or what I checked | Revision or current limitation |
| --- | --- | --- |
| Each topper should look like it is planted in the cake. | The sticks could disappear or appear on top of the cream when a pick changed. | The sticks now use a separate background layer behind the cream and below the clickable topper artwork. |
| Six picks should read as one celebratory arrangement, not six evenly spaced objects. | The first wide arrangement felt disconnected and some artwork felt awkward. | I tightened the group into back and front rows, kept the number as the focal point, and simplified the balloon and cat picks. |
| A recipient should be able to open the designed cake. | A real saved link would require a backend, which this project does not have. | The link is a front-end-only mock recipient preview that stores preset settings and the message in the URL. |
| A personal photo should be safe and reliable. | A local browser image cannot be reliably stored in a short URL without a server. | Uploaded photos stay private in the creator's browser and are excluded from the mock URL. |

## Reflection

The finished project matches my intention most strongly in the small surprise moment: the user can make choices, see the cake change, and then reveal a birthday message through the candle interaction. The cake-pick cluster and the softer preview background also made the experience feel more intentional. At first, the cake looked too simple, the sticks did not look inserted, and the topper arrangement felt too spread out. I noticed those problems while looking at the page and responded by giving more specific visual instructions instead of accepting the first result.

Codex helped me move quickly from an idea to working code and helped explain how the visual layers and URL parameters work. However, I still needed to decide what counted as a successful visual result, which features were too complicated for the assignment, and how to describe the project honestly. Real online sharing remains unresolved because it needs storage and a backend. I chose a mock recipient flow because it demonstrates the intended experience without pretending that the project can save or deliver a private cake online.

## Current limitations

- Mock links are for demonstration only; they are not a backend sharing service.
- Uploaded images remain private and local to the creator's browser.
- The project should be hosted with GitHub Pages before it is shared publicly.

## Project files

- `index.html` — the complete interactive website, including HTML, CSS, and JavaScript.
- `README.md` — this instructor-facing project overview and reflection.
- `Learning-note.md` — a development journal of decisions and revisions.
- `Design.md` — the original design plan and early scope notes.
