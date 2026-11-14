# The temporal volume — Module XIV

Standalone interactive extract of Module XIV, "The temporal volume", from the Chronowave Dynamics Temporal Engine: a single-file compendium of 17 interactive modules about the author's temporal framework. The full compendium, its manual and its edit log are in [chronowave-compendium](https://github.com/Ajuntanaga/chronowave-compendium). The module's own heading on the page reads: "Inside the cube: t&#179; made literal".

## Use it

Download or clone this repository, then open [`Module_XIV_Temporal_Volume.html`](Module_XIV_Temporal_Volume.html) from disk in a current browser (GitHub only shows its source). There is no build step and nothing to install. Math (KaTeX 0.16.9) and fonts load from cdnjs and Google Fonts, so equations and typography need a connection.

## Files

| File | What it is |
|---|---|
| [`Module_XIV_Temporal_Volume.html`](Module_XIV_Temporal_Volume.html) | The module: one page with the shared styles, this module's section and the script statements it needs. |
| [`Module_XIV_Manual.md`](Module_XIV_Manual.md) | This module's part of the compendium's plain-text manual (extracted from rev b90 and hand-patched, so it may lag the page). |

The other two files are this README and a `.gitignore`.

## Where it comes from

Made on 2026-11-14 from rev b91 of the compendium page (commit `6cf22d4` of chronowave-compendium) by the scripts in the `tools/split` folder of that repository (added in later commits). The section markup, the styles and the script statements are copied from the page without change. What differs is the page title and description, a short header and footer line and small stand-ins for the parts of other modules that this module reads (see the limits below).

## Checks and limits

- A scripted headless-Chromium test loaded the page, moved every slider, select and checkbox, clicked every button and sent pointer, wheel and key events to every canvas: 86 actions (slider moves, clicks, and pointer, wheel and key events), 1 canvas, no uncaught exception and no console error. It is a smoke test: this extract was not compared with the original module for identical behaviour, and nothing here has had an independent review.
- The rotatable cube, the three frequency sliders, the phase and threshold sliders, the field and view buttons and the live "volume this cube stands for" readout (V_T, the aspect ratio and the eq (6) normaliser A) are this module's own and work here.
- The "Lattice" chip sets the three frequency ratios from the lattice of Module IV; here the lattice is fixed at its start-up state (the identity scale, root 261.63 Hz, equal temperament), so it always fills in 1.122, 1.189 and 1.260 (read from the code).
- The "Lorenz drive" chip needs Module XII: here the attractor's x is fixed at 0, so switching it on only slows the phase animation to a quarter, with no attractor term. The "Scramble damping" chip needs Module V: the damping factor is fixed at 1, so it changes nothing visible.
- The frame choice made with the dimension buttons of Module I is not available, so the frame note beside the volume readout never appears.
- The framework is the author's own and still in progress; Module XVII of the compendium (also a repository of its own, [chronowave-verdicts-and-rulings](https://github.com/Ajuntanaga/chronowave-verdicts-and-rulings)) carries the page's own verdicts and open rulings.
- No license: all rights are reserved by default, beyond viewing and forking on GitHub; a license is the author's decision.
