# Concept 03 — Future Self Simulator

A mobile agent that lets students step into possible futures by inhabiting them, not writing about them. Three modes, all closing with one tiny experiment to try this week. Seeded from real student moments and grounded in real practitioner data.

## Anchor

**Primary hypotheses:** H3 (hard to see what's possible), H12 (action gap).

**Secondary:** H1 (linguistic gap), H5 (past launchpad experiences).

**Wedge insight (from research):**
> "Students from less educated families can't relate to traditional success paths. Some are really fighting for survival; they will not be thinking so far ahead. They can't relate to it, or see a future for themselves." (Apr 23 school session)

Plus the action-gap insight:
> "Instead of figuring out 'I want to be a doctor', how about helping them find the next smallest thing they can try? Connecting 'you want to be an influencer' to 'you need to learn to write scripts and understand data'." (Apr 21)

**The bet:** imagination of possible selves is a learnable skill. The gap between "I can't see a future for myself" and "I have one tiny experiment to try this week" is the highest-leverage and highest-equity intervention in the entire problem space. This concept attacks that gap directly.

## Pitch

Step into a possible future. Talk to it, try a day inside it, or branch from a fork you're facing. Every session ends with one small thing you could try this week. Built from real practitioner data, not stereotypes.

## Scenario

Wei Ming, Sec 4, has been wondering about being a music producer. He doesn't know anyone who does that. His parents work in F&B. The school's career talks have been doctors, lawyers, civil servants.

He opens the app. Picks "Try a Day — Music Producer." The app says: "I'll run you through a real day. The agent is built from interviews with three Singaporean producers. Here we go."

**Morning.** An email from a client asking to renegotiate a session fee. Three options. Wei Ming picks "ask why before answering." The agent (in the producer's voice): "Smart. Turned out the client's budget got cut. We negotiated half-fee for a reduced scope."

**Midday.** A vocalist is 40 minutes late. Options: chase, bill, use the time to mix. Wei Ming picks "chase." Agent: "Fair. I called. She'd missed the bus. We started 60 minutes late. I felt grumpy for the first hour."

**Afternoon.** A mix isn't sitting. Scrap and restart, or push through. Wei Ming picks "push through." Agent: "I did the same. Spent two hours forcing it. By 6pm I knew it was wrong but I was tired. I sent it anyway."

**Evening.** A sample turned out to be uncleared. Wei Ming chooses how to handle it.

After 12 minutes, debrief.

> Agent: "Which moment lit you up?"
> Wei Ming: "The one where the vocalist was late. I liked solving it."
> Agent: "Interesting. That's not music-producer-specific. That's a project-management instinct. Have you noticed yourself enjoying that anywhere else?"
> Wei Ming: "Yeah... when our band gear got mixed up before the showcase. I sort of just ran it."
> Agent: "What's the smallest version of running a thing this week?"
> Wei Ming: "I could volunteer to coordinate tomorrow's sectional setup."
> Agent: "Want me to remind you tomorrow at 2pm?"
> Wei Ming: "Yeah."

Saved as if-then: "Tomorrow at 2pm, I'll message the band leader and offer to coordinate the gear setup."

The session ends. Wei Ming didn't decide to be a music producer. He learned something true about himself today.

## Mechanic

Three modes, unlocked progressively:

1. **Talk to Future You.** Conversational chat with a future-you-at-21/25, seeded from CCA Wrapped patterns or named verbally. Future-you responds in character, asks back, shares a vivid moment. Closes with a postcard from possible-future-you to today-you.
2. **Try a Day.** Interactive simulation of a day in a possible role. Drawn from a library of practitioner-grounded personas (real anonymized day-in-life data, not stereotyped occupations). Choose-your-action format. 10-15 minutes.
3. **Branching Path Explorer.** Student names a real fork (subject combo, JC vs poly, joining a CCA leadership team). Agent generates 2-3 plausible 3-year futures from each option. Student can then enter Mode 2 inside any of them.

**Two anchoring prompts in every mode:**

- **Inward bridge.** "What does this future say about who you are TODAY?" Resolves H2's failure mode (outward easier than inward). Without this, the simulator reinforces pathway-thinking.
- **Smallest experiment.** "What's the smallest version of this future you could try this week?" Captured as if-then implementation intention. Notification reminder built in.

**Three design constraints that make it work:**

- **Practitioner-grounded library.** Personas are built from real anonymized day-in-life data, not generic role descriptions. Prevents glamorized or stereotyped futures.
- **Agent doesn't recommend.** Its job is to make possibilities legible and then ask better questions. The student decides.
- **Every session ends with an action commitment.** Not optional. The if-then capture is the artifact that bridges insight to micro-action.

## How it connects to each hypothesis

- **H3 (hard to see what's possible):** primary. The whole concept is built to attack this gap. Particularly load-bearing for students whose family/friends modelled few paths.
- **H12 (action gap):** primary. Every session ends with a captured if-then commitment. Notification reminders close the loop between insight and try.
- **H1 (linguistic gap, secondary):** the agent provides language and scenarios the student doesn't have. The day-in-the-life vocabulary lifts students into a frame they couldn't access alone.
- **H5 (past launchpad, secondary):** when seeded from CCA Wrapped, simulations build on the student's own thin beliefs ("I'm good at X") rather than starting from zero.

## How it resolves each tension

- **Risk 1 (consequence fear, critical):** conversation runs in-session and is not persisted. Only the postcard artifact and the if-then experiment are saved. AI provider must offer no-retention contract. Privacy story has to be visible in-app, not buried.
- **Risk 2 (covertness paradox):** fully honest framing. "Talk to a possible future version of yourself." It is what it says.
- **Risk 3 (platform vs relationship, highest risk):** standalone agent simulation is closest to the Journey Together failure. Mitigations:
  - Teacher introduces in CCA or ECG session, demos one Mode 1 session live
  - Student can save a moment and bring it to a 1:1 with a trusted teacher or peer
  - Optional peer mode: two friends do Mode 2 together and compare debriefs
  - Optional teacher debrief: student opt-in shares postcard with a trusted teacher who responds with their own observation
  - Without at least one of these activation layers, this concept fails predictably
- **Risk 4 (reactive vs reflective muscles):** best as curiosity-triggered or fork-anchored ritual, not daily. Notification cadence aligned to ECG checkpoints + student-initiated.
- **Risk 5 (teacher as guide vs risk):** teacher sees only what student chooses to bring. Role is debrief partner, not assessor.
- **Risk 6 (institutional frame):** student-installed app. AI provider contract visible. Critical: NOT on MOE servers.

## Mobile UX — key moments

- **Mode 1 entry.** Choose age (18, 21, 25), choose version ("the version of me who became X"). If unsure, agent helps narrow with three questions.
- **The "appearance" moment.** When future-you appears, a short visual moment that matters. Gentle animation. Sets the tone that this is a serious imaginative space.
- **Voice option.** Talking is more powerful than typing for this concept. Voice should be available in all modes.
- **Mode 2 (Try a Day) screen.** Chat-thread style with rich media (emails, messages, audio clips). Choices appear as buttons.
- **Saved moments library.** Postcards from past simulations. Searchable. Student can revisit.
- **If-then capture.** Single screen at end of session. Auto-suggests structure. Notification reminder option.

## Failure modes

- **Hallucinated future is wildly inaccurate.** Student loses trust. Mitigation: practitioner-grounded persona library. Disclaimer ("this is a simulation built from real data, not a prediction"). Student can flag a session as off.
- **Reinforces narrow paths.** Default library features the same 5 careers. Mitigation: library curation is an ongoing job. Diverse role library at launch (creative trades, healthcare-adjacent, social-impact, technical, entrepreneurial). Add new roles via student request.
- **Student feels patronized by agent voice.** Mitigation: prototype 3-4 voices and test with target segment. Avoid corporate, parental, peppy. Aim: friendly older sibling who has lived through it.
- **Imagination dependency.** Student stops imagining for themselves. Mitigation: debrief questions force student meaning-making, not agent telling.
- **Student tries the experiment, fails, gets discouraged.** Mitigation: experiment design is "smallest version" — high success rate. Follow-up notification asks "how did it go?" with non-judgmental options ("did it / didn't / changed my mind").

## Adoption strategy

- Teacher introduces in one ECG session. Demos Mode 1 with one volunteer student live (anonymized).
- After demo, students use independently.
- Optional 1:1 follow-up: student brings a postcard to a teacher conversation. Teacher's role is to listen, not assess.
- Cross-CCA design: works outside CCA context. Best for ECG / career-curious students. Could be activated by an ECG counsellor, not just CCA teacher.
- Critical: not deployed as a "LEAPS reflection tool" or a "Journey Together replacement." That framing kills it.

## Test plan

- Build Mode 1 (Talk to Future You) only. Use Claude with a tight system prompt for character voice. Mobile web app fine for prototype.
- 6 students recruited from cross-CCA cohort. Mix two profiles: 3 students who can already articulate a future direction, 3 who say they don't know.
- 30-min session: 10-min briefing, 15-min solo simulation, 5-min debrief. 2-week follow-up: did they try the experiment? What happened?
- **Measure:** did the conversation feel like talking to a person? Did the simulation surface a future they hadn't named? Did they leave with a specific next step? Did they actually try it?
- **Falsifiable claim:** at least 4 of 6 students name a possible future they had not previously articulated. At least 3 of 6 commit to a specific next-step experiment within 2 weeks. At follow-up, at least 2 of 3 actually tried it. The lift is highest among the 3 students who started saying "I don't know."

## Connection to the other concepts

- **Pairs naturally with Concept 02 (CCA Wrapped).** Wrapped builds the personal profile from real lived moments (looking backward). Simulator uses that profile to expand possible futures (looking forward). H1 (language for the past) plus H3 (imagination for the future) end-to-end.
- **Complements Concept 01 (Mirror Talk).** A peer mirror naming "you're the kind of person who runs things" can become the seed for a Future Self session ("show me three futures where running things matters"). Simulator can also prepare a student for a richer Mirror Talk by surfacing what they actually want to ask their friends about.
