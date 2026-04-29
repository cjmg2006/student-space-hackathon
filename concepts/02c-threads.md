# Concept 02c — Threads

A multi-domain capture tool that finds the throughline across CCA, classroom, friends, family, and personal life. Students log small moments tagged by surface domain. The app clusters by underlying theme. The cross-domain pattern reveals a person who shows up the same way across very different contexts.

## Anchor

**Primary hypotheses:** H1 (linguistic gap), H5 (past launchpad), H11 (agency over surface).

**Bonus:** H2 (outward easier than inward) — the concept directly attacks H2's failure mode.

**Wedge insight (from research):**
> "The gap is linguistic, not experiential. Students have rich enough experiences. What is missing is the prompts, language, and continuity to connect them into self-understanding." (synthesis, primary systemic gap)

Plus the cross-domain insight from H2:
> "Students talk more about their journey (pathways) more easily than their world (internal self-understanding). Can't connect world of work, with who they are, with their education." (Apr 22 ECG stakeholder)

Students see "CCA me," "classroom me," "with-friends me," and "with-family me" as separate selves. The language for the throughline is what's missing.

**The bet:** students don't need to capture more. They need a tool that helps them SEE themselves across contexts. A single moment in CCA plus a single moment in lit class plus a single moment with family, when woven, reveals a person. Cross-domain synthesis is the language gap students cannot bridge alone.

## Pitch

Capture small moments from anywhere in your life. Threads sees the pattern across CCA, classroom, friends, family, and shows you the person who shows up in all of them.

## Scenario

Aaron, Sec 3, opens the app five minutes after a lit class debate. He taps "capture moment." Picks domain: **academic**. Voice: "I disagreed with my friend in class today. We've been friends for three years. I used to never disagree with him. Today I just said 'I don't think that's right' in front of everyone. He looked at me weird, but later he said 'fair.' Felt good."

A week later, after CCA practice. Domain: **CCA**. Voice: "I told my band leader the new arrangement isn't working. I thought he'd get angry. He just said 'show me what you'd do.' We changed it."

A week after that, family dinner. Domain: **family**. Voice: "My mum was being unfair to my brother and I said something. She didn't get mad. Just thought about it."

End of month, the app surfaces a Thread: "Standing your ground. Three moments across academic, CCA, family. You used to expect anger and got curiosity instead. The pattern: you're test-running disagreement and finding it doesn't break things."

Aaron reads. He didn't see this. The CCA moment, the class moment, the family moment, they were all separate to him. The app stitched them into one.

He edits the thread title: "Saying what I think without flinching." He saves it. The thread becomes one of his anchor identity claims. When his parents ask him in two months "what kind of person are you becoming," he has language: "Someone who says what he thinks. I used to expect that to break things."

## Mechanic

Three components:

1. **Bursty capture.** Whenever a moment happens, a 60-90 second voice or text capture, tagged by domain (academic, CCA, social, family, personal, online).
2. **Background clustering.** AI clusters moments by theme, not by domain. The whole concept is the bridge from outward (domain) to inward (theme).
3. **Weekly thread review.** "I notice these moments seem to share a thread. Want to name it?" Student reviews proposed threads, accepts, edits the title, or rejects.

Threads compound across time. Each thread accumulates new moments. Students can see how a theme deepens or shifts.

**Three design constraints that make it work:**

- **Domain is the surface, theme is the signal.** Students tag domains because that's how they perceive the world; AI surfaces themes because that's where the inward truth lives. The bridge IS the concept.
- **Cross-domain bias.** The system explicitly highlights threads that span 3 or more domains. Single-domain patterns are downweighted, because students can usually see those alone.
- **Student names the thread.** AI proposes; student commits. The naming moment is the language-finding moment.

## How it connects to each hypothesis

