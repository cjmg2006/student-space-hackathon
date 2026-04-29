# Concepts

Three concepts, each anchored to a specific cluster of hypotheses and a specific wedge insight from the research. They cover the present, past, and future of student self-knowledge.

**Delivery constraint:** all concepts target a mobile phone app for Singapore secondary school students (Sec 1-4).

## The v1 trio

| # | Concept | Temporal anchor | Primary hypotheses | Wedge insight |
|---|---|---|---|---|
| 01 | [Mirror Talk](01-mirror-talk.md) | The present | H4, H6, H9, H10 | Friends shape 40-50% of self-knowledge; trust is person-to-person |
| 02 | [Say It Better](02b-say-it-better.md) **(recommended)** | The past | H1, H5, H11 | The gap is linguistic, not experiential — students lack the language to articulate what they've lived |
| 03 | [Future Self Simulator](03-future-self-simulator.md) | The future | H3, H12 | Students from less-resourced backgrounds can't see futures their family/friends haven't modelled |

## The 02 slot — what changed and why

**What was deprecated:** The original [Concept 02 — CCA Wrapped](02-cca-wrapped.md) was scoped too narrowly. CCA-only and term-end-only. Students live across academic, social, family, and personal domains, day to day. The language gap doesn't wait for term-end.

**What replaced it:** three broader candidates that all fill the same temporal slot (past / language gap) and anchor to the same hypotheses (H1, H5, H11), but go multi-domain and explore different cadences and mechanics.

| Slot | Concept | Cadence | Mechanic | Bet |
|---|---|---|---|---|
| 02a | [Day Logs](02a-day-logs.md) | Daily, ambient | Voice diary + monthly pattern flag | Continuity is the missing variable |
| **02b** | **[Say It Better](02b-say-it-better.md) — recommended** | **Bursty, on-demand** | **Voice rant → 3 articulated versions → library** | **The articulation gap is the language gap; close it directly** |
| 02c | [Threads](02c-threads.md) | Bursty + weekly review | Multi-domain capture clustered by theme | Cross-domain pattern is the throughline students can't see alone |

## Why 02b Say It Better wins as the v1

After deepening 02b, the recommendation rationale sharpens. The original six reasons still hold. The bigger reason now visible:

