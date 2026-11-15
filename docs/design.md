# Pip's Great Expectations — design

Small 2D platform game for an English class presentation on Dickens' *Great Expectations*.
Played by classmates on iPhone/Android (landscape) via a link/QR code; also works on PC.

## Decisions
- Single file `index.html`, HTML canvas, no libraries, no external assets (pixel art drawn in code). Works offline once loaded.
- Controls: floating mini joystick (left thumb) + jump (right thumb). Keyboard: arrows/WASD + Space.
- Text is all in English. ~5 minutes total, 5 levels of ~1 minute, replayable at home.
- Ending is fixed and happy: Pip understands how much Joe mattered, meets Estella again.

## Levels (one per key moment of the book)
1. The Marsh: bring bread to the convict (brambles, crows).
2. Satis House: rotting floor, cobwebs, rats; Estella's scorn; the stopped clock.
3. London: coins (pride) slow Pip down, hearts (kindness) lighten him.
4. The Truth: benefactor is Magwitch; escape along the Thames.
5. Home: Joe, then Estella in the ruins of Satis House. Happy ending.

After each level: one multiple-choice question in English (+50 points, with explanation if wrong).
Score = hearts, coins, items, stomps, quiz answers, minus falls. Best score saved on the phone.

## Testing
Headless browser at phone size: screenshots plus a simple bot that plays each level to check it can be completed.
