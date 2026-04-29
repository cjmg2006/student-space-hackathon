# Prototype notes

Two passes recorded here. The original overnight build (2026-04-27) and the elevation pass (2026-04-27, after Reza asked for sim-game treatment of 03 and more cinematic moments overall).

## Elevation pass — what changed (most recent)

**03 Future Self Simulator — full rewrite as a simulation game.** This is now the centerpiece. The chat-based "Talk to Future You" was replaced by an illustrated single-scene studio simulation:

- Hand-crafted SVG of a music producer's home studio (~250 SVG primitives): wood floor, cream walls, window with sky gradient, posters, wall clock, door, rug, desk with laptop and lamp, mixing console with faders/knobs/screen, speaker monitors, glass mic booth with acoustic foam, plant
- Character drawn in 4 distinct poses (at desk / standing / at console / evening at desk) — fade transitions between them
- Time-of-day system: sky gradient changes through morning → midday → afternoon → evening → debrief; CSS overlay tints scene; lamp glow animates in evening
- Subtle ambient animation: plant sways, clouds drift, character "breathes," lamp pulses
- Top HUD: time pill ("9:00 AM · Tuesday") + 5-pip day timeline
- Bottom dialog: narration card + staggered choice cards
- Reaction system: comic-style speech bubble pointing to character, anchored by character position, with the actual consequence text
- Time-skip cutscene between scenes ("LATER THAT DAY · 12:40 PM · Same studio")
- **Branching debrief**: 4 different insights (curiosity / running things / craft / integrity), each producing a different postcard text and if-then prompt. Same simulation, different reflective endings depending on which moment the player says lit them up.
- Loading screen between setup and sim: starfield, "ENTERING TUESDAY"
- Mode picker reordered: "Try a Day" is the open mode, "Talk to Future You" is now marked Soon

**01 Mirror Talk — cinematic arrival moment.**

- Ambient green flash overlay sweeps across the screen when a new mirror arrives
- Mirror card lands with a scale-bounce entrance + ripple ring outline
- "Saw you today" indicator now subtly pulses
- The arrival is now an event, not a list-update

**02b Say It Better — theatrical reveal.**

- Thinking moment redesigned: large breathing orb with concentric ripple rings (replaced bouncing dots)
- Thinking text cycles through three phrases ("Listening to what you really meant" → "Finding the words you didn't have" → "Drafting three angles")
- Three-version cards stagger in one at a time with a soft bounce, ~380ms apart
- Original-rant recap fades in first, before the versions
- When you pick a version, the others dim to 35% opacity and slightly blur; the selected one lifts and brightens

## Decisions made in the elevation pass

