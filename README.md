<p align="center">
  <img src="assets/hero.svg" alt="MAYA: Making ADHD Your Ally. Explanations your brain can actually start, follow, and come back to." width="100%">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/made%20for-ADHD%20brains-7B5CFA?style=for-the-badge" alt="Made for ADHD brains">
  <img src="https://img.shields.io/badge/works%20with-Claude-FF6B5B?style=for-the-badge" alt="Works with Claude">
  <img src="https://img.shields.io/badge/dumbing%20down-0%25-2EC4A6?style=for-the-badge" alt="Dumbing down: 0%">
</p>

<p align="center">
  <b>Most explanations are written for a brain with one tab open.<br>MAYA writes for yours.</b>
</p>

## TL;DR (we know you scrolled straight here)

MAYA is an ADHD-friendly explainer for Claude. Ask it about a concept, a chunk of code, an error message, a research paper or a how-to, and you get an explanation you can start, follow, and find your place in again after you drift off.

The facts and the math stay intact, and the full depth is there whenever you ask for it.

**[Install it with one command](#install)**

## Sound familiar?

- You open the topic. You see the wall. You close the tab.
- You ask a yes-or-no question and get a history lesson first.
- You read the same paragraph three times and nothing sticks.
- You get up for water and come back to... what were we doing?
- You ask for help and get a 5-day plan plus a pep talk, when what you needed was one thing to do right now.

Getting stuck has more than one cause. Sometimes the topic is too big, sometimes a piece of background is missing, sometimes the material is unclear, and sometimes you're just tired. MAYA reads which one it is from what you say. A tired brain gets one small piece and a clear place to stop. A missing basic gets taught in a few sentences before the explanation carries on. You won't get a lecture about focus.

## See the difference

<p align="center">
  <img src="assets/before-after.svg" alt="Before and after. A typical AI answer to 'I can't start studying' is a wall of text with a five-day plan and a pep talk. MAYA gives one five-minute step." width="100%">
</p>

<details>
<summary><b>Read the full MAYA answer</b></summary>

<br>

> **You:** I have a thermodynamics exam Friday and I can't even start. It's too much.
>
> **MAYA:** For the next five minutes: find out what Friday's exam actually covers. Nothing else yet.
>
> Open the syllabus, review sheet or course page and list the topics the exam includes, names only. Don't open the textbook yet.
>
> If there's no list, write down the chapter titles and mark each one "know", "shaky" or "no idea". Guesses are fine.
>
> Send me that list and we'll turn it into a short plan for the days you have, starting with the topic the others build on. That's the whole first step.

MAYA still makes a plan. It makes it after the first step, out of what that step turned up.

</details>

## What MAYA does differently

**Your answer comes first.** It's in the opening sentence, so you don't have to dig for it in paragraph four.

**Each chunk holds one idea** and opens with a bold line that states it, which makes skimming work.

**It keeps track of things for you.** A term gets explained where it first shows up, and a symbol gets a quick reminder when it comes back, so you never have to scroll up to remember what "r" was.

**It stops at a natural break.** Each answer ends with at most one suggested next step.

**The hard parts stay in.** Math, code, caveats and the real terminology are all still there, laid out so they're easier to take in. If an analogy helps, MAYA tells you where it stops matching the real thing.

**If you just need the answer, you get it.** Practice and step-by-step coaching only happen when you ask for them.

## It adjusts to what you say

Most questions get MAYA's standard explanation: the core idea in a sentence or two, then an example with real numbers or code, then how it actually works, then the one catch that would trip you up. Some things you say shift it into a different mode:

<p align="center">
  <img src="assets/modes.svg" alt="Six modes: Start, Quick, Deep, Practice, Research and Resume, each triggered by what you say." width="100%">
</p>

There are no settings or commands, and you never pick a mode. If you start out frozen and get curious three messages later, MAYA switches with you.

## Explain it for someone else

Say *"explain this to my manager"*, *"for my mom"* or *"like I'm 10"* and MAYA changes the vocabulary, the examples and what it emphasizes. The facts stay the same, so the manager version and the engineer version of an explanation always agree.

Plain "ELI5" gets everyday words and concrete examples written for an intelligent adult. Baby talk is saved for when the reader really is a kid.

## Things MAYA will never say to you

<p align="center">
  <img src="assets/banned.svg" alt="Banned phrases: Great question! You've got this! Does that make sense? Obviously, it's simple. Just focus harder. Let me know if you have any questions!" width="100%">
</p>

It won't open with a five-day plan or a list of options to choose from, and it won't bring up ADHD unless you do. MAYA works the same way whether or not you've ever mentioned it, so you get the help without the label.

<a id="install"></a>

## Install

**Claude Code on macOS / Linux**

```bash
git clone https://github.com/i-am-mushfiq/maya.git ~/.claude/skills/maya
```

**Claude Code on Windows (PowerShell)**

```powershell
git clone https://github.com/i-am-mushfiq/maya.git "$env:USERPROFILE\.claude\skills\maya"
```

**Claude apps**

Click **Code → Download ZIP** at the top of this page, then upload the ZIP in your Skills settings.

Now go get that water. (Then come back.)

## How to use it

Talk to Claude the way you normally would. Some things to try:

- *"I have a presentation tomorrow and I can't start."*
- *"tl;dr what's an APR"*
- *"Why am I getting this error?"* + paste it in
- *"Explain Kubernetes to my manager"*
- *"Quiz me on photosynthesis"*
- *"ok I'm back, where were we"*

MAYA kicks in when you ask for an explanation, or when you say you're stuck, overloaded or picking back up.

It's built for understanding things. It won't plan your week or track your to-do list.

## Is this legit?

Partly, and here's exactly how much.

Most of the rules come from research on ADHD and on how people learn, such as breaking material into small chunks, cutting interesting details that distract from the point, worked examples, recall practice and specific feedback. A few, like putting the answer first, are design practice that hasn't been tested directly. [`references/evidence.md`](references/evidence.md) rates every rule as Supported, Promising or Heuristic and lists the sources.

Nobody has studied this exact approach, with an AI, for people with ADHD, so MAYA itself hasn't been clinically tested. It's a tool for understanding things. It isn't a treatment.

ADHD also looks different from one person to the next, so MAYA responds to what you actually say instead of working from a checklist.

## What's inside

```
maya/
├── SKILL.md                  # the rules and modes
└── references/
    ├── evidence.md           # the research behind every rule, rated
    ├── examples.md           # good vs. bad answers for each mode
    ├── audiences.md          # explaining for a kid, a manager, an engineer...
    └── topic-playbooks.md    # approaches for math, code, history, papers and more
```

## Help the next brain find it

If MAYA saved you from even one wall of text, give it a star. Stars are how the next person with 47 tabs open finds it.

Got a phrase MAYA should ban, or an idea to make it better? [Open an issue](../../issues).

<br>

<p align="center"><sub>MAYA is a tool for understanding things. It is not medical advice and doesn't replace professional care.</sub></p>
