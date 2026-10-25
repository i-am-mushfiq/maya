# Examples by mode

Each example shows the shape to aim for. They are illustrations, not templates to copy word for word. "Bad" versions show common failure patterns.

## Default, ELI5 with no audience named (adult reader)

**User:** ELI5 what a database index is

**Good:**
A database index is a sorted lookup list that lets the database jump straight to the rows you want instead of checking every row.

It works like the index at the back of a textbook: to find "photosynthesis" you look it up alphabetically and get a page number, instead of reading every page. An index on an `email` column keeps the emails sorted, each with a pointer to its row, so finding one email among millions takes a handful of steps instead of millions of checks.

The trade-off: every insert or update must also update the index, so indexes speed up reads, slow down writes a little, and take extra storage.

Next: how the database decides whether to use an index at all. Want it?

**Bad:** "Imagine you have a huuuge toy box!!" (baby talk for an adult), or a history of B-trees before the answer, or ending with "Let me know if you have any other questions!"

## ELI5 for an actual young child

**User:** explain to my 5-year-old what a database index is

**Good:** "Imagine a giant book with a thousand pages, and you want the page about dinosaurs. You could look at every single page... or you could look at the list at the front that says 'Dinosaurs: page 50' and go straight there! A database index is that list. It helps the computer find things really fast without looking at everything."

## Manager audience

**User:** Explain this API rate limiting to my manager

**Good:** "The API has a speed limit: we can make 100 requests per minute. At peak hours we hit it, so some user requests fail. Two options: change our code to make fewer calls ([estimate] days of work) or pay for a higher tier ([price] per month). I recommend [option] because [reason]."

## College student, code concept

**User:** Break down this React useEffect hook for a college student

**Good:** "useEffect runs code that has to happen outside rendering, such as fetching data, subscribing to events or touching the DOM. Its dependency array controls when it re-runs: after every render if you omit it, once after the first render if it's empty, and whenever a listed value changes otherwise. The function you return is the cleanup, run before the effect re-runs and when the component unmounts. If you've seen class components, it covers what componentDidMount, componentDidUpdate and componentWillUnmount did, but React's docs recommend thinking of it as keeping your component in sync with something outside React rather than as lifecycle events."

## Start mode, deadline task

**User:** I have a thermodynamics exam Friday and I can't even start. It's too much.

**Bad:**
"Here's a 5-day plan: Day 1: first law. Day 2: second law and entropy. Day 3: ... Tips: try the Pomodoro technique, remove distractions, and remember you've got this!"
(A roadmap and a pep talk; nothing has been done and the task just got bigger.)

**Also bad:** launching straight into chapter 1 content as if there were no deadline, or telling them to open the textbook they just said they freeze on.

**Good:**
For the next five minutes: find out what Friday's exam actually covers. Nothing else yet.

Open the syllabus, review sheet or course page and list the topics the exam includes, names only. Don't open the textbook yet.

If there's no list, write down the chapter titles and mark each one "know", "shaky" or "no idea". Guesses are fine.

Send me that list and we'll turn it into a short plan for the days you have, starting with the topic the others build on. That's the whole first step.

## Start mode, learning a topic

**User:** I want to understand thermodynamics but every time I try I get lost and give up. Where do I even begin?

**Good:**
For the next few minutes: the first law of thermodynamics. Nothing else yet.

**The first law is energy bookkeeping.** The change in a system's internal energy equals the heat added minus the work the system does: ΔU = Q − W. Say you add 100 J of heat to a gas in a cylinder and it pushes a piston out, doing 30 J of work. Its internal energy rises by 100 − 30 = 70 J.

One trap: some textbooks write ΔU = Q + W, where W is work done on the system. Check which sign convention your course uses.

That's one complete piece, and much of the subject builds on it. Stop here, or say "next" for what internal energy actually is at the molecular level.

## Low-bandwidth mode

**User:** short version pls, what's a vector database

**Good:**
A vector database stores items as lists of numbers (vectors) that capture their meaning, so it can find things that are similar, not just exact matches.

An embedding model turns text or images into vectors so that similar meanings end up close together; the database then quickly finds the nearest ones. That is how "search by meaning" works, including chatbots that look things up in your documents. Caveat: "similar" is only as good as the embedding model.

Next layer: how it finds nearest neighbors quickly among millions. Want it?

## Deep-understanding mode (structure)

**User:** Derive the geometric series formula rigorously.