- **Sim-game style for 03 only.** 01 and 02b got cinematic touches but kept their core UI metaphors (messaging app, utility tool). Forcing a sim metaphor on those would have been counterproductive. Their elevation focused on the magic moments (arrival, version reveal).
- **Mode 1 vs Mode 2 swap.** The concept doc had Mode 1 (Talk to Future You) as the v1 build target. The elevation reveals that Mode 2 (Try a Day) is actually the more compelling experience and the one that lands the simulation game framing. Mode 1 is now positioned as a smaller / lower-stakes alternative for v2.
- **Branching debrief over single insight.** Originally the postcard was hardcoded. Now there are 4 different insights and 4 different postcards. Makes the simulation feel responsive and rewards multiple playthroughs.
- **Hand-drawn SVG over imported assets.** Pure SVG primitives, no image files. Trade-off: slightly stylized/chunky look (think Animal Crossing's flat illustration register), full portability and editability, no asset pipeline.
- **5-scene structure.** Morning email / late vocalist / mix problem / sample issue / debrief. Three weekday issues + one ethics issue + reflection. Could expand to 6-8 if the team wants a longer day.
- **Choice consequences are honest, not gamified.** No score, no win state. Each choice in the day produces a real-feeling reaction from future-you ("I tried that. He went quiet. We didn't end up working again."). The point isn't to win; it's to notice what you'd do.
- **Music producer is the only full day.** The setup lets you type any role, but only "music producer" has the full scripted day. Other roles will fall through to the same script. Documented as a known limitation.

## Open questions from the elevation pass

In rough priority:

1. **Aesthetic call on 03.** I went stylized-chunky / Animal Crossing-flat-illustration in pure SVG. Could shift cooler/more painterly, or more pixel-art, or more vector-flat. CSS vars and SVG are at top of the file if you want to re-skin.
2. **Day length / scene count.** Five moments takes ~3 minutes to play. Could go longer with more nuance, or shorter for a tighter experience. Sweet spot for testing?
3. **Multiple roles or just one?** Should the Try a Day prototype have 3-4 fully-scripted role variants (producer, teacher, designer), or is one enough to validate the concept?
4. **Reaction bubble persistence.** Currently disappears after ~4 seconds. Should the player be able to dismiss / re-read?
5. **Branching debrief — should choices in the day matter to which insights are available?** Right now, all 4 insights are always available regardless of how the day went. Could be: only insights related to choices you actually made are available. More work but more responsive.
6. **Time-skip cutscene tone.** Currently functional. Could be more atmospheric (a quote from future-you, an environmental beat, a song title).
7. **Sound design.** No audio. A simple ambient layer (soft synth pads, the lamp click on, distant city sounds through the window) would dramatically lift the sim feel. Not built. Worth a v1.
8. **Self-criticism safeguard for 02b.** Still an open design problem from the concept-deepening pass. Not addressed in either prototype version.

---

## Original overnight pass — what got built (older)

Three single-file HTML prototypes, mobile-shaped, self-contained, no backend, no AI calls. Each demonstrated the core mechanic of one concept end-to-end.

- `01-mirror-talk.html` — peer mirror flow with simulated async arrival
- `02b-say-it-better.html` — voice rant to three articulated versions to library (canned demo)
- `03-future-self-simulator.html` — Mode 1 only, scripted future-self conversation (since replaced)

Open any of them by double-clicking. Works in any browser.

## What got built

Three single-file HTML prototypes, mobile-shaped (375px container), self-contained, no backend, no AI calls. Each demonstrates the core mechanic of one concept end-to-end.

- `01-mirror-talk.html` — peer mirror flow with simulated async arrival
- `02b-say-it-better.html` — voice rant to three articulated versions to library (canned demo)
- `03-future-self-simulator.html` — Mode 1 only, scripted future-self conversation through to postcard and if-then capture

Open any of them by double-clicking. Works in any browser. No install required.

## Decisions made on your behalf

**Format.** Single-file HTML. Vanilla JS. No framework, no build step, no server. You can edit any of them directly in a text editor. Trade-off: no component reuse across prototypes; if we go to v1 we'll likely rebuild in React or Swift.

**Aesthetic direction.** Warm cream background, soft sage accent, system fonts. Designer-friendly minimal, in the Linear / Things 3 / Apple Notes register. NOT corporate, NOT institutional. The visual language is one of the design statements. You can change it; the CSS variables are at the top of each file.

**Mobile-shaped, not actually mobile.** Each prototype renders at iPhone width (375px) inside the browser. There's a phone-frame wrapper visible on desktop. On a real mobile browser it goes full-screen. This is deliberately rough; it's a clickable mock, not an iOS build.

**No real AI, no real audio.** 02b's three-version output is canned for one demo rant (Joshua's interview moment from the spec). 03's chat is fully scripted. 01's "voice note" is a simulated audio waveform with no real recording. This is fine for conceptual review. For user testing you'll want real AI.

