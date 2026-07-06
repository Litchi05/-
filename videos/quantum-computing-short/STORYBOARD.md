---
format: 1080x1920
message: "Quantum computers don't think in 0 OR 1 — they think in both at once, and that changes everything."
arc: concept-explainer
audience: general YouTube Shorts viewers — curious, zero physics background, 1-second attention window
music: dark pulsing electronic, tense and driving, builds to a confident drop
---

## Video direction

- palette system: from `frame.md` (broadside) — ink-black ground for every frame (the two-register system stays dark-register throughout; fire-orange appears only as the scarce voltage: one emphasized word, one counter, one underline per frame). cream = primary type ink; cream-muted/cream-hint = secondary + chrome; fire-orange = the single accent, never two accents in one scene. Frame 5 may cool the ambient toward a frost-blue *tint of the ground only* (a low-opacity overlay wash), type stays cream/orange.
- motion grammar: smooth long-tail settles (`power3`) everywhere; zero bounce/overshoot. Every frame reveals sequentially on its VO cues — at t=0 only the words being spoken enter; each further line/tile/number waits for its spoken cue, with reveals spread into the back ~50%. During holds: stillness, at most subtle jitter (`sine-wave-loop`, low amplitude). No lazy breathing, no back-half pan/push.
- portrait discipline: 1080x1920; stacked layouts only (no side-by-side triptychs); centered heroes anchor at y ≈ 806 (0.42 × height); all primary content in the top ~83% — bottom ~17% is the caption band keep-out. Type runs huge, few words per line (Barlow 900 lowercase per frame.md).
- rhythm / held frames: Frames 1–4 ride escalating reveal energy; Frame 5 opens with a deliberate held beat ("the catch?" alone, still, one full breath) before the glitch turn — the video's one planned stillness; Frame 6 is calm and resolved, long hold on the final line.
- negative list: no purple-blue "AI gradient" bokeh; no browser chrome / UI mocks (nothing here is an interface); no slideshow failure (front-load-then-freeze) and no screensaver failure (everything floating independently); no `repeat`/`yoyo`, no randomness; broadside forbids soft shadows and rounded-friendly decoration — flat planes, 1px hairlines, hard geometry only.

## Frame 1 — Hook

- scene: Bare ink-black canvas. Massive lowercase Barlow 900 punches in beat by beat: "your computer" / "thinks in 0s and 1s." — then the hard turn: "quantum computers think in BOTH" with "both" slamming in fire-orange, "at once." stamped beneath.
- voiceover: "Your computer thinks in zeros and ones. Quantum computers think in both — at the same time."
- duration: 5s
- transition_in: cut
- status: outline
- src: compositions/frames/01-hook.html
- type: hook
- persuasion: Counterintuitive claim
- beat: Surprise + intrigue
- blueprint: kinetic-type-beats (Reproduce)
- focal: the word "both" — the fire-orange slam that lands the counterintuitive claim
- roles: statement lines = foreground subject · "0 1 0 1" mono chrome rain-columns = background (dim ~35%, deterministic) · "at once." stamp + hairline rules = supporting
- sfx: impact-deep, tick

Reproduce: kinetic-type-beats — a statement builds across full-screen beats, each its own move, onto a spring-pop payoff (smooth settle, no overshoot).
Scene 1 (0.0–1.6s): ink-black field with faint mono "0 1" digit columns as background texture (dim, static after entrance); "your computer" then "thinks in 0s and 1s." land as two kinetic beat-slams (`kinetic-beat-slam`) — centered stack, hero type filling ~55% of width, anchored around y≈806; each line lands on its VO cue with a long-tail settle.
Scene 2 (1.6–3.4s): hard-cut word-swap (`discrete-text-sequence`) clears the first statement at the sentence seam — "quantum computers" slams in, then "think in" — the swap is the beat; layout stays centered, type scales up a step (hierarchy by size + weight).
Scene 3 (3.4–5.0s): on the spoken "both", the word "both" spring-pops (`spring-pop-entrance`, smooth settle) dead-center in fire-orange at the largest size on screen (3:1 over supporting lines); "at once." stamps beneath on its cue (`kinetic-beat-slam`); ambient glow blooms faintly behind the orange word (`ambient-glow-bloom`); hold still to the cut — subtle jitter only.

