# Paisley RFC Playbook 2026/27

Interactive play animator for the 26/27 season, plus the written playbook it was built from.

## Open it

Single file, no install: open `index.html` on any phone or laptop. If GitHub Pages is switched on for this repo it will be live at `https://paisleyrfc-sc.github.io/Playbook2.0/`.

Pick a section, pick a call, and it runs. Scrub the timeline, slow it to ½ or ¼ speed, or tap any step in the list to jump to that moment.

## What's in it

| Section | Contents |
|---|---|
| Game plan | Attack zones (red / amber / green), Arrowheads, ABCD at the ruck, kick calls & comms |
| Playbook | The written playbook, page by page, with PDF and Word downloads |
| Forwards | Punch, Jab, Escape (both versions), Reload, 10 call, Chaos, Ronnie Ball |
| Back row | Yellow, Black 1, Black 2 — full 8 v 8 scrums |
| Backs | Polo, Munster, Spencer, Strike, Exeter, Munster Wedge, Wiper, Wedge, Frank, Carter, Stevie, Accies, Wasps, Bath, Back Door, 10 call |
| Taranaki | Set-up, A1–A4, B1–B5 |
| Kicking | Apple, Pear, Orange, Red-zone exit, Paisley Kick chase shape |
| Lineout | Codes, set-ups (7/6/5/4/3), South Africa, Sweenie Ball, Drive Ball, Switch Ball, defending a lineout |
| Kick-off | Our kick-off, receiving |
| Defence | Numbering up, Press (zoom-paddle-zoom), set-up, principles, counter attack |

## Reading the animation

- **Blue** is us, **red** is them. The **amber ball** leaves a solid line showing where it has been.
- **Dotted blue** lines are running lines. **Dashed amber** lines are decoy runs — the man is there to draw defenders, not to get the ball.
- A solid **amber arrow** marked MISS is a miss pass; the man it goes past is the one being skipped.
- Defenders are not scripted: they read the runners in front of them, get committed by decoys, and come up or drift depending on the play. The ball carrier picks his hole once he has the ball. So the same call can finish slightly differently from the paper diagram — that is the point.
- **Amber notes** on a card mean the written playbook could be read two ways, or names something it does not describe. Settle those with the coach before drilling.

## Known gaps

- **LION / LIONS** is called in the game plan and the kick-off receive but never described in the playbook.
- The second tryline lineout code **H: 1 356 748** is listed with nothing after it.
- Wasps: "8 attacks 12 inside shoulder" — drawn as their 12; if it means ours, 8's line changes.
- Kick chase personnel are not named in the book; the animator's choices are illustrative.

## Changing a play

Everything is in `index.html`. Each play is one object in the `PLAYS` array: a list of `players` with starting positions (metres across × metres up the pitch) and a list of `actions` — `run`, `pass`, `kick`, `dummy`, `lift`, `mark` — each with a start time `t` and duration `d` in seconds. Edit the numbers, reload the page.

## Source

`playbook/` holds the written playbook as given (Word and PDF) and the page images shown in the Playbook tab. The animator is an interpretation of it, not a replacement for it — where they disagree, the book wins.
