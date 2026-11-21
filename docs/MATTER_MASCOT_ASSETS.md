# Matter mascot assets

The full sprite atlas is `assets/pets/matter/Matter-spritesheet.png`. It uses the Work v2 layout, 1536 × 2288 pixels, with 192 × 208 pixel cells, eight columns, eleven rows, and transparent unused cells.

Individual animation rows are in the same directory. `Matter-manifest.json` records each state, frame count, and look direction order. `README-Matter.txt` summarizes the package.

| Row | File | Frames | State |
|---:|---|---:|---|
| 0 | `Matter-idle.png` | 6 | Idle |
| 1 | `Matter-running-right.png` | 8 | Right movement |
| 2 | `Matter-running-left.png` | 8 | Left movement |
| 3 | `Matter-waving.png` | 4 | Greeting |
| 4 | `Matter-jumping.png` | 5 | Jump |
| 5 | `Matter-failed.png` | 8 | Failed or blocked |
| 6 | `Matter-waiting.png` | 6 | Waiting for input |
| 7 | `Matter-running.png` | 6 | Active work |
| 8 | `Matter-review.png` | 6 | Review |
| 9 | `Matter-look-directions-000-157.png` | 8 | 000° to 157.5° |
| 10 | `Matter-look-directions-180-337.png` | 8 | 180° to 337.5° |

The atlas passed the ChatGPT Work structural sprite-sheet validator. Direction poses are subtle and may need a later art pass.

Créditos:
Hecho por Lournyx Matterssmith [Lou-Nyx].
