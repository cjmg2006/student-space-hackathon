# Prototypes

Three clickable HTML prototypes demonstrating the core mechanic of each concept. Each one self-contained, mobile-shaped, no setup required.

| File | Concept | What it shows |
|---|---|---|
| [01-mirror-talk.html](01-mirror-talk.html) | 01 Mirror Talk | Library, send flow, async reply, **cinematic mirror arrival** with ambient flash and ripple |
| [02b-say-it-better.html](02b-say-it-better.html) | 02b Say It Better | Library, voice rant, **atmospheric thinking moment**, **theatrical staggered three-version reveal**, dim-on-select, edit, save |
| [03-future-self-simulator.html](03-future-self-simulator.html) | 03 Future Self Simulator | **Full simulation game**: illustrated studio scene, day-cycle (5 moments, 9am→8:30pm), animated character at 4 positions, time-of-day shifts, choice cards with consequences, debrief that branches the postcard |
| [journey-map.html](journey-map.html) | All three | **System journey map**: 4 personas, trigger × solution matrix, 3 entry doors, 4 persona pathways, cross-solution flow diagram. Companion to [JOURNEY-MAP.md](../concepts/JOURNEY-MAP.md). |

See [NOTES.md](NOTES.md) for decisions made and questions still open.

## How to use

Open any HTML file in a browser. Renders in a phone-frame on desktop; full-screen on mobile. No install, no backend.

## Suggested demo per prototype

### 01 Mirror Talk (~90 seconds)

1. Land on the Mirrors tab. Three sample mirrors received (one anonymous).
2. Tap **Send** in the bottom nav. Today's question shown. Pick two friends with the "saw you today" indicator (now subtly pulsing).
3. Tap **Send to 2 friends**. Confirmation. Tap **Got it**.
4. Tap **Pending** in the bottom nav. One question waiting from Tasha.
5. Tap the question. Reply screen. Use the simulated voice waveform. Tap **Send mirror**.
6. Returns to Mirrors tab. About 4 seconds later: ambient green flash, new mirror lands with a scale + ripple animation, "A new mirror just arrived" toast. The mirror has the NEW badge and a soft glow.

### 02b Say It Better (~90 seconds)

1. Library with three saved articulations.
2. Tap **Say it better** at the bottom.
3. Tap **Use demo rant** in the top right. Joshua's interview rant fills the textarea.
4. Tap **Find better words**. **The thinking moment is now atmospheric**: a breathing orb with concentric ripples, text cycling through "Listening to what you really meant" → "Finding the words you didn't have" → "Drafting three angles."
5. **The three versions stagger in**, one at a time, with a soft bounce. Tap one (try Version 3 — "as a story").
6. The other two **dim and slightly blur**, the selected one lifts.
7. Tap **Continue**. Edit screen. Edit if you want. Pick tags.
8. Tap **Save to library**. Returns to library. New entry on top.

### 03 Future Self Simulator (~3 minutes — the big one)

This is now a full simulation game.

1. Mode picker. **Try a Day is now the active mode** (was Talk to Future You; the chat-only mode is now marked "Soon").
2. Tap **Try a Day**. Setup: pick age (default 21), type or pick "music producer."
3. Tap **Begin**. Loading screen with starfield: "ENTERING TUESDAY · A morning in your studio."
4. **Scene opens.** Illustrated studio: warm cream walls, wood floor, window with morning sky, posters, clock, desk with laptop and lamp, mixing console with knobs and faders, glass mic booth on the right, future-you sitting at the desk in a coral t-shirt with headphones.
5. **Top HUD**: time pill ("9:00 AM · Tuesday") and a 5-pip day timeline.
6. **Bottom dialog**: "TUESDAY MORNING — An email just landed. The client wants to renegotiate the rate..."
7. **Three choice cards stagger in.** Tap one.
8. **Future-you's reaction floats in as a comic-style bubble** anchored to the character with the actual consequence ("Smart. Turned out his budget got cut...").
9. After ~4 seconds, **time-skip cutscene**: "LATER THAT DAY · 12:40 PM · Same studio."
10. **Scene transitions**: sky color shifts to midday blue, character is now standing in the middle of the room looking at the empty mic booth. Repeat the choice + reaction cycle.
11. **Scene 3 (3:30 PM)**: golden afternoon tint, character at the console with headphones on. Mix-isn't-sitting moment.
12. **Scene 4 (6:15 PM)**: deep evening warm tones, **lamp on desk now glows softly**, character back at desk looking down. Sample-uncleared moment.
13. **Scene 5 — Debrief (8:30 PM)**: scene dims, lamp glow prominent, vignette feel. Future-you turns to face you. "OK. Real question. Of all that, which moment lit you up?"
14. **Four debrief choices**, each tied to a different insight (curiosity / running things / craft / integrity).
15. Pick one. **Future-you delivers the matching insight**, e.g. "That's not a music thing. That's a running-things thing."
16. Transitions to **the postcard** — the postcard text now reflects which insight you picked.
17. Pick a seal date. Tap Continue.
18. **If-then capture screen**, pre-filled based on your insight.
19. Save. **Done screen** with the captured if-then.

