# Learning Notes

## September 27, 2026

### Setup

- Created a temporary project folder named `project-draft`.
- Added a `README.md` to explain the project.
- Added this learning note so I can record decisions, tests, questions, and discoveries as I work.

### Next step

Choose a small project idea and a final project name.

## September 27, 2026 — Idea chosen

- Chose the project name **Make a Wish!**
- Planned a Birthday Cake Maker with a photo topper, custom message, candle animation, and confetti.
- Wrote `Design.md` to keep the feature list and first-version scope clear.

## September 27, 2026 — First website version

- Built the whole project in one `index.html` file: HTML creates the page content, CSS creates the visual style, and JavaScript makes it interactive.
- Added cake flavor choices, a local image upload, a message box, candle blow-out animation, confetti, and a reset button.
- The uploaded photo is shown with `URL.createObjectURL()`. This creates a temporary browser-only link, so the image is not sent to a server.
- Added code comments that connect each user action (input) to the change that appears on screen (output).

## September 27, 2026 — Version 2.0 decoration studio

- Added more cake flavors: lemon, matcha, and rainbow, in addition to the first four flavors.
- Replaced the one photo topper with six fixed decoration spots. This is simpler than drag-and-drop because each sign has a clear, intentional place on the cake.
- Added preset signs (balloon, heart, star, gift, mini cake, and message card). Clicking a cake spot chooses where the next preset or uploaded image appears.
- Kept custom images browser-only. Background removal/image extraction is not included because reliable extraction would need a larger image-processing tool or AI service.

### Saved milestone

- Saved this working version as **Version 2.0** before planning the next visual redesign.
- The next plan is to make the decorations look like layered, differently shaped cake picks with sticks, inspired by real birthday topper sets.

## September 27, 2026 — Layered cake-pick redesign

- Redesigned the cake as a small cylinder with a visible cream-covered top surface.
- Added four cream flavors and four topping choices. JavaScript changes CSS variables, which repaint the cream and topping on the cake immediately.
- Changed the six matching round signs into a layered set of different-shaped cake picks: banner, number badge, balloon bunch, star, party character, and gift.
- Each pick keeps a visible stick and a separate position, so the decoration arrangement feels closer to a real birthday cake topper set.

## September 27, 2026 — Visual refinement

- Improved the visual style with patterned backgrounds, layered shadows, decorative frosting piping, textured cake sides, and more detailed pick patterns.
- Replaced most in-cake emoji artwork with simple text and CSS-drawn patterns, so the topper arrangement feels more like a designed paper set.

## September 27, 2026 — Stick fix and style choice

- Fixed disappearing wooden sticks by separating each pick's patterned artwork from its outer button. The stick now belongs to the outer layer, while clipping only shapes the inner artwork.
- Tried a generated cake texture, then returned to the lighter emoji-style design because it better matches the playful feel of this project.

## September 28, 2026 — Return to emoji-style reference version

- Restored the earlier single-cake emoji-style composition after testing tiered and bento-cake variations.
- Kept the separate inner artwork and outer stick structure, so the earlier visual style still benefits from the wooden-stick bug fix.

## September 28, 2026 — Share-link interaction

- Added a **Create share link** button. JavaScript stores the cake choices, preset pick designs, and birthday message in URL parameters.
- When the link is opened, JavaScript reads those parameters and rebuilds the cake with lit candles. The friend can then click **Make a Wish** to show the message and confetti.
- A locally uploaded photo is intentionally not included in the link. Without a backend, keeping a photo in the URL would create an unreliable and overly long link.

## September 28, 2026 — Stage-first workshop layout

- Added a short reminder next to the share button explaining that sharing currently includes preset choices and the message, but not local uploaded photos.
- Replaced the stretched equal-height columns with a stage-first layout. The cake preview has its own intentional height, so it does not gain large empty areas just because the controls are tall.
- Kept cake styling and topper choices (steps 1–4) beside the preview. Moved the personal photo, message, wish button, and sharing actions into a clearly named finishing section below.

## September 28, 2026 — Compact desktop customizer

- Widened the desktop workspace so the cake choices use the available screen space instead of creating large empty margins at the sides.
- The flavor choices now use two readable rows, while the cream and topping choices fit on one row. This shortens the left panel without making its choice buttons smaller.
- Made the six cake-pick buttons a little shorter and reduced section spacing. The left panel now sits much closer to the height of the preview, so the finishing section begins without a large empty gap.