**02b is self-perception infrastructure, not just an articulation tool.** Naming is the upstream act of identity. Self-perception, self-advocacy, decision-making, identity formation, and emotional literacy are all downstream of self-articulation. The connection map in [02b's deepened doc](02b-say-it-better.md) shows 02b touches every cluster of the research base: Cluster A (self-knowledge), Cluster B (what moves students), Cluster D (trust and consequences), and even Cluster E (the action gap, indirectly). 02a Day Logs is a continuity bet; 02c Threads is a cross-domain bet; 02b is the **upstream** bet.

The original six reasons:

1. **Most direct hit on the wedge insight.** The language gap IS an articulation gap. 02b is built precisely for the moment a student wants to say something true about themselves and can't quite find the words.
2. **Multi-domain by default.** Any rant works: a fight with a sibling, a confusing conversation with a teacher, a moment of pride in CCA, a thought about a future path. Explicit fix for the CCA-only narrowness.
3. **Lightest cognitive load.** No daily streak. No tagging discipline. Used when the student wants language, not on a schedule.
4. **Cleanly differentiated from 01 and 03.** 01 is peer-relational. 03 is AI-future. 02b is solo-past-articulating. Same AI scaffold as 03 but a fundamentally different function (rephrase vs simulate).
5. **Pragmatic for a hackathon timeline.** Voice in, three versions out, save. Easiest to prototype, easiest to test.
6. **Naturally absorbs the application context.** Interviews, personal statements, and scholarship apps are where the language gap bites hardest. Those are explicitly out of scope, but a library of articulated language is what students reach for in those moments anyway. Side effect, not the framing.

**Two new reasons surfaced by the deepening:**

7. **Strongest of the three concepts on Risk 1 (consequence fear).** No human reads. AI doesn't retain. Library is private. Ang Yu Xian's specific failure mode (disclosure leads to escalation) is structurally impossible because nothing is disclosed to anyone in real time. 02b can be a student's first step on a disclosure ladder.
8. **Equity lift, if designed carefully.** The connection map exposes a privilege-gap risk: students with more articulate parents start with more language. But it also exposes the lift opportunity: voice-first, scaffold-low-articulacy prompt design, and library compounding can specifically benefit "Eager but stuck" students who have rich experience but no language. The test plan now explicitly checks that low-articulacy students show comparable or greater lift. If they don't, redesign before deploying.

## Why not 02a (Day Logs)

Strong concept on continuity, but the daily commitment is the wrong ask. Teen drop-off rates on daily-prompt apps are high. It also adds notification load on top of whatever the rest of the app uses. Better as an inspiration for the library architecture in 02b than as the v1 itself.

## Why not 02c (Threads)

Conceptually the richest of the three. Uniquely addresses H2 (outward easier than inward) by explicitly bridging domain to theme. But: it requires sustained multi-domain capture before the value (threads) emerges, which is a heavy lift to test in 4-6 weeks. The cross-domain weaving is the right v2 evolution: once Say It Better has built up a personal library, themes can emerge from it organically. Threads is the future direction, not the v1.

## Hypothesis coverage at a glance (with 02b in the trio)

| Hypothesis | 01 Mirror | 02b Say It Better | 03 Simulator |
|---|---|---|---|
| H1 — Linguistic gap | Secondary | **Primary** | Secondary |
| H2 — Outward easier than inward | — | Supporting (Version 2 = inward bridge) | Mitigated by inward-bridge prompt |
| H3 — Hard to see what's possible | — | Tangential (library expands self-image) | **Primary** |
| H4 — Friends shape self-knowledge | **Primary** | Tangential (library feeds friend conversation) | — |
| H5 — Past launchpad experiences | — | **Primary** | Secondary |
| H6 — Students are relational | **Primary** | Live tension (solo by design; needs human intro) | Highest risk if unmitigated |
| H9 — Trust individuals not institutions | **Primary** | Supporting | Secondary |
| H10 — Fear of consequences | **Primary** | **Primary as mitigation (no human reads)** | Secondary |
| H11 — Agency over surface | Secondary | **Primary** | Secondary |
| H12 — Action gap | — | Tangential (named problems are easier to address) | **Primary** |

The deepened 02b doc now connects to every hypothesis in the research base, with a full evidence map. See [02b's connection map section](02b-say-it-better.md#connection-map) for verbatim research quotes against each hypothesis.

Note: H2 (outward easier than inward) is now partially addressed by 02b (Version 2 = identity claim, the inward-bridge version). If H2 surfaces as more critical than expected, **02c Threads** remains the right swap-in for explicit cross-domain weaving.

## Tension resolution at a glance

| Tension | 01 Mirror | 02b Say It Better | 03 Simulator |
|---|---|---|---|
| Risk 1 — Consequence fear | Friend-group only, async, optional anonymity | On-device voice + library, no retention | Conversation not persisted, only postcard saved |
| Risk 2 — Covertness paradox | Honest framing | Honest framing | Honest framing |
| Risk 3 — Platform vs relationship | Lowest risk | Low risk (solo, light activation) | **Highest risk** — needs teacher activation + 1:1 debrief |
| Risk 4 — Reactive vs reflective muscles | High-frequency, low-stakes | Bursty, on-demand | Curiosity- or fork-triggered |
| Risk 5 — Teacher as guide vs risk | Teacher activates and steps out | Teacher never sees content | Teacher debriefs only on opt-in |
| Risk 6 — Institutional frame | Outside MOE servers | Outside MOE servers | Outside MOE servers |

## Primary segment fit

| Segment | 01 Mirror | 02b Say It Better | 03 Simulator |
|---|---|---|---|
| Eager but stuck (primary) | High | **Highest** | High |
| Disengaged | Medium-high | Medium | Medium-high |
| Self-directed | Medium | High | Medium |
| Capable but apathetic | Low-medium | High (when applying for things) | Medium-high (at fork moments) |

## How they fit together

The three concepts are temporally complementary and could become three modes of one app:

- **Mirror Talk** anchors the present. Friends reflect what's true about you today.
- **Say It Better** anchors the past. Your moments become your own articulated language, ready when you need it.
- **Future Self Simulator** anchors the future. Possible selves become legible and reachable.

Signals can flow between modes:

- A peer mirror ("you're the kind of person who runs things") becomes a saved articulation in Say It Better.
- Articulations in the library seed Future Self Simulator sessions ("you said you like being relied on when no one's watching — let's start there").
- A Future Self session can surface a question the student wants to bring back to friends as the next Mirror Talk question.

## Recommendation

**Build 02b + 03 as the v1 build.** Strongest end-to-end story (language for the past, then imagination for the future). Highest equity lift. Same AI scaffold can power both, reducing prototype build cost.

**Add 01 Mirror Talk as the v1.5** if the team's bet is that relational activation is the load-bearing condition. It's the lightest standalone mechanic and the most testable in a hackathon setting.

If only one concept can be built and tested:

- **Build 03 Simulator** if the team's bet is on possibility expansion.
- **Build 02b Say It Better** if the team's bet is on articulation and the language gap.
- **Build 01 Mirror Talk** if the team's bet is on relational activation.

## Open design questions

1. **Single app with three modes, or three separate experiences?** The recommendation above implies a single app with mode-level entry points. This requires a unified identity and privacy story.
2. **Identity model.** Anonymous, school-account, or self-managed? Decides the privacy story for all three concepts.
3. **AI provider and retention contract.** Who hosts the conversation data? This is the make-or-break for trust on Concepts 02b and 03.
4. **Teacher onboarding script.** How does a teacher introduce this in a CCA or ECG session without making it feel institutional?
5. **Cross-term continuity.** Does the profile (peer mirrors, articulations, simulations) survive into the next year? Without this, all three concepts are one-off experiences.
6. **Friend graph bootstrap.** For Concept 01, how does the friend graph get established without requiring school-issued accounts?

## Files

- [01 Mirror Talk](01-mirror-talk.md) — present, relational
- **[02b Say It Better](02b-say-it-better.md) — past, language (recommended)**
- [02a Day Logs](02a-day-logs.md) — past, alternative (continuity bet)
- [02c Threads](02c-threads.md) — past, alternative (multi-domain weaving bet)
- [02 CCA Wrapped (deprecated)](02-cca-wrapped.md) — earlier scoping, kept for reference
- [03 Future Self Simulator](03-future-self-simulator.md) — future, imagination
- [99 Postcards merged into Future Self](99-postcards-merged-into-future-self.md) — earlier merge note

## Clickable prototypes

Three HTML prototypes demonstrate the core mechanic of each concept. Self-contained, mobile-shaped, no setup required. See [prototypes/README.md](../prototypes/README.md) for the demo flows and [prototypes/NOTES.md](../prototypes/NOTES.md) for design decisions made during the build.

- [01 Mirror Talk prototype](../prototypes/01-mirror-talk.html)
- [02b Say It Better prototype](../prototypes/02b-say-it-better.html)
- [03 Future Self Simulator prototype](../prototypes/03-future-self-simulator.html)

## Journey map

How the three solutions serve four personas across the trigger moments from research. The visual journey map shows the trigger × solution matrix, the three entry doors, four persona pathways, and the cross-solution flow.

- [Visual journey map (HTML)](../prototypes/journey-map.html)
- [Journey map analysis (markdown)](JOURNEY-MAP.md)