**No persistence.** Reload the page and state resets. By design (no localStorage in this environment, and persistence isn't useful for a demo).

**Demo data.** Used the named characters from the concept docs (Aisyah, Tasha, Hakim for 01; Joshua for 02b; Wei Ming for 03). Keeps the prototype tied to the scenarios you've already read.

**One scripted flow per prototype, not a full app.** Each prototype demonstrates the magic moment of its concept clearly, with one or two additional screens for context. They're not feature-complete apps. The goal is "show the mechanic to a teammate in 90 seconds."

## Questions for tomorrow

In rough priority order. Items I genuinely want your call on, not things that block the prototypes from being useful as-is.

1. **Aesthetic.** I went warm cream + sage. Designer call. If you want different mood (cooler / darker / more playful / Singapore-specific palette), say so and I'll re-skin all three in one pass. CSS vars are at top of each file.

2. **One app or three?** The prototypes are three separate flows. The concept docs suggest these could be one app with three modes. Should v1 be a unified shell with mode-switching, or three discrete experiences?

3. **02b's three-version naming.** I labelled the versions "literal", "identity", "specific" inside the prototype. Felt clinical. Better candidates: "as you said it / as a claim about you / as a story". Want to workshop?

4. **02b voice fidelity.** Canned three-version output is fine for the demo, but the mechanic's quality depends entirely on the AI prompt. Want me to draft and test the actual rephrase prompt next? That's the highest-leverage technical work for 02b.

5. **03's agent character voice.** I wrote the future-self responses in a "friendly older sibling who's lived through it" register, leaning warm and specific. Could feel different (more wry, more grounded, less expressive). Worth a side-by-side test with 2-3 voice options.

6. **01's friend graph bootstrap.** The prototype assumes friends are already added. In a real app, how does the graph get established without school accounts? I noted this as an open design question in the concept doc; haven't solved it.

7. **Self-criticism safeguard for 02b.** In the deepening pass we identified self-criticism rehearsal as the most ethically important failure mode. The prototype doesn't include any safeguard. Want me to design the safeguard mechanic before any user test of 02b?

8. **Prototype showcase format.** Should I also build a single-page index that lets the team click between all three? Or are the three files enough?

9. **Mode 2 (Try a Day) and Mode 3 (Branching Path) for 03.** Only Mode 1 is in the prototype. Mode 2 is the most distinctive of the three but also the most complex (interactive day simulation). Worth prototyping if 03 advances.

## Things I considered and decided NOT to do

- **Real audio recording in 02b.** Browser audio APIs work but introduce permission flows and dead-end UX (no real transcription). Cleaner to fake the voice input with a typed-rant + record-button visual.
- **Real AI in 02b.** Requires API key, rate limits, and prompt-tuning. Premature for a conceptual prototype. Better as the next step once the prototype is reviewed.
- **Animation library for 03's "appearance" moment.** Used a simple CSS fade + delay. Looks OK. A library would be over-engineered.
- **Onboarding flows.** Skipped onboarding screens. Each prototype drops you into the active state. Real app needs onboarding; for a demo it's noise.
- **Privacy posture screens.** Critical for the real product (visible privacy is load-bearing per the concept docs). Skipped here for prototype scope. Worth adding before user testing.
- **Multilingual / Singlish support.** Out of scope for the prototype, in scope for the real product.

## How to use these in a hackathon

For each prototype, the suggested 90-second demo flow:

**01 Mirror Talk.** Open. Show the library tab — already populated with two mirrors received. Tap "Mirror time." Pick two friends. Send. Switch to Pending tab — show one question waiting from a friend. Reply. Switch back to library — watch a new mirror arrive (simulated). Total time: 90 seconds.

**02b Say It Better.** Open. Show library with three saved articulations. Tap "Say it better." Use the demo rant (pre-loaded with Joshua's interview moment). Hit "send." See three versions. Pick version 3. Edit one word. Tag and save. Show new entry in library. Total time: 75 seconds.

**03 Future Self Simulator.** Open. Pick "Talk to Future You." Pick age 25. Type "the version of me who became a music producer" or pick suggested chip. Watch the appearance moment. Walk through the scripted conversation (pick suggested replies or type your own). Get to the postcard. Pick open date. Capture if-then. Total time: 2 minutes.

## Risks of using these as research stimuli

- The fidelity is just-believable-enough that students might think the AI output is intelligent. It isn't. Show the canned demo rant only. Don't let students try arbitrary inputs.
- The aesthetic looks finished. Reviewers might focus on visual details rather than the mechanic. Strip the UI to wireframe before user-testing if visual polish is distracting from the concept critique.
- These feel like working products, not concepts. Frame them carefully when sharing: "this is a concept demo, the core mechanic is what matters, not the UI."

## File locations

All under `student-space-hackathon/prototypes/`:
- `NOTES.md` — this file
- `README.md` — index with demo flows
- `01-mirror-talk.html`
- `02b-say-it-better.html`
- `03-future-self-simulator.html`

Open the HTML files directly in any browser. No setup required.
