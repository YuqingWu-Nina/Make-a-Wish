# Make a Wish! — Design Plan

## Project idea

**Make a Wish!** is a small browser-based birthday-cake maker. It gives someone a playful way to personalize a cake and turn it into a short digital birthday surprise.

## Intended experience

The creator builds a cake with choices that are easy to understand: flavor, cream, topping, cake picks, an optional local image, and a birthday message. The key moment happens when the candles are blown out and the message appears with confetti.

The project also includes a darker **mock recipient preview**. It demonstrates what a recipient would experience after opening a birthday-cake link, while staying honest that this front-end project does not provide real online storage or delivery.

## Current interaction flow

1. Choose a cake flavor, cream flavor, and topping style.
2. Choose one of six fixed cake-pick spots.
3. Add a preset pick, customize a number or banner, or replace the selected pick with one local image.
4. Write a short birthday message.
5. Select **Make a Wish** to extinguish the candles, show confetti, and reveal the message.
6. Select **Create share link** to make a mock recipient-preview URL.
7. In recipient preview, select **Blow Out the Candles** to brighten the scene, show confetti, and reveal the saved message.

## Visual direction

- A warm pastel palette of pink, cream, lavender, pale gold, and soft blue.
- A centered layered cluster of six cake picks: banner, number, balloons, star, cat, and gift.
- Separate wooden-stick layers behind the cream surface, so the picks look inserted into the cake.
- A calm party-room display background made with CSS: a soft gradient, subtle bunting, faint edge balloons, sparse sparkles, dots, and a glow under the cake.
- A darker but still readable version of the same atmosphere for recipient preview.

## Technical choices

- One `index.html` file keeps the HTML, CSS, and JavaScript together for this beginner learning project.
- Fixed topper positions are used instead of drag-and-drop so the arrangement stays intentional and the interaction remains easy to test.
- CSS variables update cake, cream, and topping colors without needing external assets.
- A local image uses `URL.createObjectURL()`, which keeps it in the current browser rather than uploading it to a server.
- The mock recipient URL stores preset choices and the message in URL parameters.

## Current limitations

- The mock recipient link is a front-end demonstration, not a real sharing service.
- Uploaded images stay private in the creator's browser and are not included in the mock URL.
- The project has no accounts, saved cakes, email delivery, or backend storage.
- Automatic image extraction or background removal is not included.

## Possible future exploration

- User testing and accessibility review.
- Hosting the project with GitHub Pages.
- A real sharing workflow only after planning secure image storage and privacy.
