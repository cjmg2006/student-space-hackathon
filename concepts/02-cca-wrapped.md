# Concept 02 — CCA Wrapped (Story Threads) — DEPRECATED

> **Status: DEPRECATED as of 2026-04-27.** Reza pushed back: too narrow as scoped (CCA-only, term-end-only). Replaced by three broader candidates: [02a Day Logs](02a-day-logs.md), [02b Say It Better](02b-say-it-better.md), [02c Threads](02c-threads.md). Recommended replacement: **02b Say It Better**. See [README](README.md) for the full rationale.
>
> The original concept is preserved below for reference only. Some elements (cross-term continuity, Wrapped-style synthesis) survive in the replacements.

---

A capture-and-synthesize ritual. Students log small CCA moments in real time. The app helps them find the pattern and shape the language at term-end. The artifact is theirs to edit, keep, and carry forward across years.

## Anchor

**Primary hypotheses:** H1 (linguistic gap), H5 (past launchpad experiences), H11 (agency over surface).

**Secondary:** H10 (fear of consequences).

**Wedge insight (from research):**
> "The gap is linguistic, not experiential. Students have rich enough experiences. What is missing is the prompts, language, and continuity to connect them into self-understanding." (synthesis, primary systemic gap)

Plus: "Experiences are indeed a powerful leaping point, even if level of maturity is: 'I like X, I'm good at Y.' The intervention mines and connects, rather than creates new experiences." (Apr 22)

**The bet:** students don't need more experiences. They need help connecting the experiences they already have into a coherent, self-authored narrative, with their own language. Building this language is a learnable skill if the prompts and synthesis are well-designed.

## Pitch

Capture small CCA moments now. AI helps you find your pattern. End-of-term, you have language for who you've been becoming. You edit it. You keep it. You carry it forward.

## Scenario

Junhao, Sec 2, joins the school band. First three weeks of CCA term, the app sends him 1-2 push notifications during practice. Each is a 5-minute capture window: mood emoji + 60-second voice or 1 photo + 1 sentence. He picks the easiest option each time.

His captures: "Pak Cik [sectional teacher] showed me a different fingering today and I felt stupid for like 10 seconds and then good. Photo of my marked-up score." Some weeks he skips entirely. No penalty.

By week 5, the app shows a "do you see something" check: a small panel with three of his moments and one observation. "I noticed three of your moments mention Pak Cik. Is something happening there?" Junhao thinks. He hadn't noticed that. He taps "yeah, kinda" and adds: "He's the first teacher who treats me like I might actually be good." That becomes part of his thread.

By week 10 (end of term), he gets a notification: "Your CCA story is ready. 12 minutes." He opens it. Vertical-scroll, like a Wrapped slideshow. The AI has identified a theme: "I noticed you came back to the moment when you helped a junior debug the bass line. You called that 'just being patient' but it shows up six times." Junhao reads. He thinks "yeah, but it's not patience. It's that I get a kick out of seeing them figure it out." He taps the slide and edits the text. The slide now says: "I'm someone who gets a kick out of seeing other people figure things out."

He saves the story. A year later, when he opens the Future Self Simulator and picks "Try a Day - teaching", the simulator pulls from this thread. The agent says: "You said you get a kick out of seeing others figure things out. Let's start there."

## Mechanic

Three components, working together:

1. **Capture.** Push-notified, low-friction, structured (mood emoji + 60s voice or photo + 1 sentence). Random within CCA hours. Frequency tunable. Default: 1-2 per week.
2. **Mid-term observation.** AI surfaces an emerging pattern at week 5 and asks a single open question. Student can confirm, deny, or rewrite.
3. **End-of-term synthesis.** AI generates a draft story (8-12 vertical slides). Student edits. Final artifact is identity claim + 3-5 supporting moments + one tiny experiment for next term.

**Three design constraints that make it work:**

- **Capture is sub-60-seconds.** Voice + photo over typing. Captures impulse, not curated reflection.
- **AI is a draftsperson, not the author.** Edit affordance on every slide. Multiple regenerate options. The student's words win.
- **Cross-term continuity.** Each term builds on the last. The thread becomes a personal narrative archive that grows across years.

