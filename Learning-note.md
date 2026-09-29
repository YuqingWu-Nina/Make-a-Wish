# Learning Notes

## 1. Idea and scope

I chose **Make a Wish!** as a small, playful birthday-cake maker. I wanted the main interaction to feel like preparing a digital surprise, not like building a complicated design tool. To keep the project realistic for a beginner, I used one `index.html` file and did not include accounts, a backend, or external services.

I created `README.md`, this learning note, and `Design.md` so I could track the idea, the decisions I made, and what I learned while building the project.

## 2. First build

The first complete interaction included a cake, one local image upload, a birthday message, candles, confetti, and a reset button. The uploaded image uses `URL.createObjectURL()`, so it appears only in the current browser and is not sent to a server.

I used Codex as a coding partner while I built this first version. I described what I wanted the user to see and do, then used the generated code as something to read and question. The comments in the JavaScript helped me connect an input to an output: for example, clicking the wish button is the input, while turning off the candle flames, showing the message, and starting confetti are the outputs. This made the code feel less like separate technical pieces and more like a sequence of instructions for the browser.

## 3. Testing and revision

I added cake, cream, and topping choices, plus six fixed cake-pick spots. I chose fixed positions instead of drag-and-drop because they made the interaction easier to understand and reduced the risk of building a harder system before the basic experience was working.

During revision, I noticed that the wooden sticks could disappear or look as though they sat on top of the cream. I learned that this was a visual-layering problem: the stick and topper artwork were not arranged in the right order. I asked Codex to help separate the sticks from the clickable topper artwork, then checked that the cream could cover the lower part of each stick. This helped me understand how CSS `z-index` and stacking order can change what an object looks like without changing its basic function.

I also tightened the topper positions into a centered back row and front row. The number pick remains the highest focal point, while the other picks create a smaller celebratory cluster around it. This revision taught me that interaction design includes visual arrangement: the buttons still needed to be clickable, but the group also needed to look intentional.

## 4. Visual refinement

The first topper arrangement was too wide and did not feel like one celebration. I simplified the balloon into a taller CSS cluster and changed the party character into one clear cat emoji because the earlier versions were visually awkward. I kept the lighter emoji-style cake after trying a more realistic texture direction because it better matched the playful tone I wanted.

Codex was helpful for trying focused changes, but I had to decide whether a result actually matched my idea. I learned to give more precise instructions when something looked wrong, such as saying that the candles should remain visible, that the background should stay behind the cake, or that a decoration should not block another control. This made the revisions more useful than only asking for something to look “better.”

I also refined the preview stage with a soft party-room background. The bunting, edge balloons, dots, sparkles, and glow are made with CSS and stay behind the cake. This helped me see that CSS can create atmosphere with shapes, gradients, and layers rather than only changing colors or font sizes.

## 5. Current limitations and next steps

I wanted a finished cake to be shareable, but a real sharing service would need a backend to save the cake and image. Instead of claiming the project could do that, I made a front-end-only **mock recipient preview**. The URL stores preset settings and the birthday message, then opens a darker recipient view with lit candles. The recipient can select **Blow Out the Candles** to brighten the scene, show confetti, and reveal the message.

Uploaded photos stay local and are deliberately excluded from the mock URL because they cannot be safely or reliably shared without storage. This decision helped me understand the difference between a visual front-end prototype and a real online service. Codex helped explain possible technical approaches, but I chose the mock flow because it is honest about what this project can do.

Next, I would like to ask classmates to try the interaction, review the page for accessibility issues such as keyboard navigation and color contrast, and publish a hosted version. If I later build real sharing, I would first need to plan secure storage and privacy for uploaded images.