narrativeRole: Opens the cognitive gap in the first second — a machine that holds two contradictory states at once violates everything the viewer knows about computers.
keyMessage: Quantum computers break the most basic rule of computing: a value is 0 OR 1.

## Frame 2 — The spinning coin

- scene: Consistent dark stage. A flat coin marked "0 | 1" lies flat — label "a normal bit: heads OR tails." Then the coin kicks up into a spin (3D flip driven on the GSAP timeline, orange edge-glow) — label swaps to "a qubit: heads AND tails". The word "superposition" stamps in mono chrome beneath.
- voiceover: "A normal bit is a coin lying flat — heads or tails. A qubit is that coin spinning — both at once. That's superposition."
- duration: 8s
- transition_in: cut
- status: outline
- src: compositions/frames/02-spinning-coin.html
- type: product_intro
- persuasion: Analogy / metaphor + coined term
- beat: Clarity + "aha"
- blueprint: kinetic-type-beats (Adapt)
- focal: the coin — a flat disc that becomes a spinning superposition
- roles: coin disc = foreground subject (top band, ~45% of width) · labels "a normal bit / a qubit" + "heads OR tails / heads AND tails" = supporting (stacked beneath the coin) · "superposition" mono stamp = supporting payoff · hairline grid rules = background
- sfx: whoosh-soft, impact-deep

Adapt: keep kinetic-type-beats' signature (the statement swapping in place, each swap a beat) but give the beats a drawn subject — the coin diagram above the type. Vertical stack: coin in the upper third, label lines mid, coined term last. The coin's spin is a finite 3D rotationY tween sequence on the timeline (not a CSS loop), reading as "spinning" for the shot's remainder.
Scene 1 (0.0–2.6s): a flat ellipse-coin (SVG, cream stroke on ink, "0" and "1" on its halves) draws itself in (`svg-path-draw`) at y≈600 as the VO says "a coin lying flat"; label line "a normal bit" then "heads OR tails" reveal beneath on their cues (`dynamic-content-sequencing`), asymmetric stack, coin dominant.
Scene 2 (2.6–5.4s): on "spinning", the coin kicks up into a fast 3D flip (finite rotationY tween chain with `motion-blur-streak` on the kick) and a fire-orange edge-glow blooms (`ambient-glow-bloom`); the labels hard-cut word-swap (`discrete-text-sequence`): "a normal bit" → "a qubit", "heads OR tails" → "heads AND tails" — each swap exactly on its spoken word, orange lands on "AND".
Scene 3 (5.4–8.0s): on "superposition", the coined term stamps in as a full-width mono chrome bar (`kinetic-beat-slam`) under the stack; the coin's flip decelerates to a slow settle-tilt and holds; everything else still — subtle jitter at most.

narrativeRole: Names the protagonist (the qubit) and concretizes superposition with the one analogy everyone gets: a spinning coin is neither heads nor tails until it lands.
keyMessage: A qubit is a spinning coin — genuinely both states until you look.

## Frame 3 — Exponential explosion

- scene: Consistent dark stage. A count-up sequence: "1 qubit = 2 states" → "2 = 4" → "10 = 1,024" — numbers snowball, then the hero stat slams in: "300 qubits" in fire-orange over "more states than ATOMS in the universe", with a deterministic particle-scatter starfield blooming behind.
- voiceover: "Every qubit you add doubles the power. Ten qubits — a thousand states. Three hundred? More states than there are atoms in the entire universe."
- duration: 8s
- transition_in: push-slide UP
- status: outline
- src: compositions/frames/03-exponential.html
- type: social_proof
- persuasion: Statistical proof + anchoring on a familiar referent
- beat: Fascination + escalation
- blueprint: dataviz-countup (Adapt)
- focal: the escalating state-count number — a value-scaled counter that becomes the "atoms in the universe" claim
- roles: giant counter = foreground subject (center, y≈806) · "N qubits" mono ladder rail = supporting (upper band, rows accumulate) · deterministic dot starfield = background (blooms at the climax, dim ~40%) · hairline rules = supporting
- sfx: tick, riser, impact-deep

