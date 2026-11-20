# Class Tempo v2.12 — Narrow Mode Mini-Games

Complete replacement `index.html` based on the published November 18, 2026 Class Tempo source (GitHub blob `3cbdf4873c305c0bd1d9a4746bc6bd35749f487d`). Existing school schedules, shared school profile, timers, scenes, themes and browser-storage keys are retained.

## Install

Replace `index.html` in the Class Tempo repository with the included file. No other runtime files, packages, accounts or external downloads are required. Keep other repository files unchanged. This README documents the update; it is optional to upload.

## Use

1. Choose Narrow (or Auto at a narrow window width).
2. Check **Enable mini-games** on the timer stage. It is off for a new browser profile.
3. Select Snake, Checkers or Chess. Uncheck the option to restore the ordinary narrow layout; wide mode is unaffected.
4. The activity timer moves immediately below the main countdown when mini-games are enabled. If it is running, its countdown also appears in the game panel. The main timer is mirrored there too.

### Snake

Automatic play seeks randomly placed, weighted fruit using a grid path search. Click the canvas or Play Snake to begin manually. Arrow keys, WASD and the small onscreen arrows work. The game records a high score locally. A collision, Escape, Stop, change of class period, tab becoming hidden or 15 seconds without movement input ends manual play and resets to automatic play. Reduced motion pauses automatic animation. Fruit: apple 10; banana/orange 15; strawberry 20; grapes 25; watermelon 30; pineapple 40; rare golden star 100. Manual play speeds up slightly as score increases.

### Checkers and chess

Choose Computer or Two players (same device). The computer is a lightweight casual opponent; no online play or difficulty ladder. Checkers uses mandatory captures, chained jumps and kings. Chess supports legal move highlighting, check, checkmate, castling, en passant and promotion. The casual chess implementation automatically declares a draw at three repeated positions or 50 moves without a pawn move or capture rather than requiring a formal claim. Changing games, turning the feature off or leaving the page preserves the two board positions in browser storage. New game asks for confirmation.

School mode pauses mini-games when outside an active class, lunch or arrival period. A completed manual countdown also pauses them. The two timers remain independent of all game state. Both games and preferences stay on this browser; no network services are used. Contrast switches board squares to more opaque colors for readability.

## Verification

Chromium smoke tests at a 410px viewport with an in-memory storage test double: enabled/disabled, Snake input, chess and checkers CPU turns, saved board across game switches, running activity timer, relocated timer, and restoring the original placement. JavaScript syntax validation passed. Chess initial move-tree counts 20/400/8902, checkmate, en passant and castling verified; checkers forced chained capture verified. Actual Chromebook performance and long-term browser-storage behavior should be checked after deployment.