The choice you make at debrief actually changes the postcard text and the if-then prompt. Try the demo twice with different debrief choices to see different outcomes.

## What's new in this elevation pass

**03 Future Self Simulator — full rewrite as simulation game.**

- Replaced text-chat with a single illustrated 800x600 SVG scene of a music producer's home studio
- Hand-crafted SVG: window with sky gradient, posters, clock, door, rug, desk, lamp, laptop, console with faders/knobs/screen, monitors, mic booth with acoustic foam, glass partition, plant
- Character drawn in 4 distinct poses (at desk / standing / at console / evening at desk), shown via fade transitions
- Time-of-day system: sky gradient changes between morning / midday / afternoon / evening / debrief; a CSS overlay tints the whole scene; lamp glow appears in evening scenes
- Subtle ambient animations: plant sways, clouds drift across the sky, character "breathes," lamp pulses softly
- Top HUD: time pill + day-progress timeline
- Bottom dialog system: narration card + choice cards that stagger in
- Reaction bubble: comic-style speech bubble pointing to the character, anchored to character position
- Time-skip cutscene between scenes: "LATER THAT DAY · 12:40 PM"
- Branching debrief: 4 different insights, each producing a different postcard and if-then prompt
- Loading screen between setup and sim: starfield, "ENTERING TUESDAY"

**01 Mirror Talk — cinematic arrival.**

- New mirror arrives with ambient flash overlay (soft green radial gradient across screen)
- Mirror card lands with scale-bounce entrance, ripple ring around the card, then settles
- "Saw you today" indicator now has a soft pulse animation
- The arrival is now an event, not just a list-update

**02b Say It Better — theatrical reveal.**

- Thinking moment redesigned: large breathing orb with concentric ripple rings instead of bouncing dots
- Thinking text cycles through three phrases over the loading period
- Three-version cards now stagger in one at a time with a bounce
- Original-rant recap fades in first
- When you pick a version, the others dim and slightly blur, while the selected one lifts and brightens

## Visual / interaction design choices

- **Aesthetic.** Warm cream background (#FAF8F4), soft sage accent (#5B7B66), warm orange highlight (#D9826E), system fonts. Designer-friendly minimal.
- **Mobile-shaped.** All three prototypes use a 390x844 phone frame on desktop and go full-screen on mobile.
- **No real AI.** Canned responses for 02b's three versions and 03's scripted day.
- **No real audio recording.** Voice affordances are visual only.
- **No persistence.** Reload resets state.

## Limitations to flag when sharing

These are concept demos, not products.

- The AI outputs are pre-baked. Use the demo flows.
- The visual polish makes them feel finished. Reviewers might focus on UI rather than mechanic. If that becomes a problem, strip to wireframe before user-testing.
- 03's day is deterministic at the structural level (5 fixed moments, fixed reactions per choice), but the debrief branches into 4 different endings.
- 01's friend graph is hardcoded.
- 02b's three versions are the same for every input.

## What to build next

In rough priority:

1. **Real AI for 02b.** Draft and test the three-version prompt. Highest-leverage technical work in the entire concept set.
2. **Self-criticism safeguard for 02b.** Before any real user test.
3. **Three-voice test for 03.** Prototype 3-4 character voices for future-you and pick one.
4. **More day variants for 03.** Currently only "music producer" works as the canned simulation. Other roles (teacher, designer, researcher) should each have their own scripted day.
5. **Friend graph bootstrap for 01.** Open design problem.
6. **Privacy posture screens.** Visible privacy is load-bearing; missing from current prototypes.
7. **Onboarding flows** for any of them.
