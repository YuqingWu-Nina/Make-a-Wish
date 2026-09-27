# Make a Wish! — Design Plan

## What we are making

**Make a Wish!** is a small, playful browser-based Birthday Cake Maker. It lets someone create a personalized digital birthday surprise for another person.

## The main experience

1. The user sees a colorful birthday cake with lit candles.
2. They upload one image from their computer.
3. The image appears above the cake as a round decorative topper with a gold border and a small stick.
4. They type a short birthday message (up to about 80 characters).
5. They click **Make a Wish**.
6. The candles turn off, confetti falls, and the birthday message appears in a celebration card beside or below the cake.

## Small personalization choices

- Choose one of a few cake colors/flavors: Strawberry, Vanilla, Chocolate, or Blueberry.
- Upload a photo for the cake topper.
- Write a short custom birthday message.

## Polish details

- The main button changes to **Wish Made!** after it is clicked, so the animation does not replay accidentally.
- A **Make Another Cake** button resets the page for a new surprise.
- The photo stays in the browser only; it is not uploaded to a server.

## What we will not build in the first version

- User accounts or saved cakes.
- Sending emails or messages.
- Online sharing features.
- Real music or complicated sound controls.

Keeping the first version small will help us finish, test, and explain one complete interaction well.

## Saved milestone: Version 2.0

Version 2.0 is the current saved version. It adds seven cake flavors and six fixed decoration spots, where a user can choose a preset sign or upload one personal image.

## Next design direction: layered cake-pick set

The next version will replace the matching round decoration spots with a small collection of **different die-cut cake picks**, inspired by real birthday cake toppers.

### Visual idea

- Each pick has its own silhouette and pattern, such as a party-hat sign, curved “Happy Birthday” banner, balloon bunch, star, age/number badge, gift, or character face.
- Each pick has a visible wooden stick that appears inserted into the cake.
- Picks are arranged in three visual layers: tall picks at the back, a large feature pick in the middle, and smaller picks at the front.
- The picks overlap slightly to feel like one celebratory arrangement instead of six separate buttons.

### Cake customization ideas

1. **Cake flavor**: choose the cake color/base flavor.
2. **Cream flavor**: choose a frosting style and color, for example vanilla whipped cream, strawberry pink cream, chocolate swirl, or matcha cream.
3. **Top decorations**: choose one light sprinkle layer, such as rainbow sprinkles, berries, candy pearls, cookie crumbs, or fruit cubes.

### Suggested build order

1. Redraw the cake as a more realistic small cylinder with a visible top surface.
2. Add cream style and sprinkle choices to that top surface.
3. Build a small preset library of different-shaped picks with CSS and emoji/text artwork.
4. Place those picks in fixed back/middle/front positions.
5. Keep custom-image upload as an optional replacement for one selected pick.

We will still avoid automatic background removal for now. Good image extraction needs larger image-processing tools or an external AI service, while this project is designed to work fully in the browser without accounts or a backend.