Adapt: keep dataviz-countup's signature (the count-up number as hero, camera landing on one hero metric) but replace the chart with a doubling ladder: small mono rows accumulate ("1 qubit → 2", "2 → 4", "10 → 1,024") while one giant value-scaled counter dominates center. The "camera push-through" becomes a single zoom-to-target on the final stat.
Scene 1 (0.0–2.2s): on "every qubit you add doubles", the first ladder rows reveal one per cue (`dynamic-content-sequencing`) in mono chrome, full-width strip rows upper band; the giant counter fades in at center showing "2", then doubles to "4" — value-scaled counter (`counting-dynamic-scale`), type growing with the value.
Scene 2 (2.2–4.6s): on "ten qubits — a thousand states", the ladder jumps a row ("10 → 1,024") and the hero counter races up to 1,024, scale climbing (`counting-dynamic-scale`) with tick SFX; background dots begin a sparse deterministic scatter-in (`depth-scatter-assemble`, index-derived positions).
Scene 3 (4.6–8.0s): on "three hundred?", zoom-to-target (`coordinate-target-zoom`) tightens on the counter as it hard-cuts to "300 qubits" in fire-orange (`discrete-text-sequence`); on "atoms in the entire universe" the payoff line "more states than atoms in the universe" slams beneath (`kinetic-beat-slam`) as the starfield blooms to full density behind (`depth-scatter-assemble` completing, dim); hold the read, still.

narrativeRole: Grounds the abstract claim in one staggering, verifiable number — turns "quantum is powerful" from hype into arithmetic.
keyMessage: Quantum power doubles with every qubit — 300 qubits out-count the atoms in the universe.

## Frame 4 — What it cracks

- scene: Consistent dark stage. Three labeled tiles cascade in one at a time on the VO cues — "new medicines" (molecule glyph), "new materials" (lattice glyph), "unbreakable codes" (lock glyph) — stacked vertically under a header "problems that would take supercomputers MILLIONS of years".
- voiceover: "That could crack problems supercomputers would need millions of years for. Designing new medicines. New materials. Unbreakable codes."
- duration: 8s
- transition_in: push-slide UP
- status: outline
- src: compositions/frames/04-applications.html
- type: benefit_highlight
- persuasion: Concretization + rule of three
- beat: Momentum + foresight
- blueprint: grid-card-assemble (Adapt)
- focal: the three application tiles — the vertical stack that cashes the power claim into stakes
- roles: three bordered tiles (glyph + label) = foreground subject (stacked, ~70% width each) · header lines "problems that would take supercomputers / millions of years" = supporting (top band, "millions of years" orange) · hairline frame + faint digit texture = background
- sfx: whoosh-soft, tick, tick, tick

Adapt: keep grid-card-assemble's signature (items self-assembling in a staggered cascade, then held as one array) but the grid becomes a portrait-correct vertical stack of three flat broadside tiles (1px cream hairline borders, no shadows), each entering only on its spoken cue.
Scene 1 (0.0–2.8s): header lands in two beats on its cues — "problems that would take supercomputers" (`kinetic-beat-slam`), then "millions of years" swaps in at double size with orange on "millions" (`discrete-text-sequence`); top-band placement, tiles' zone still empty.
Scene 2 (2.8–6.4s): the three tiles cascade in one per spoken cue — "new medicines" / "new materials" / "unbreakable codes" — each a flat bordered tile sliding up into the stack (`grid-card-assemble` cascade, one item per cue, long-tail settle); inside each tile its SVG glyph self-draws (`svg-path-draw`): a 5-node molecule, a 3×3 lattice, a padlock.
Scene 3 (6.4–8.0s): the completed stack holds; a keyword glow (`asr-keyword-glow`) sweeps "unbreakable" as the VO lands it; stillness to the cut.

narrativeRole: Cashes the power claim into three concrete stakes the viewer can picture — medicine, materials, encryption.
keyMessage: Exponential state-space means real-world impossible problems become solvable.

## Frame 5 — The catch

- scene: Hard tonal turn on the same dark stage. "the catch?" alone in huge type. Then: "one tiny vibration destroys the magic." — the display type itself jitters and glitch-shakes as the line lands. Then a temperature readout counts DOWN: 20°C → −273.135°C, frost-blue ambient bleeding in, ending on "colder than deep space" with "deep space" in orange.
- voiceover: "The catch? Qubits are so fragile, one tiny vibration destroys the magic. So quantum computers live in freezers colder than deep space."
- duration: 9s
- transition_in: cut
- status: outline
- src: compositions/frames/05-the-catch.html
- type: pain_point
- persuasion: Counterexample (here is when it breaks) + statistical proof
- beat: Tension + unease
- blueprint: dataviz-countup (Adapt)
- focal: the temperature counter plunging to −273.135°C
- roles: temperature readout = foreground subject (giant mono digits, center y≈806) · "the catch?" / "one tiny vibration destroys the magic." lines = foreground in scenes 1–2, cleared before the counter · frost-blue ambient wash = background (low-opacity overlay, ground only) · "colder than deep space" payoff line = supporting
- sfx: glitch, riser, impact-deep

