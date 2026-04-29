# Concept 01 — Mirror Talk

A mobile ritual where friends ask each other one good question and reflect each other back, asynchronously. Built on the strongest unmet leverage point in the research: peers see things in students that students cannot see in themselves.

## Anchor

**Primary hypotheses:** H4 (friends shape self-knowledge), H6 (students are relational), H9 (trust individuals not institutions), H10 (fear of consequences).

**Secondary:** H1 (linguistic gap).

**Wedge insight (from research):**
> "40-50% of student issues surface through friends rather than direct teacher contact. Friends know themselves in ways they may not know themselves." The SASS dynamic: peers reflect back what students can't yet see. (Apr 21 NYGH research)

Plus: "Students only want to speak with people they're comfortable with. Familiar faces preferred over professional services. Takes time to build trust." (Apr 21)

**The bet:** peers are the highest-trust, highest-signal, most under-utilized source of self-knowledge for teens. Build a tool that turns peer-to-peer conversation into a structured, low-stakes, language-generating ritual. Bypass the institution entirely for the disclosure surface.

## Pitch

The app gives the question. Friends do the rest. Over a term, students accumulate dozens of small, specific mirrors from people they trust. The mirrors become the raw material for who they are becoming.

## Scenario

Aisyah, Sec 3, just finished CCA practice. Her phone pings: "Mirror time. Pick up to 3 friends who saw you today." She taps two: Tasha and Hakim.

The app sends each one a single private question: "What's one thing Aisyah did today that was true to her?" Tasha replies with a 30-second voice note: "She stayed back to help me figure out the cue. I didn't ask. She just saw me struggling and stopped what she was doing." Hakim types: "She's the only person who can disagree with me without it turning into a fight."

An hour later, Aisyah opens the app at home. The two replies surface, slowly. She didn't notice she'd helped Tasha. She'd thought she was just being polite. She didn't see Hakim's framing of how she handles disagreement.

She saves both mirrors to her library. Next morning, the app prompts her: "Owe one back. Who saw something true today that you could mirror?" She picks Tasha and answers: "You let yourself ask for help instead of pretending you had it."

Over a term, Aisyah accumulates 20-30 mirrors. They become her own language for who she is becoming.

## Mechanic

Two functions inside one ritual:

1. **Peer-as-interviewer.** Friends ask you one structured question. Async, private, voice or text. The question library ensures specificity ("what's one thing X did today that was true to her" beats "what is X like").
2. **Peer-as-mirror.** Friends describe back to you something they noticed. Same async, same private, same one-thing-at-a-time discipline.

The system maintains a question library, schedules pairings, manages a soft reciprocity loop ("you owe a mirror back"), and stores mirrors privately for the receiver.

**Three design constraints that make it work:**

- **Async, never sync.** No live-on-the-spot moments. Friend chooses when to reply, receiver reads alone.
- **One thing per round.** No survey, no essay, no list. One question, one answer.
- **Anonymous-by-default mode.** Optional anonymity for sensitive mirrors. If on, receiver sees the mirror but not who sent it. Recovers signal that would otherwise self-censor.

## How it connects to each hypothesis

- **H4 (friends shape self-knowledge):** the mechanism IS friends shaping self-knowledge. Direct hit on the strongest finding in the research.
- **H6 (students are relational):** activation is the relationship. Platform is invisible.
- **H9 (trust individuals not institutions):** trusted friends mediate, not platforms or roles. Aisyah trusts Tasha. She doesn't trust the school's wellbeing initiative.
- **H10 (fear of consequences):** closed friend group, async, optional anonymity, never reaches a teacher.
- **H1 (linguistic gap, secondary):** the question library is the language scaffold. "What's true to her" is a frame the student didn't have.

## How it resolves each tension

- **Risk 1 (consequence fear, critical):** all data closed-friend-group, opt-in. No teacher access. No school server.
- **Risk 2 (covertness paradox):** honest framing. "Ask your friends what they saw." Reflection is the byproduct.
- **Risk 3 (platform vs relationship):** pure peer-to-peer. Closest of the three concepts to the Risk 3 ideal.
- **Risk 4 (reactive vs reflective muscles):** low-stakes, high-frequency. Builds the muscle without forcing it.
- **Risk 5 (teacher as guide vs risk):** teachers don't see content. Their role is to model the format once and step out.
- **Risk 6 (institutional frame):** student-installed app. Data layer is private to the friend group.

## Mobile UX — key moments

- **Asking screen.** One question, big text, single tap to answer. Voice, text, or photo + sentence.
- **Receiving a mirror.** Full-screen, single mirror at a time. Slow reveal animation. Receiver chooses pace.
- **Mirror library.** Scrollable, search-by-friend, copy-to-message. Private to receiver.
- **Pairing.** Opt-in suggestions ("These three friends saw you today"), never assignment.
- **Notification design.** Gentle. "A mirror is waiting" not "respond now."
- **Privacy default.** Mirrors private to receiver. To share, copy-paste manually. No "post to feed" button anywhere.

## Failure modes

- **Cruel or flat mirror.** Receiver can mute or block. No public consequence. No retaliation surface.
- **Zero engagement.** Student gets no mirrors back. Mitigation: app monitors silently and offers "want to start with an AI mirror to see the format?" only if usage is low.
- **Performative niceness.** "Nice things to say about your friend" mode. Mitigation: question library is specific. Vague answers prompt "say more about a moment."
- **Screenshot leaks.** Trust breaks if mirrors circulate. Mitigation: disable screenshots in-app. Watermark sender ID. Some leakage is unavoidable; design for graceful failure.
- **Pair drift.** Same friends always picked, others isolated. Mitigation: rotation suggestions surface friends who saw the student today but haven't been picked recently.

## Adoption strategy

- One CCA, 15-30 students, friends with each other.
- Teacher introduces in one session. Demos one round live (anonymized). Then steps out.
- After 60% adoption in the cohort, format spreads via friend invites to adjacent groups.
- LEAPS / CCE staff are NOT informed. The data is not part of the LEAPS reflection requirement.

## Test plan

- 4-6 students from one CCA, friends with each other. 4 weeks. Wizard-of-Oz the question scheduling via group chat or simple form.
- **Measure:** did mirrors continue past week 2 without facilitator nudges? Can students name 2 things friends saw in them they hadn't noticed? Did any mirrors get shared outside the group (red flag — social currency drift)?
- **Falsifiable claim:** by week 4, at least 4 of 6 students name a specific thing a peer saw in them that changed how they think about themselves. At least 3 of 6 ask to keep using it past week 4.
