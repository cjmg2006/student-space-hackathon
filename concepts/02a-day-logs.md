# Concept 02a — Day Logs

A 60-90 second voice habit, every day, about anything. Across CCA, classroom, friends, family, anything that happened. Light monthly synthesis surfaces the patterns the student couldn't see day-by-day.

## Anchor

**Primary hypotheses:** H1 (linguistic gap), H5 (past launchpad experiences), H11 (agency over surface).

**Wedge insight (from research):**
> "The gap is linguistic, not experiential. Students have rich enough experiences. What is missing is the prompts, language, and **continuity** to connect them into self-understanding." (synthesis, primary systemic gap; emphasis added)

The CCA Wrapped concept tried to capture continuity term-by-term. But students don't experience their lives in 10-week chunks. They live day to day, across academic, CCA, social, family, and personal domains.

**The bet:** continuity is the missing variable. A daily voice habit, low-friction and domain-agnostic, accumulates language across all of student life. Monthly synthesis surfaces themes the student couldn't see in any single moment.

## Pitch

One short voice note a day. About anything. Six months in, you have language for who you've been becoming.

## Scenario

Mei Lin, Sec 3, gets a notification at 9pm: "60 seconds. About anything." She's brushing her teeth. She picks up the phone, starts talking: "Today was weird. Mr Chen asked me to lead the discussion in lit class and I almost said no but then I just did it. It was actually fine. I don't know why I always think I can't." She taps stop. Tag suggestions appear: "academic", "leadership", "self-doubt". She picks the first two.

Wednesday she skips. Thursday she captures something about a fight with her brother. Friday she captures something about getting an unexpected compliment from a CCA junior. Saturday she skips. The app adjusts cadence quietly, no streak shaming.

A month later, a softer notification arrives: "Pattern check. 30 seconds." She opens it. The app shows: "You mentioned Mr Chen six times this month. The pattern: you're noticing when adults give you responsibility. You called yourself 'someone who almost said no but did it' twice." Mei Lin reads. Yeah, that's true. She types a one-line addition: "Maybe I'm not as scared as I think I am."

Three months later, her cousin asks her at family dinner what she wants to do. She doesn't say "I don't know" the way she usually does. She says "I think I'm someone who keeps surprising myself by saying yes." That language came from the library.

## Mechanic

Three components:

1. **Daily capture.** Voice note at student-chosen time (default 9pm). 60-90 seconds max. Domain-agnostic. Tag after speaking, not before.
2. **Quiet cadence adjustment.** Skip is free. No streaks. App auto-pauses if 7 days missed and waits to be re-invited.
3. **Monthly synthesis.** 30-second pattern flag, not a full narrative. AI surfaces 1-2 emerging themes. Student confirms, denies, or rewrites.

**Three design constraints that make it work:**

- **Voice-first, typing fallback.** Friction is the enemy of continuity. Voice is faster than typing in bed.
- **Light synthesis.** Monthly, not weekly. Pattern flag, not a finished story. Avoids over-summarizing thin data and avoids feeling surveilled.
- **Domain-agnostic capture, theme-aware synthesis.** Tags are how the student categorizes; themes are what the AI surfaces.

## How it connects to each hypothesis

- **H1 (linguistic gap, primary):** the synthesis closes the language gap. Student gets a draft of their own pattern, in language they can adopt or edit.
- **H5 (past launchpad, primary):** every voice note is a past experience being mined, even if thin. Six months of notes is a deep launchpad library.
- **H11 (agency over surface, primary):** student edits, tags, owns the library. AI is light-touch.

## How it resolves each tension

- **Risk 1 (consequence fear, critical):** voice notes encrypted on-device. Synthesis runs locally or with no-retention contract. Critical: privacy posture is visible inside the app.
- **Risk 2 (covertness paradox):** honest framing as a daily voice habit. Slightly weaker than CCA Wrapped's memory-keeping framing because students may perceive it as "reflection."
- **Risk 3 (platform vs relationship):** solo tool. Teacher can introduce ("this is something I do, you might try"), but the tool doesn't depend on them.
- **Risk 4 (reactive vs reflective muscles):** builds the muscle directly. Daily cadence IS the muscle.
- **Risk 5 (teacher as guide vs risk):** teacher never sees content.
- **Risk 6 (institutional frame):** outside MOE servers. Student-installed.

## Mobile UX — key moments

- **Capture screen.** One tap to record. 60-90s max. Big stop button. Tag suggestions appear after recording.
- **Library view.** Timeline + filter by domain or mood. Search by keyword.
- **Pattern check (monthly).** Small panel, 1-2 themes, three buttons (yes / no / let me edit).
- **Notification.** Gentle. Default 9pm. Movable. Snooze for a day with one tap.
- **Privacy posture.** Visible in-app banner: "On-device. No retention. Delete any note any time."

## Failure modes

- **Capture fatigue.** The single biggest risk. Mitigation: tunable cadence, generous skip, auto-pause after 7 missed days, low default frequency.
- **Surveillance feel.** "Why is this app tracking my daily life?" Mitigation: explicit privacy posture. Voice notes deletable individually. No analytics dashboard.
- **Synthesis hallucination.** AI sees patterns that aren't there. Mitigation: students confirm or deny patterns; rejected patterns don't reappear.
- **Triggering content.** Daily voice could surface mental health concerns. Mitigation: this is NOT a counselling tool. Standard signposting if certain phrases detected, no auto-escalation, no teacher visibility.
- **Domain skew.** Student only captures CCA moments out of habit, defeats the multi-domain goal. Mitigation: occasional prompt variants ("not from CCA today, what else happened?").

## Adoption strategy

- Soft introduction by a teacher, peer, or counsellor as a personal practice tool.
- Not deployed as a school programme. No mandatory rollout.
- Library is portable. Student can export at any time. No lock-in.

## Test plan

- 5 students from across CCAs and academic streams. 6 weeks.
- Telegram-bot wizard for daily prompt. Hand-craft monthly synthesis at week 6 (Claude in the loop).
- **Measure:** median capture rate by week 4? Did the synthesis surface something the student hadn't named? Did they edit? At week 6, did they want to keep going? Did any students capture across more than two domains?
- **Falsifiable claim:** at least 3 of 5 students hit >50% capture rate by week 4 across at least 3 domains. At least 4 of 5 say the month-1 synthesis showed them something true. At least 3 of 5 say they want to keep using it past week 6.
