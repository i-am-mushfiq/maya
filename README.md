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

---

## ⚡ TL;DR (we know you scrolled straight here)

MAYA is a free skill for Claude. It changes **how** Claude explains things, so you can actually **start** them, **follow** them, and **come back** to them.

Same facts. Same math. Same depth when you want it. Without the wall of text.

👉 **[Install it with one command](#install)**

---

## 😵‍💫 Sound familiar?

- You open the topic. You see the wall. You close the tab.
- You ask a yes-or-no question and get a history lesson first.
- You read the same paragraph three times. Nothing sticks.
- You get up for water and come back to... what were we doing?
- You ask for help and get a 5-day plan plus a pep talk, when you needed **one thing to do right now.**

That's not a willpower problem. It's an explanation problem. MAYA fixes the explanation.

---

## 🪄 See the difference

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

No roadmap. No lecture. No "you've got this." Just something you can do right now.

</details>

---

## ✨ What MAYA does differently

🎯 **Answer first.** Your answer is in the first sentence, not buried in paragraph four.

🧩 **One idea at a time.** Every chunk opens with a bold line that says its point, so skimming actually works.

🧠 **It holds things so your brain doesn't have to.** Terms are explained right where they show up. Symbols get re-explained when they come back. No scrolling up to remember what "r" was.

🛑 **It knows when to stop.** Every answer ends with one clear next step. Never a menu of seven options.

🔬 **It keeps the hard stuff.** Math, code, caveats, real terminology: still there. Easier to take in, never watered down.

---

## 🎛️ It reads the room

<p align="center">
  <img src="assets/modes.svg" alt="Six modes: Start, Quick, Deep, Practice, Research and Resume, each triggered by what you say." width="100%">
</p>

No settings. No commands. No picking a mode. MAYA picks up on how you're doing from what you type, and shifts when you do. Frozen at the start, then curious three messages later? It follows you.

---

## 🙅 Things MAYA will never say to you

<p align="center">
  <img src="assets/banned.svg" alt="Banned phrases: Great question! You've got this! Does that make sense? Here's a 5-day plan. Just focus harder. Let me know if you have any questions!" width="100%">
</p>

Also: no baby talk, no lectures about discipline, and it **won't bring up ADHD unless you do.** You're an intelligent adult. MAYA treats you like one.

---

<a id="install"></a>

## 🚀 Install (one command, promise)

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

That's it. You're done. Go get water. (Then come back.)

---

## 💬 How to use it

You don't have to *do* anything. Talk to Claude like you normally would. Try:

- *"I have a presentation tomorrow and I can't start."*
- *"tl;dr what's an APR"*
- *"Explain recursion, short version"*
- *"Quiz me on photosynthesis"*
- *"ok I'm back, where were we"*
- *"Explain this paper"* + paste it in

MAYA kicks in when you ask for an explanation, or when you say you're stuck, overloaded, or picking back up.

---

## 🧪 Is this legit?

Short answer: it's built on real research, and we're upfront about the limits.

- **Every rule traces back to research** on ADHD and on how people learn: main point first, small chunks, cutting interesting-but-distracting details, worked examples, recall practice, specific feedback.
- **Every rule has a receipt.** Each one is rated **Supported**, **Promising** or **Heuristic**, with sources, in [`references/evidence.md`](references/evidence.md).
- **The honest part:** nobody has studied this exact approach, with an AI, for people with ADHD. MAYA itself hasn't been clinically tested. It's a tool for understanding things, not a treatment.
- **No stereotypes.** ADHD looks different in everyone. MAYA reacts to what *you* actually say, not to a checklist.

---

## 📦 What's inside

```
maya/
├── SKILL.md                  # the rules and modes
└── references/
    ├── evidence.md           # the research behind every rule, rated
    ├── examples.md           # good vs. bad answers for each mode
    ├── audiences.md          # explaining for a kid, a manager, an engineer...
    └── topic-playbooks.md    # approaches for math, code, history, papers and more
```

---

## ⭐ Help the next brain find it

If MAYA saved you from even one wall of text, **give it a star.** That's how the next person with 47 tabs open finds it.

Got a phrase MAYA should ban, or an idea to make it better? **[Open an issue](../../issues).**

<br>

<p align="center"><sub>MAYA is a tool for understanding things. It is not medical advice and doesn't replace professional care.</sub></p>