## How it connects to each hypothesis

- **H1 (linguistic gap):** primary connection. The synthesis IS the language scaffolding moment. Student gets a draft of language they didn't have, then revises it toward truth.
- **H5 (past launchpad experiences):** the captures are the past experiences being mined. Even thin beliefs ("I'm good at X") become threads.
- **H11 (agency over surface):** student edits, names, owns the artifact. Not a form they fill in. Mirrors the e-portfolio finding: students who feel ownership take it seriously.
- **H10 (fear of consequences, secondary):** captures stay on-device by default. The synthesis is the only thing that ever leaves, and only if shared.

## How it resolves each tension

- **Risk 1 (consequence fear, critical):** on-device capture. AI synthesis runs locally or with no-retention contract. Privacy posture is visible inside the app, not buried in T&Cs.
- **Risk 2 (covertness paradox):** honest framing. "Save your CCA moments. We'll help you find the story." Reflection is the byproduct of memory-keeping.
- **Risk 3 (platform vs relationship):** lower platform-vs-relationship risk than Future Self because the synthesis is a deliverable to YOURSELF, not a substitute for human conversation. Light teacher activation ("we're trying this in our CCA"); the tool is solo-use after that.
- **Risk 4 (reactive vs reflective muscles):** ambient capture builds the muscle. Term-end synthesis is the structured milestone. Two-mode design.
- **Risk 5 (teacher as guide vs risk):** teachers see synthesis only if the student shares. They never see captures.
- **Risk 6 (institutional frame):** student-installed app. MOE referral, not hosting.

## Mobile UX — key moments

- **Capture screen.** One tap to record, max 60 seconds, single screen. Mood emoji top, voice/photo bottom. Five-minute window after notification.
- **Mid-term observation panel.** Small card, one observation, three buttons (yes / no / let me edit).
- **Synthesis story.** Vertical-scroll like Spotify Wrapped or Instagram stories. 8-12 slides. Each slide has an edit affordance. Tap to rewrite. Hold to regenerate.
- **Story library.** Timeline view. Each term is a chapter. Past stories visible. Quotable moments tagged for reuse.
- **Share sheet.** Full story or single slide. Native iOS/Android share. Default audience = nobody.

## Failure modes

- **AI synthesis sounds generic.** Students reject it. Mitigation: fine-tune prompts heavily on actual student language. Test before deploying. Allow regenerate-from-different-angle.
- **AI projects identity claims the student rejects.** ("I'm a leader" when they don't see themselves that way.) Mitigation: edit affordance is one tap. Multiple draft options. Student can decline a slide.
- **Sparse captures, thin story.** Mitigation: mid-term check surfaces this and offers a "fill in" mode where AI asks a question to top up.
- **Capture fatigue.** Notifications get muted. Mitigation: tunable cadence. Default low (1-2 per week). Notifications are gentle.
- **Story leaks.** Student feels exposed. Mitigation: stories private by default. Sharing requires explicit action. Native share sheet only, no in-app feed.

## Adoption strategy

- Teacher introduces in one CCA session at term start. Frame: "We're trying this. It's not for grades. It's for you to look back at your year."
- Cohort = one CCA. Mandatory installation? No. Opt-in only.
- End-of-term: optional showcase where students can voluntarily share one slide from their story. Builds peer normalization without mandatory disclosure.
- LEAPS staff are NOT informed. The story is not part of the LEAPS reflection requirement.

## Test plan

- 5 students from one CCA. Wizard-of-Oz: use a Telegram bot or Google Form for capture. Hand-craft the synthesis at week 10 (Claude in the loop to make it feel agent-generated).
- **Measure:** did students engage with capture (>60% of prompts answered)? Did the synthesis feel like them (post-read interview)? Did they edit it? Did they share any of it?
- **Falsifiable claim:** when students see the synthesis, at least 4 of 5 will say it captured something they hadn't articulated themselves. At least 3 of 5 will edit at least one slide to be more accurate. At least 2 of 5 will choose to share at least one slide.
