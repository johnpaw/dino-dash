# Dino-dash
Dino Dash is a retro-styled infinite runner game that pays homage to classic handheld console aesthetics. Players control a running dinosaur traversing a desert landscape, aiming to achieve the highest score possible by dodging obstacles and surviving as speed increases.

# Visual & Audio Style
- Aesthetic: The game utilizes a classic 4-color "Game Boy" palette, featuring shades of olive and dark green (#9bbc0f, #8bac0f, #306230, #0f380f).
- Typography: Uses the 'Press Start 2P' font for a nostalgic, pixel-art feel.
- Background: Features a dynamic parallax scrolling system with multiple layers of random, procedurally generated mountains that move at different speeds to create depth.
- Audio: Synthesized retro sound effects powered by Tone.js:
  - Jump: A sharp square-wave beep.
  - Level Up: A soft two-note chime.
  - Collision: A white-noise crash.

# Gameplay Mechanics

Objective: 
- Run endlessly to accumulate a high score. The score increases with distance traveled.

Obstacles:
- Cacti: Ground-based obstacles of varying heights and widths.
- Birds: Flying enemies with animated wings (bat-like shape) that appear at variable heights, requiring the player to duck or jump depending on their altitude.

Progression:
- Speed: The game speed starts at a base level and increases incrementally every time the player passes a score threshold (every 30 points).
- Levels: A level counter tracks difficulty progression.
- Physics: Includes variable jump height mechanics—holding the jump button results in a higher jump, while a quick tap results in a shorter hop ("jump cut").

# Controls
- Desktop
  - Jump: Up Arrow, Spacebar, or Left Click (on the left side of the screen).
  - Duck: Down Arrow or D Key.
  - Debug: H key toggles hitbox visibility.

- Mobile / Touch
  - Jump: Tap the Left side of the screen.
  - Duck: Tap the Right side of the screen.

# Technical Details
- Storage: High scores are persisted locally in the browser (localStorage).
- Engine: Custom HTML5 Canvas rendering loop requesting animation frames for smooth performance.
- Responsiveness: The game container maintains a fixed aspect ratio (800:300) but scales to fit different screen sizes.
