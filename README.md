# Perennial

**One tree is shade in summer, food in fall and fire in winter.**

A Four Seasons game for the ThunderHacks 2026 Algoma Game Jam.

![Title](screenshots/title.png)

## Run it

Open `index.html` in any modern browser (Chrome, Edge, Firefox, Safari). That is the whole game: one file, no install, no server, no internet connection needed. Click the window once if the keyboard doesn't respond.

For the judging table: open it full screen (F11), keep the volume up, and let the judge press **Enter**.

## How to play

| Key (remappable) | Does |
|---|---|
| WASD or arrow keys | Move |
| Space or E | Act: plant, fill bucket, water, chop, feed the fire |
| Q or F | Eat a fruit (heals) |
| Esc or P | Pause (the pause screen explains every season in pictures) |

Gamepad (stick or d-pad, A act, X eat, Start pause) and touch (drag to move, buttons on the right) also work.

Walk over seeds, fruit and wood to pick them up. Survive **3 winters** to win; after that you can keep going in endless mode. Your score is counted in tree rings.

## The four seasons change the rules

| Season | What changes | Your job | Danger |
|---|---|---|---|
| **Spring** (rain) | Soil is soft. Seeds can only be planted now. The pond is full. | Plant seeds in the soil plots. | Rabbits come to eat your sprouts. Chase them off. |
| **Summer** (heat) | The sun hurts you outside of shade. The pond shrinks. Sprouts dry out. | Carry water from the pond to your sprouts. Rest in tree shade or on the porch. | Heat stroke. Sprouts that dry out wither. |
| **Fall** (wind) | Sprouts that survived become trees. Trees drop fruit, seeds and branches. Wind pushes you and blows loose fruit away. | Gather fruit (basket holds 6) and wood (arms hold 6). Collect seeds for next spring. Stock the fire. | Fruit left on the ground rots when winter comes. |
| **Winter** (snow, night) | It's dark and you move slowly through snow. The fire burns fuel fast. Hunger is sharp. The pond freezes over (slippery). | Keep the hearth burning. Eat. Venture into the dark for deadwood, or chop one of your own trees. | Cold away from the fire light. Wolves in the dark. Standing on the ice when spring thaws drops you in. |

### The stray dog

A few seconds into summer, a stray dog wanders into the meadow. Walk up to it and press the act key to adopt it. A dashed outline then appears beside the cabin: drop **4 wood** there to build the dog a house. That wood is the same wood you need for the winter fire.

Once adopted, the dog helps you in every season:

- **Spring:** it chases rabbits away from your sprouts.
- **Summer:** now and then it digs up a stick.
- **Fall:** it fetches fruit from anywhere on the map, but only while your basket has room.
- **Winter:** with a house, it walks with you into the dark and barks wolves away. Without a house, it shivers by the fire and can't help.

The dog and the rabbits walk around the pond, never through it. A rabbit going after your sprouts shows a red **!!** bubble.

If you don't adopt it by the end of summer, it leaves, and it comes back next summer. Press the act key beside your dog when there's nothing else to do, and you'll pet it.

![The dog and its house](screenshots/dog.png)

### The one idea

Every tree you plant is a choice that carries across the whole year and into the next:

- In **summer** it is shade, the only shelter from the sun besides the porch.
- In **fall** it drops fruit, seeds for next year, and branches.
- In **winter** it can be chopped for 2 or 3 logs of firewood, but then it is gone forever: no more shade, fruit or seeds.

So the player plans a cycle: plant more in spring to have more shade, food and fuel later, and decide in the dark of winter whether to burn the future to survive tonight.

### Season changes are part of the play

- The season wheel (top left) and the countdown (top right) show what's coming next.
- The last 3 seconds of every season tick audibly.
- **Spring to summer:** sprouts start needing water.
- **Summer to fall:** surviving sprouts become trees; dried-out ones stay dead.
- **Fall to winter:** fruit left on the ground rots. Dusk falls during the last seconds of fall.
- **Winter to spring:** the ice visibly cracks in the last 5 seconds; anyone still on it falls through.
- Each new year is harder (hotter summers, colder and hungrier winters, more rabbits and wolves).

## Accessibility (Options menu)

- **Remappable controls** for every action (two keys per action; the second is a fixed alternative).
- **Colour-blind palette** (Okabe-Ito colours; fruit changes from red to outlined orange so it never relies on red versus green, health turns blue).
- **Difficulty:** Gentle, Normal, Hard (season length, heat, cold, hunger, wolves, fruit yield, fire burn).
- **Picture hints:** first year only, always, or off.
- **Reduce motion:** turns off screen shake, bobbing and most particles. It's on by default if the OS asks for reduced motion.
- Separate music and sound effect volume.
- Auto-pauses when the window loses focus.
- Settings are saved in the browser.

## Teaching without text

The first year is the tutorial, and it uses no instruction text:

- Movement keycaps appear under the character until you move.
- Picture bubbles point at the next useful thing (seed, then plot; bucket, then pond; sun, then shade; wood, then fire).
- An arrow by the character points to whatever the bubble is on.
- A context bubble with the act key appears over anything you can use right now. A crossed-out sprout shows that seeds can't be planted out of season.
- Each season opens with a banner of two picture rules, such as `seed → sprout` and `rabbit ✕`.
- The pause screen shows all four seasons as picture rules.

## Art and audio (made during the event)

- **Art:** every shape is drawn in code on an HTML5 canvas in one flat "paper diorama" style. Each season uses the same shapes with its own palette, and colours cross-fade when the season turns.
- **Music:** generated live with the Web Audio API. Each season has its own key, tempo and instrument: plucked major pentatonic for spring, slow lydian pads for summer, dorian reeds for fall, sparse minor bells for winter.
- **Ambience and sound effects:** synthesized from noise and oscillators, including rain, cicadas, wind gusts, a winter howl, chopping, splashing, fire crackle, rabbit squeaks, wolf howls and ice cracks.

## Third-party assets, tools and libraries

**None in the game.** No engine, framework, library, image, sound or font file is used. Text uses the computer's own system font.

Tools used to make it: a text editor, a web browser, and Playwright with headless Chromium for automated playtesting (not part of the game). The game was written with help from Claude, an AI assistant by Anthropic. Check whether the jam rules ask you to declare AI assistance, and say so if they do.

## Files

- `index.html`: the complete game
- `screenshots/`: one screenshot per season, plus the title screen
- `PITCH.md`: a 5-minute pitch script and likely judge questions
- `SUBMISSION.md`: the deliverables checklist mapped to the brief and rubric
