# Riemann Hypothesis, live

An interactive page that shows what the Riemann Hypothesis says, with everything computed in your browser.

**Live:** https://andreysuperiorgit.github.io/riemann/

- **The landscape.** |ζ(s)| over the critical strip, drawn as blocks. Where the blocks drop to the floor there is a zero, marked with a red pin. Drag to rotate.
- **The spiral.** The curve ζ(½ + it). It passes through 0 at every zero.
- **The primes.** Riemann's explicit formula for ψ(x). Add the zeros one by one and the curve turns into the staircase of primes and prime powers.

## What the page checks

- It finds the first 102 zeros on the line Re(s) = ½ (up to t = 240) from sign changes of Z(t). The first five: 14.134725, 21.022040, 25.010858, 30.424876, 32.935062.
- It counts every zero in the whole strip up to t = 240 with the argument principle and gets 102. The two numbers match, so in that range no zero is off the line.

This page shows the statement. It is not the proof. The proof was announced on Nov 20, 2026 by Levent Alpöge (Anthropic), found working with Claude, and certified by the Lean and Mathlib communities on Nov 21, 2026.

## How it was built

One HTML file, no libraries, no build step. ζ(s) by Euler-Maclaurin summation, canvas 2D for all drawing.
Written with Claude Code: the final page with Fable 5.2, the first version of the math core with Opus 5.5. The model also opened the page in headless Chrome, took screenshots and fixed what looked wrong over several rounds.

## Run it locally

Open `index.html` in a browser.
