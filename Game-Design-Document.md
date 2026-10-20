# Lantern Loop — One-Page Game Design Document

**Genre:** Small top-down arcade survival / collection game  
**Platform:** Browser (desktop and mobile)  
**Audience:** Casual players and beginners; suitable for a 3–5 minute play session  
**Player fantasy:** You are a tiny lantern bringing light back to a dark garden.

## Goal
Collect **10 glowing fireflies** before the 60-second timer expires, while avoiding shadow moths.

## Core mechanic and loop
**Move → approach a firefly → collect it and see the score increase → dodge moths → decide which firefly to pursue next.**  
This is the single core action: movement and positioning. The score, glow, lives, and timer provide immediate feedback.

## Rules
- The player moves in four directions and stays inside the play area.
- Touching a firefly adds one to the score; a new firefly appears elsewhere.
- Shadow moths chase the player. Touching a moth costs one life and grants a short invulnerability window.
- The player starts with 3 lives and 60 seconds.
- **Win:** collect 10 fireflies. **Lose:** timer reaches zero or lives reach zero.
- Start/Restart begins a fresh run. Pause freezes play.

## Controls
- **Keyboard:** WASD or arrow keys to move; Space to pause.
- **Touch:** directional buttons below the game canvas.
- **UI:** Start / Restart and Pause buttons.

## Feedback states
1. **Onboarding / ready:** “GUIDE THE LIGHT” overlay explains the goal and start action.
2. **Playing:** score, time, and lives remain visible; fireflies glow and moths are pink.
3. **Damage:** life counter drops; brief blinking indicates temporary protection.
4. **Paused:** dark overlay with “PAUSED”.
5. **Win:** “LIGHT RESTORED!” and a restart instruction.
6. **Loss:** “THE NIGHT WON” and a restart instruction.

## Scope cuts
No levels, inventory, story dialogue, sound, online leaderboard, account, monetization, or external art assets. Shapes and canvas effects are placeholder art to keep the prototype self-contained and easy to run.

## Testable success criteria
- A first-time player can state the goal after reading the opening screen.
- Movement works with keyboard and touch.
- Collecting a firefly increases the score by one.
- Moth collision reduces lives, and win/loss/restart states work.
- A complete attempt takes no more than 60 seconds, with a target play session of 3–5 minutes including retries.
