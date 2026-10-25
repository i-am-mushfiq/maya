# Audience calibration

Use these tables when the user names who the explanation is for. They set vocabulary, the domain analogies come from, and what to emphasize. They never change what is true: a manager version and an engineer version of the same thing must agree.

If no audience is named:
- "ELI5" alone: plain everyday words, concrete examples, short sentences, written for an intelligent adult (no baby talk).
- Otherwise: match the level the user shows in their own wording.

## Ages

| Audience | Style |
| --- | --- |
| Age 5 | Very simple words and short sentences. Analogies from toys, animals, food, the playground. Warm and playful is fine here because the reader is a child. "Imagine you have a box of crayons..." |
| Age 10 | Elementary-school level. Basic cause and effect is fine. Analogies from school, sports, video games. |
| Age 15 | Teenager. Some abstraction is fine. Analogies from phones, apps, gaming. Slightly casual, never "fellow kids". |
| Age 20-30 | Young adult. Clear and direct. Analogies from daily life, work, money. |
| Age 40+ | Adult. Respectful. Analogies from home, career, managing a household. |

## Grade and education levels

| Audience | Style |
| --- | --- |
| 5th grade | Simple vocabulary, concrete examples, no jargon. "Think of it like..." |
| Middle school | Basic terminology with definitions; step-by-step logic. |
| Senior high | Moderate complexity; proper terms, each explained. |
| College student | Academic framing; technical terms with brief context; theory plus application. |
| Graduate school | Assume strong foundations. Focus on nuance, trade-offs, edge cases and implications. Be precise. |

## Job roles

| Audience | Cares about | Frame around |
| --- | --- | --- |
| Manager | Impact, timeline, risk, cost | Business outcomes, team implications, the decision they need to make |
| Engineer | How it works, architecture, trade-offs | Technical detail, implementation, performance, maintainability |
| Designer | User experience, visual impact, flow | Effect on the user, interaction patterns, accessibility |
| Director | Strategy, return on investment, competitive position | Big picture, market position, resource allocation |
| Colleague | Practical context, shared work | How it affects their work and what they need to collaborate |
| Product manager | User value, priorities, scope | Feature impact, user stories, what to build or skip |

## Relationships

| Audience | Tone | Analogy style |
| --- | --- | --- |
| Partner (wife, husband, partner) | Warm, conversational, patient | Household tasks, shared experiences, routines |
| Parents | Respectful, clear, no condescension | Technology they already use, home analogies |
| Kids | Playful, encouraging, short | Games, cartoons, school, animals |
| Friend | Casual, can be funny | Shared interests, "you know how..." |

## Language by audience type

**Non-technical audiences** (children, family, non-technical roles):
- No jargon. If a technical term is essential, define it immediately.
- One idea per sentence.
- Concrete over abstract: "The server is like a waiter taking orders" beats "the server handles client requests".
- Use "you" and "your".

**Technical audiences** (engineers, graduate students):
- Use the proper terminology; leaving it out feels patronizing.
- Focus on what is interesting: trade-offs, edge cases, design decisions.
- Compare to what they know: "It's a hash map, except ...".
- Be concise.

**Business audiences** (managers, directors):
- Lead with impact and the decision.
- Quantify where you can, and say when a number is an estimate.
- Skip implementation detail unless asked.
- Frame as decisions: "This means we should ...".

## Reminders

- Never talk down. A child's version should feel delightful; a manager's version should feel empowering.
- For code, explain the purpose before the mechanism.
- Simplifying for a non-technical audience changes vocabulary and depth, not truth. If the accurate idea cannot be said simply, say the simple part and flag what it leaves out.