Adapt: keep dataviz-countup's signature (one hero number carrying the argument) but invert it — the counter counts DOWN, and the emotional arc runs still → violent → cold. This frame owns the video's planned held beat (Scene 1) and its only sanctioned shake (the vibration IS the subject).
Scene 1 (0.0–1.8s): everything else gone — "the catch?" alone, centered, huge, lands on its cue (`kinetic-beat-slam`) and then HOLDS in true stillness for a full beat; the video's breather before the turn.
Scene 2 (1.8–4.6s): on "one tiny vibration", the line "one tiny vibration destroys the magic." reveals per-word (`dynamic-content-sequencing`) — and on "destroys", the whole type block violently jitter-shakes (`sine-wave-loop` at high amplitude, finite, decaying) with a glitch SFX; the shake decays to dead still by "magic."
Scene 3 (4.6–9.0s): scale-swap (`scale-swap-transition`) hands the center to a giant mono temperature readout starting at "20°C"; on "freezers" it plunges — a value-scaled countdown (`counting-dynamic-scale`, digits shrinking-cooling in tracking as the number falls) to "−273.135°C" while a frost-blue ambient wash bleeds into the ground (`ambient-glow-bloom`, cold register, background only); on "colder than deep space" the payoff line stamps beneath with "deep space" in orange (`kinetic-beat-slam`); hold the frozen read.

narrativeRole: The twist beat every good Short has — undercuts the hype with the real physics problem (decoherence) and lands the most shareable fact: colder than deep space.
keyMessage: Quantum states are absurdly fragile — that fragility, not power, is the real engineering battle.

## Frame 6 — Payoff

- scene: Bare dark canvas, calm after the glitch. Two beats of huge type: "the next computing revolution isn't coming." — then "isn't coming." wipes and "it's already being built." spring-pops in with a fire-orange underline drawing beneath "already". Small mono chrome line settles at the bottom of the safe area: "follow for more science in 40 seconds".
- voiceover: "The next computing revolution isn't coming. It's already being built."
- duration: 6s
- transition_in: crossfade
- status: outline
- src: compositions/frames/06-payoff.html
- type: branding
- persuasion: Distillation + callback
- beat: Inevitability + resolve
- blueprint: kinetic-type-beats (Reproduce)
- focal: the line "it's already being built." with the orange underline on "already"
- roles: thesis lines = foreground subject (centered stack, y≈806) · orange underline = supporting accent · follow line = supporting chrome (mono, small, above the caption band) · faint digit columns callback = background (dim ~30%, echoes Frame 1)
- sfx: impact-deep, whoosh-soft

Reproduce: kinetic-type-beats — a two-beat statement where the second beat replaces the first's ending in place; the swap is the payoff.
Scene 1 (0.0–2.4s): the faint "0 1" digit columns from Frame 1 return as background (callback, dim); "the next computing revolution" lands per-word on its cues (`dynamic-content-sequencing`), then "isn't coming." beat-slams beneath (`kinetic-beat-slam`); centered stack, hero scale.
Scene 2 (2.4–4.4s): on "already being built", "isn't coming." hard-cut swaps to "it's already being built." (`discrete-text-sequence` — the in-place swap is the beat); a fire-orange rule draws itself under "already" (`svg-path-draw`); faint glow blooms behind the line (`ambient-glow-bloom`).
Scene 3 (4.4–6.0s): the mono chrome follow line "follow for more science in 40 seconds" ticks in small above the caption band (`dynamic-content-sequencing`); long still hold to the end — the final exit is a simple settle, no motion past the last reveal.

narrativeRole: Lands the thesis as a one-line stinger and closes the loop opened by the hook — the impossible machine from frame 1 is real and under construction.
keyMessage: Quantum computing is not sci-fi — it is being built right now.
