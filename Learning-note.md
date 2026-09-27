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
