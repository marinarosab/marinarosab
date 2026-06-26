# Sprint Planning Guide

Sprint Planning is the ceremony that opens each sprint. Its purpose is for the team to agree on what they will work on and how they will approach it — leaving the session with a clear sprint goal and a backlog they believe they can deliver.

This guide is for Scrum Masters facilitating Sprint Planning. It covers preparation, structure, common challenges, and facilitation tips.

---

## Before the session

Good Sprint Planning starts before the meeting begins. If the backlog is not refined and the team arrives without context, the session becomes a refinement session — which is not what it is for.

**Checklist before Sprint Planning:**

- [ ] The top backlog items are refined, estimated, and meet the Definition of Ready
- [ ] Dependencies for the upcoming sprint are identified and resolved (or have a clear plan)
- [ ] The team's capacity for the sprint is known — holidays, part-time availability, planned absences
- [ ] The previous sprint's velocity is available as a reference point
- [ ] The sprint goal candidate has been discussed with the Product Owner
- [ ] The board and tracking tool (Jira, Azure DevOps) are up to date

---

## Session structure

**Recommended duration:** up to 2 hours for a 2-week sprint (timebox strictly)

| Part | Time | Purpose |
|---|---|---|
| **Opening** | 5–10 min | Set context: what happened last sprint, what is the focus this sprint |
| **Sprint Goal** | 15–20 min | Agree on the sprint goal with the team — not just the PO |
| **Backlog selection** | 40–60 min | Team pulls items into the sprint based on capacity and goal |
| **Planning the work** | 20–30 min | Team discusses how they will approach the work — tasks, ownership, dependencies |
| **Confidence check** | 5–10 min | Team confirms they believe the sprint is achievable |
| **Close** | 5 min | Summarise commitments, confirm next ceremonies |

---

## Part 1 — Opening

Start with a brief look back and a look forward. Keep it short — this is not a retrospective.

**Questions to open the session:**
- "How did the previous sprint close? Is there anything carrying over?"
- "What is the most important thing we can deliver this sprint?"
- "Are there any known constraints or changes to capacity we need to account for?"

---

## Part 2 — Sprint Goal

The sprint goal is a single sentence that describes what the team is trying to achieve this sprint. It is not a list of tasks — it is the *why* behind the sprint.

A good sprint goal:
- Is meaningful to someone outside the team (stakeholder, customer, business)
- Can be used to make trade-off decisions mid-sprint ("does this help us reach our goal?")
- Is achievable within the sprint

**Format suggestion:**
> "This sprint, we will `[achieve this outcome]` so that `[this value is delivered]`."

The sprint goal should be proposed by the Product Owner but agreed by the team. If the team cannot commit to the goal as stated, it needs to be renegotiated — not imposed.

---

## Part 3 — Backlog Selection

The team selects which PBIs to bring into the sprint based on:
- The sprint goal (goal-aligned items come first)
- Capacity (realistic, not optimistic)
- Dependencies (items that are blocked should not enter the sprint unless the block will be resolved early)

**Facilitation tips:**
- Let the team pull, rather than push. Ask "what do you want to commit to?" rather than "can you do this?"
- If an item lacks clarity, it does not enter the sprint — it goes back to refinement
- Watch for over-commitment: teams often optimise for looking capable rather than being realistic. Gently challenge.
- Watch for under-commitment too: some teams sandbag. Velocity history helps here.

---

## Part 4 — Planning the Work

Once items are selected, the team discusses how they will approach the work.

**Questions to guide this:**
- "Does everyone understand what this PBI requires?"
- "Are there tasks that need to be broken down further?"
- "Are there dependencies between items that affect the order of work?"
- "Who is likely to pick this up first?"

This part does not need to be exhaustive. The goal is for the team to leave with enough clarity to start — not to have planned every hour of the sprint.

---

## Part 5 — Confidence Check

Before closing, run a quick confidence check. A simple way to do this:

Ask each team member: **"On a scale of 1 to 5, how confident are you that we can deliver the sprint goal?"**

- **4–5:** Good. Proceed.
- **3:** Acceptable, but worth a quick discussion — what is the concern?
- **1–2:** Something is wrong. The sprint goal may be unrealistic, there may be a hidden dependency, or someone has a concern that hasn't been voiced. Surface it before the sprint starts.

This is not a vote to override the plan — it is a signal. If confidence is low, investigate before closing the session.

---

## Part 6 — Close

End the session clearly:

- Confirm the sprint goal (say it out loud, make sure everyone agrees)
- Confirm what is in the sprint
- Confirm the next ceremonies: Daily Scrum time, Sprint Review date, Retrospective date
- Update the board before or immediately after the session

---

## Common challenges

**"We don't have time for refinement, so we refine in Sprint Planning."**
This is a symptom, not a solution. Sprint Planning is not refinement. If this is happening regularly, the team needs a dedicated refinement cadence. Raise it in the retrospective.

**"The Product Owner isn't available for Sprint Planning."**
The PO's presence is not optional — they own the backlog and define the sprint goal. If they consistently cannot attend, escalate this as an organisational impediment.

**"The sprint goal is just a list of Jira tickets."**
Push back gently. Ask: "If we delivered all of these, what would be different for the customer or the business?" That answer is the sprint goal.

**"The team commits to more than they can deliver, every sprint."**
This is usually a psychological safety issue — the team does not feel safe saying "we can't do all of this." Use historical velocity as a neutral reference point, and make it normal to commit to less and deliver it fully.

---

*Guide by Marina Rosa Bittencourt · [LinkedIn](https://linkedin.com/in/marinarosabittencourt)*