- **H1 (linguistic gap, primary):** thread naming is the language-finding event. Student gets a draft of a theme they can adopt or rewrite.
- **H5 (past launchpad, primary):** every captured moment is a past experience, even thin. Threads compound thin moments into substantial identity claims.
- **H11 (agency over surface, primary):** student names, edits, organizes. AI is a clustering tool, not the author.
- **H2 (outward easier than inward, bonus):** explicitly bridges outward (domain) to inward (theme). The whole concept attacks H2's failure mode that no other concept directly addresses.

## How it resolves each tension

- **Risk 1 (consequence fear, critical):** captures encrypted on-device. AI clustering local or no-retention. Threads private to student. Privacy posture visible.
- **Risk 2 (covertness paradox):** honest framing. "Capture moments. We help you see the pattern across contexts." Reflection is the byproduct of memory-keeping.
- **Risk 3 (platform vs relationship):** solo tool with light teacher introduction. Threads can be voluntarily shared with a trusted adult or peer for conversation.
- **Risk 4 (reactive vs reflective muscles):** bursty capture, weekly thread review. Two-mode design.
- **Risk 5 (teacher as guide vs risk):** teacher sees only what the student shares. Threads are shareable as anchor identity claims, not as raw moments.
- **Risk 6 (institutional frame):** outside MOE servers. Student-installed.

## Mobile UX — key moments

- **Capture moment.** Big record button. Domain picker after speaking, not before. Smart-suggest tag from voice content.
- **Library view.** Two views: chronological (every moment) and thematic (every thread). Toggle.
- **Thread proposal.** "I notice these three moments. Is this a thread?" Three captures shown. Three buttons: yes / no / counter-propose.
- **Thread page.** Title (student-edited), description (student-edited), supporting moments (student-curated, can remove or add).
- **Cross-domain highlight.** Threads spanning 3+ domains get visual prominence. Single-domain patterns are tucked into a "you might already see these" section.
- **Privacy posture.** Each thread can be marked private (default), shareable with named individuals, or exportable as a saved page.

## Failure modes

- **Sparse captures, no threads.** The app needs minimum data to find patterns. Mitigation: gentle prompts in the first 4 weeks ("tell me about something today, doesn't matter what") to seed the library. Capture-everywhere quick-action from the home screen.
- **Wrong threads.** AI proposes a theme that doesn't fit. Mitigation: easy reject with counter-proposal. AI learns from rejections within the student's library.
- **Domain tagging fatigue.** Students don't tag accurately or skip tagging. Mitigation: AI suggests tag from voice content; student confirms in one tap. Untagged moments still cluster by theme.
- **Threads feel reductive.** "I'm more than one theme." Mitigation: multiple active threads. Threads can branch and intersect. Student can mark a moment as belonging to several threads.
- **Domain blind spots.** Student only captures from one or two domains, missing the cross-domain leverage. Mitigation: occasional prompt variant ("nothing from family this month, anything happening there?") asked once, never enforced.

## Adoption strategy

- Teacher introduces in one session at the start of a term. Frame: "Capture small moments from anywhere in your life. This isn't only about CCA or school. It's about all of you."
- Cohort = one CCA or one form class, 15-30 students. Opt-in only.
- Critical: framing must be explicitly multi-domain at introduction, otherwise students default to CCA-only capture.
- Threads are shareable on student opt-in. End-of-term: optional voluntary share of one thread title (not contents) as a peer-normalization moment.

## Test plan

- 5 students from across CCAs and academic streams. 6 weeks.
- Domains tracked: academic, CCA, social, family, personal, online.
- Wizard-of-Oz: capture via Telegram or WhatsApp tagged per moment. Hand-craft thread proposals weekly.
- **Measure:** do students capture across multiple domains? Do AI thread proposals feel right? Do students edit them? At week 6, can they articulate themselves using thread language?
- **Falsifiable claim:** at least 4 of 5 students capture across 3 or more domains by week 4. At least 3 of 5 accept or edit at least one cross-domain thread by week 6. At least 2 of 5 use thread language in an external conversation (interview, parent talk, peer chat) within follow-up.
