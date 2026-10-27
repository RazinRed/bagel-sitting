# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users
Cat sitters looking after Bagel while her owners are away. A mix of first-timers reading the guide cold and regulars (friends, family) doing several visits in a row. They open the link from the group chat on their phone and use it in the flat, one-handed, often while holding a bowl, can or scoop. Visits happen at any time of day, so the page is read in daylight and in a dim flat at night.

## Product Purpose
Get a sitter through one complete, correct visit without having to message the owners: arrive without letting Bagel out or startling her, prepare and serve her meal exactly, deal with litter and water, optionally play, and leave safely. Success is a sitter who never loses their place, never has to hunt for an item, and gets the meal details right first time.

## Positioning
A guide written for one specific cat and one specific flat: every step names the real object, its exact location and a photo of it. A generic pet-sitting app could not copy that.

## Operating Context
- Phone in one hand, often mid-task; glances between steps rather than reading continuously.
- Order matters: the visit runs door → bowl → fridge → kettle → food → krill oil → water → lid → serve → fountain → litter → play → treat → leave.
- Problems are reported in the owners' group chat; there is no in-page messaging.
- Progress is kept per device in the browser (localStorage key `bagel-visit-v5`), and the sitter starts a new visit by clearing it.

## Capabilities and Constraints
- Single static file (`index.html`) plus `images/`, hosted on GitHub Pages. No build step, no backend.
- Content is factual and owner-written: quantities (⅓ can, ½ pump, about 40°C), products (Kit Cat Tuna & Chicken Hearts, Absolute Holistic krill oil with the red "Hip & Joint" label, Inaba Ciao Churu, Petkit Fresh Element Solo), locations and the kettle's 功能 / 取消 button. These must not be changed or invented.
- The repo and site are public, so the photos of the home are visible to anyone with the link.

## Brand Commitments
- Warm, personal voice from the owners ("our girl", "Bagel says meow (probably)", "Thank you!").
- Bagel's real photos in `images/`.
- Cutesy and pink (owner-pinned in the redesign round). Any direction must render cute and pink-led; clarity still wins over decoration.

## Evidence on Hand
Photos: `face.jpg`, `sit.jpg`, `yawn.jpg`, `cat.jpg` (Bagel); `supplies.jpg`, `kettle.jpg`, `krill.jpg`, `feeder.jpg`, `churu.jpg`, `bowl.jpg`, `sofa.jpg`, `treat.jpg` (blurry; owners know). There is no photo of the litter box, the fridge or the water fountain on its own, and none should be fabricated.

## Product Principles
1. One step at a time: the sitter always knows exactly where they are and what comes next.
2. Show, then tell: wherever a photo exists, it sits next to the step that needs it.
3. Exact details are unmissable: quantities, temperatures and the right bottle stand out at a glance.
4. Safety first and last: the door warning is impossible to miss on arrival and on leaving.
5. Calm about the normal stuff: hiding, not eating and not playing are reassured, not alarmed.

## Accessibility & Inclusion
Readable one-handed at arm's length, in bright and dim light: large tap targets, high contrast in both themes, no reliance on hover.
