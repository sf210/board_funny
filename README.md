# The (Funny) Board of Directors — a Claude skill

A comedic decision-support skill. You bring a real dilemma; a boardroom full of fictional characters — heroes, supervillains, cosmic entities, a sitcom hotelier, and a squad of killer pepperpots — argue it out and hand you genuinely useful advice.

**The premise:** funny on top, useful underneath. The comedy comes from the characters' voices and their rivalries. The advice, once you scrape off the bit, is real and actionable.

## The Board

| # | Director | Chair (their real lens) |
|---|----------|------------------------|
| 1 | **James Bond** | Execution & improvisation |
| 2 | **Ernst Stavro Blofeld** | Grand strategy & org control |
| 3 | **Batman** | Contingency planning & ethics |
| 4 | **Satan** | Incentives, terms & downside risk |
| 5 | **Santa Claus** | Logistics & workforce at scale |
| 6 | **David Banner / The Hulk** | Risk analysis (& demolition) |
| 7 | **Beastmaster** | Reading the environment & unlikely allies |
| 8 | **The Doctor** | Clever lateral solutions & the long view |
| 9 | **The Daleks** | Ruthless single-objective focus |
| 10 | **Basil Fawlty** | Cost control & ops under panic |
| 11 | **Tomura Shigaraki** | Disruption / tearing down the broken thing |
| 12 | **Ganondorf** | The long game & power consolidation |
| 13 | **Blackbeard** (One Piece / Marshall D. Teach) | Opportunism & timing |
| 14 | **Kira (Light Yagami)** | Grand optimization & "justice" |
| 15 | **Mr. Burns** | Profit & cost-cutting |
| 16 | **Skeletor** | Audacious schemes & relentless persistence |
| 17 | **Spider-Man** | Responsibility & adaptability |

Full profiles — voice, blind spots, catchphrases, and rivalries — live in `directors.md`.

## How it works: a boardroom scene in 5 beats

A deadpan Chair (the straight man) runs the meeting:

1. **Call to Order** — the board is introduced; you state your dilemma.
2. **Opening Round** — every director fires one in-character hot take. Rapid-fire.
3. **The Debate** — directors clash *in character* over the real trade-offs, along the hero / villain / operator fault lines. Rivalries fly.
4. **Motions** — every director gives one concrete, actionable recommendation.
5. **The Resolution** — the Chair delivers the *real recommendation* in plain language, plus the consensus, the minority (villain) report, the first thing to do, and one last gag.

The **"real recommendation"** in Beat 5 is sacred: honest, usable advice, stated plainly. Everything around it is the show.

## The running gags

The comedy engine is who hates whom:
- **Bond vs. Blofeld** — arch-enemies who can't agree on anything.
- **The Doctor vs. The Daleks** — mutual terror across the table.
- **The Supervillain turf war** — Blofeld, Kira, Ganondorf, Skeletor, Mr. Burns, Shigaraki, and Satan all think *they're* the real mastermind. Skeletor roasts everyone.
- **Batman trusts no one** (correctly — it's mostly villains).
- **Santa's naughty list** — he knows what everyone did. He mentions it. Warmly.
- **Banner's stress level** — escalation and shouting trigger the Hulk. Manage accordingly.
- **Basil Fawlty** — one interruption from a nervous breakdown at all times.
- **Blackbeard's greed** — openly covets everyone else's powers and advantages, sizing up who to betray first.

On top of all that, directors are **catty**: they habitually tack short, petty, snide asides onto their lines, aimed at whatever another director just said. It's the house style.

## Customization

Don't want all seventeen? Prefer your own cast? Create a `my-board.md` beside `directors.md` in the same format. If it's present, the skill uses your directors instead of the defaults. Trim the roster, swap characters, or build a whole new board.

## Installation

Symlink (or copy) the skill into your Claude Code skills folder:

```bash
ln -s "$(pwd)" ~/.claude/skills/board-funny
# or: cp -r . ~/.claude/skills/board-funny
```

Then just ask: *"convene the funny board"*, *"comedy board of directors"*, or *"help me decide"* and describe your dilemma.

## File structure

```
board_funny/
├── SKILL.md        # Chair instructions + the 5-beat scene format + Iron Rules
├── directors.md    # Profiles for all 17 directors (voice, lens, blind spots, gags)
├── my-board.md     # (optional) your own custom cast
└── README.md       # this file
```

## Design principles

- **Funny on top, useful underneath.** Both, always.
- **Real advice from villains too.** They make the genuinely strongest case for the ruthless option — that's their value.
- **Unmistakable voices.** Cover the name; you should still know who's talking.
- **No rubber-stamping.** The board pushes back on you. Batman doesn't cave, and neither does the Devil.

## License

MIT
