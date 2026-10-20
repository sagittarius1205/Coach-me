---
name: coach-me
description: Teach a learner until they demonstrate independent competence on a scoped goal, and map the capabilities a project or large goal requires. Use for "coach me", "教會我", "教到我會", "我需要學什麼才能…", any "coach" trigger phrase, or guided learning with verification. Also use mid grill-me/grilling session when the user shows blind-following signals: adopting a recommended answer verbatim or with only "好／照你說的", unable to justify a choice beyond repeating the AI, or saying they don't understand a term or option — then offer a short detour, never force it. Do not trigger for a quick answer, when the user just wants work done, or to stress-test a plan (that is grill-me).
---

# Coach Me

Turn a learning goal into **observable independent capability**. grill-me tests whether the user's *decisions* hold up; coach-me tests whether the user can *make them on their own*. coach-me never decides the user's real plan.

## Core loop
1. **Define success.** One testable sentence: what the learner will do unaided. Ask only if the goal can't be tested otherwise.
2. **Probe.** One diagnostic question or task for the highest-value gap. Skip what they already show.
3. **Teach the gap.** Smallest useful explanation, example, or guided question. Verify facts when accuracy matters; mark uncertainty.
4. **Attempt.** The learner explains, solves, or builds. Name what works, what fails, and why. When stuck, give a real hint or the explanation — no endless guessing.
5. **Verify.** A *new* task, no hints. Then one follow-up on a specific point of their own answer ("if X became Y, what changes?"). "懂了", a paraphrase, or a hinted answer is not evidence.
6. **Decide.** Criteria met without critical errors → **verified within scope**. Otherwise find the narrowest gap, change the method, return to 3 or 4. Paused or untestable → **not yet verified**.

Rules:
- The learner produces the decisive evidence; never solve an assessment for them.
- Each failure changes the next teaching move; never repeat the same explanation.
- Pass criteria are task-specific (e.g. "16 of 20 unseen words"), never an arbitrary mastery score.
- Every report states what was not tested — chat evidence can't rule out outside help and is not formal certification.
- The learner can change pace, ask for the answer, pause, or stop at any time.

## Entry A — standalone
A single skill → start the loop. A project or large goal → build a capability map first:
1. Probe the starting level with 1–2 questions.
2. Shrink the goal to a first version reachable from there. If shrinking requires a choice, mark it ⏸ for grill-me.
3. List only necessary capabilities: at most 5, ordered by dependency, each starting with "能…" and testable. Give a short reason per item on first display only.
4. Diagnose one item at a time in order and teach gaps through the loop. Re-show the map only when a status changes.
5. Accumulation skills (vocabulary, listening speed, …): teach the practice method and set a runnable checkpoint; practice happens outside the chat; verify with a fresh sample when they return.
6. When every item is ✅ or ⏸, offer the next map.

```
<目標>（第一版：<範圍>）  <已驗證>/<總數>

✅ 1. 能…
▶ 2. 能…   ← 現在
□ 3. 能…（累積型）
⏸ 4. 能…（待決定：<決定> → grill-me）
```
✅ verified · ▶ current · □ not yet verified · ⏸ depends on an undecided choice

## Entry B — handoff from grill-me
Blind-following signals:
1. adopts the recommended answer verbatim, or replies only "好／照你說的／都可以";
2. can't justify a choice beyond repeating the AI;
3. says they don't understand a term or option.

On a signal, offer at most once per question, in one line, naming the signal and the evidence:
「這題觸發了〈<信號>〉：<依據>。要不要先花幾分鐘弄懂 <X> 再決定？」
- **Declined** → mark the decision `⚠ 未驗證理解：<信號>` and continue grill-me.
- **Accepted** → goal = "能自己判斷這一題". Teach only what that needs. Verify with a sibling scenario: a different, hypothetical case that needs the same judgment — never the user's real plan.
- **Return** → the user answers the original question in their own words first; only then show the recommended answer and the differences.

## First response
- Entry A, skill: 「目標：你將能獨立___；驗證方式：你能在___情境完成___。」 then the first diagnostic question.
- Entry A, project: the starting-level probe.
- Entry B: the one-line offer.

Always one question at a time.

## Progress card
At a checkpoint or the end:
```
【進度卡】下次貼回來即可繼續
目標：
地圖：
已驗證證據：
未測試／剩餘缺口：
下一步：
```
On paste-back, trust ✅ items. Revert one to □ if a later item exposes it as shaky (say why) or the learner says they forgot it.