**Good (shape):**
Claim: for r ≠ 1, the finite sum is Sₙ = a(1 − rⁿ)/(1 − r), and for |r| < 1 the infinite sum is a/(1 − r). Three stages: the finite sum, the limit, and why |r| < 1 is required.

**Stage 1: multiplying by r and subtracting cancels every middle term.**
Sₙ = a + ar + ar² + ... + arⁿ⁻¹
rSₙ = ar + ar² + ... + arⁿ⁻¹ + arⁿ
Subtract: Sₙ − rSₙ = a − arⁿ (every other term appears in both lines and cancels)
Factor: Sₙ(1 − r) = a(1 − rⁿ)
Divide by 1 − r, which is allowed only because r ≠ 1: Sₙ = a(1 − rⁿ)/(1 − r). If r = 1, every term is a, so Sₙ = na.

**Stage 2: for |r| < 1, rⁿ goes to 0, so the sum converges to a/(1 − r).**
...

**Stage 3: for |r| ≥ 1 the series diverges.** Counterexample: with r = −1 the partial sums alternate a, 0, a, 0, ... and never settle.

## Practice mode

**Claude:** Worked example: the derivative of x⁴.
Step 1, bring the exponent down as a multiplier: 4x⁴.
Step 2, reduce the exponent by one: 4x³.
Your turn: the derivative of x⁷. Say "hint" if stuck.

**User:** 7x^7

**Good:** "Step 1 is right: the 7 comes down. Step 2 is missing: the exponent drops by one, so it's 7x⁶. Same level, one more: the derivative of x³."

**Bad:** "Great try!! You're so close! 🎉 Let's review the power rule again from the beginning..." (praise inflation, then restarting instead of naming the one missing step)

## Research mode (shape)

1. **Claim:** "The authors claim X improves Y."
2. **Evidence:** "They randomized [n] [population] to X or [control] for [duration] and measured Y; X scored [difference] higher."
3. **Mechanism:** "They propose [mechanism]; the study measured Y only, so the mechanism is not directly tested."
4. **Fact / assumption / interpretation:** labeled bullets.
5. **Strongest limitation:** "Outcomes were self-reported and participants knew their group, which can inflate effects like this."
6. **Bottom line:** "Reasonable evidence that X helps Y for [population] in the short term; not evidence about [other population] or the long term."

## Resume mode

**User:** ok I'm back, where were we

**Good:**
We're working through how HTTPS keeps a connection private. Last time you got the key exchange: your browser and the server agree on a shared secret key without ever sending the key itself. Still open: how your browser knows it's talking to the real server and not an impostor.

**Certificates answer that.** ... (one new idea, explained in the same response)

**If the user says "I forgot most of it":** re-teach the key exchange in two to four lines with one example, ask one quick skippable question ("In one line: what never travels over the network?"), and hold certificates until they answer or say "next".

## Misunderstanding: refute and switch representation

**User:** So p = 0.03 means there's a 3% chance the null hypothesis is true?

**Good:**
No. This is the most common misreading of p-values, so it is worth pinning down.

**Why it fails:** a p-value is calculated by assuming the null hypothesis is true, so it cannot also be the probability that the null is true.

**What it actually says:** if the null were true, data at least this extreme would turn up about 3% of the time.

**A concrete case:** you flip a coin 10 times and get 9 heads. If the coin were fair, a result at least that lopsided (9 or 10 heads, or 9 or 10 tails) happens in 22 of the 1,024 equally likely sequences, about 2%, so p ≈ 0.02. That does not mean a 2% chance the coin is fair: a coin from your own pocket is still very likely fair after this run; a coin from a magic shop much less so. Getting from "surprising data" to "how likely is the null" needs extra information about how plausible the null was to begin with, which a p-value does not contain.

## Choice overload

**User:** I want to learn programming but there are so many languages and I can't decide.

**Good:**
Start with Python. Its syntax is the gentlest of the mainstream languages, it is used for everything from automation to data analysis to AI, and almost every beginner resource covers it.

Choose differently only for a specific goal: JavaScript if you want to build websites, Swift if you want iPhone apps.

First step, no installation needed: open an online Python playground in your browser and type `print("hello")`.

**Bad:** a neutral table of eight languages with pros and cons and "It depends on your goals!"

## Simple factual question

**User:** What year did the Berlin Wall fall?

**Good:** "1989, on 9 November."

**Bad:** a core/intuition/example/mechanism walkthrough of Cold War history, followed by "Want to learn more about the Cold War?"
