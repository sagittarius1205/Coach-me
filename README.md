# coach-me

**Skills for Gen AI** · English · [繁體中文](README.zh-TW.md) · [简体中文](README.zh-CN.md) · [日本語](README.ja.md)

An AI skill that **fills in the knowledge and abilities you're missing until you can reach your goal on your own**, with verification.

## Why

Many people use grill-me to stress-test a plan without understanding the knowledge behind it. They copy-paste the AI's recommended answers, and the project stalls or heads in the wrong direction.

coach-me and grill-me split the work with no overlap:

| | What it tests | Touches your real plan? |
|---|---|---|
| grill-me | Whether your **decisions** hold up | Yes |
| coach-me | Whether you have the **ability** to make them yourself | No — it verifies with hypothetical side scenarios only |

## Install

Claude Code (or any tool that supports the `SKILL.md` Agent Skills format):

```bash
git clone https://github.com/sagittarius1205/Coach-me ~/.claude/skills/coach-me
```

For other chat AIs, paste the contents of `SKILL.md` into the system prompt or custom instructions.

## Two ways to use it

**1. Standalone** — say "coach me", "teach me until I get it", or "what do I need to learn to…".

- A single skill: goes straight into the loop of diagnose → teach → you do it → verify with a new task.
- A project or large goal: probes your starting level, shrinks the goal to a first version, then gives you a capability map of at most 5 items.

**2. With grill-me** — during a grilling session, if you show any of these "blind-following signals", coach-me offers a short detour in one line and says why:

- adopting the recommended answer as-is, or replying only "OK" / "whatever you said";
- being unable to justify a choice beyond repeating the AI;
- saying you don't understand a term or option.

You can decline; that decision is then marked `⚠ understanding not verified`. If you accept, coach-me teaches only what that one question needs, verifies with a hypothetical scenario, then sends you back to **answer the original question yourself first** before you see the recommended answer.

## Example: reaching JLPT N1

coach-me first probes your level with 1–2 questions. Suppose you've already passed N2:

```
JLPT N1 (v1: N2 → N1 reading & grammar)  0/5

▶ 1. Can tell apart similar N1 grammar (〜ものを／〜ものの)   ← now
□ 2. Can read an N1 essay and state the author's claim
□ 3. Can finish a reading section within the time limit
□ 4. Can recognize common N1 vocabulary (accumulation)
□ 5. Can follow news at natural speed (accumulation)
⏸ Exam date, textbook choice → grill-me
```

- Items 1–3 are taught in the chat, verified with a new task, then one follow-up on a detail of your answer.
- Items 4–5 are accumulation skills: coach-me teaches a practice method and sets a checkpoint (e.g. "16 of 20 random words"). You practice outside the chat and are verified with a fresh sample when you return.
- Listening can't be verified in a text chat, so the report says "not tested".

At the end you get a **progress card**; paste it back next time to continue.

## What it won't do

- Make project decisions for you — that's grill-me's job.
- Give scores like "87% mastery" — it only checks whether you can complete a concrete task on your own.
- Treat a pass in chat as a formal qualification or certificate.
