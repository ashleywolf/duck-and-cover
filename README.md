# :duck: Duck & Cover

Physically duck below your webcam to dodge. Pop back up and yell to shoot. You are a prairie dog with a gun and no fear.

## [Play Now](https://ashleywolf.github.io/duck-and-cover/) (Chrome/Edge)

## What Is This

The most physical game in the collection. MediaPipe tracks your body pose through the webcam while Web Audio listens for volume spikes. Objects fly at you on screen. Duck your actual body to dodge them, then pop up and yell to fire back. An animated prairie dog mirrors your every move.

## Features

- Pose tracking via 33 body keypoints with nose Y position driving duck detection
- Dynamic duck calibration from your standing baseline (works at any height)
- Animated prairie dog character that mirrors your ducking and opens its mouth when you shoot
- Muzzle flash on the prairie dog when you fire
- Volume-based yell detection for shooting, plus spacebar fallback if you can't make noise
- 280px volume meter so you can see your yell intensity
- "BANG!" feedback on successful shots, "SO CLOSE!" on near-misses
- Combo milestones: x5 gold burst, x10 fanfare, x15+ rainbow "UNSTOPPABLE!" display
- localStorage high scores

## How to Play

- Stand in front of your webcam with some room to move.
- Objects fly toward you. Duck your body below the camera to dodge.
- Pop back up and yell (or press spacebar) to shoot.
- Rocks must be dodged. Targets can be shot. Bombs must be shot before they hit.
- Chain dodges and shots for combo multipliers.

## Tech

- MediaPipe PoseLandmarker tracking 33 body keypoints (nose Y drives duck state)
- Web Audio API with real-time volume analysis for yell/shout detection
- Dynamic baseline calibration so duck thresholds adapt to your setup
- HTML5 Canvas with sprite animation for the prairie dog character

## Browser Support

Chrome or Edge recommended. Requires both webcam and microphone access. You need enough room to physically duck, so laptop-on-desk or standing at a monitor both work.

## Part of Browser Party Games

8 single-file browser games built with MediaPipe, Transformers.js, Web Audio, and Web Speech. No servers, no build steps, no installs.

| Game | Input | Tech |
|------|-------|------|
| [Type or Die](https://ashleywolf.github.io/type-or-die/) | Keyboard | Vanilla JS |
| [Grin Sweeper](https://ashleywolf.github.io/grin-sweeper/) | Smile (webcam) | MediaPipe Face |
| [Show & Tell](https://ashleywolf.github.io/show-and-tell/) | Real objects (webcam) | Transformers.js DETR |
| [Pitch Climber](https://ashleywolf.github.io/pitch-climber/) | Voice pitch (mic) | Web Audio API |
| [Spell Caster](https://ashleywolf.github.io/spell-caster/) | Shout spells (mic) | Web Speech API |
| [Stone Face](https://ashleywolf.github.io/stone-face/) | Don't react (webcam) | MediaPipe Face |
| [Ninja Hands](https://ashleywolf.github.io/ninja-hands/) | Hand tracking (webcam) | MediaPipe Hands |
| [Duck & Cover](https://ashleywolf.github.io/duck-and-cover/) | Duck + yell (webcam+mic) | MediaPipe Pose + Web Audio |

---
Built with vanilla JS + browser ML. Each game is one HTML file. Fork it, break it, make it yours.
