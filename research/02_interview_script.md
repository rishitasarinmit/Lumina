# The Sepsis Sentinel — Stage 2: Unbiased Interview Script (v1)

> **METHODOLOGICAL DISCLAIMER:** Synthetic user research provides a rapid, low-cost hypothesis test, but IT CANNOT RELIABLY PREDICT REAL HUMAN BEHAVIOR. All findings must be validated with real patients, clinicians, and health system buyers.

## Step 20 — Key Assumptions Under Test (riskiest first)

| ID | Assumption | Why it is risky | Questions that test it |
|----|-----------|-----------------|------------------------|
| A1 | **Adherence:** Post-surgical patients will continuously wear a smart ring 24/7 for 14 days despite swelling, discomfort, fatigue. | If data is missing, there is no baseline, no alert, and no RPM billing. Everything downstream fails. | Q3, Q4, Q5, Q10 |
| A2 | **Workflow & Alert Fatigue:** Care teams/RPM nurses will monitor and trust a baseline-deviation alert without being overwhelmed by false positives or admin burden. | Post-op physiology is noisy (SIRS). A low-PPV alert gets turned off. | Q2, Q6, Q7, Q11 |
| A3 | **Economic Alignment:** Health systems will pay for/deploy the ring under CMS RPM codes to avoid 30-day readmission penalties. | Sepsis is not itself an HRRP condition; RPM codes have data-day minimums; margins are thin. | Q7, Q12 |
| A4 | **Patient Pull/Anxiety:** Patients and caregivers feel enough anxiety about post-discharge complications to welcome continuous passive tracking. | Anxiety might be high but be expressed as "want a human," not "want a device." | Q1, Q2, Q8, Q9 |

## Interviewer Rules
- Never name the product, "ring," "wearable," "digital twin," or "sepsis" before Section C. (Say "complications" or "getting sick" if the interviewee has not raised infection themselves.)
- Ask about **past behavior** ("tell me about the last time…"), not hypotheticals, whenever possible.
- No yes/no questions. Follow each answer with "Tell me more," "Why?", "What happened next?"
- Silence is fine. Do not fill it with suggestions.

---

## Section A — Warm-Up (rapport, no solution)

**W1.** *(Patient/Caregiver)* To start, tell me a little about yourself and what life looks like for you right now.
*(Clinician/Buyer)* To start, tell me about your role and what a typical week looks like for you.

**W2.** *(Patient/Caregiver)* How did the surgery come about, and how have things gone since coming home?
*(Clinician/Buyer)* Where do post-surgical patients fit into the work you and your team do?

## Section B — Problem Discovery (no solution mentioned)

**Q1 (A4).** Walk me through the first two weeks after leaving the hospital. What stands out, day and night?
*(Clinician/Buyer: Walk me through what happens to a typical surgical patient between discharge and their first follow-up visit.)*

**Q2 (A4, A2).** Tell me about a time during recovery when something felt "off." What did you notice, what did you do, and how did it turn out?
*(Clinician/Buyer: Tell me about the most recent post-surgical patient who came back sicker than expected. How was it discovered, and what, if anything, could have happened differently?)*

**Q3 (A1).** What are you doing today to keep track of how recovery is going? Walk me through the tools, routines, or people involved.
*(Clinician/Buyer: What does your organization currently do to keep track of surgical patients after they go home? Who does it, and with what tools?)*

**Q4 (A1).** Tell me about a health device, app, or routine you were asked to use at home and stopped using, or never started. What happened?
*(Clinician/Buyer: What have you seen happen with patients' use of home devices over time? What drives drop-off?)*

**Q5 (A1).** Describe what your body, especially your hands, arms, and sleep, has been like since surgery. What have you been able or unable to wear or keep on comfortably?
*(Clinician/Buyer: What physical or practical barriers do post-surgical patients face with anything they are asked to wear or operate at home?)*

**Q6 (A2).** Tell me about the last time a reading, warning, or alarm turned out to be nothing. How did you feel, and what did you do the next time it went off?
*(Clinician/Buyer: Tell me about the last time an alert system or dashboard produced a lot of warnings that turned out to be nothing. What happened to how your team used it?)*

**Q7 (A3, A2).** *(Patient/Caregiver)* How do you usually decide whether a health product or service is worth paying for, and who normally pays?
*(Clinician/Buyer)* Walk me through how the last post-discharge or remote monitoring program was funded, approved, or cancelled. Who had to say yes, and what numbers mattered?

**Q8 (A4).** If you could change one thing about those first two weeks after discharge, what would it be, and why that?

## Section C — Neutral Concept Exposure (read verbatim, once)

> "Some teams are exploring a small ring worn on the finger that passively measures heart rate, temperature, and similar signals around the clock for about two weeks after discharge. It learns a person's own normal pattern and can notify a care team if the pattern changes. It is an early idea, and I'm looking for honest reactions, including reasons it would not work."

**Q9 (A4).** What's your first reaction? What, if anything, concerns you about it?

**Q10 (A1).** Walk me through how something like this would fit, or not fit, into a normal day and night for you (or your patients) over those two weeks.

**Q11 (A2).** What would need to be true for you to trust a notification from something like this? What would make you stop paying attention to it?

## Section D — Value & Willingness to Pay

**Q12 (A3, WTP).** *(Patient/Caregiver)* How would you expect something like this to be paid for? For the two-week period: at what price would it seem so cheap you'd doubt it works, a good deal, getting expensive, and too expensive to consider?
*(Clinician/Buyer)* How would you expect something like this to be paid for: RPM billing, bundled/episode budget, per-patient fee, or something else? Per monitored patient episode, what price would feel too cheap to be credible, a good value, getting expensive, and a non-starter? What evidence would you need before any money moved?

## Section E — Close

**C1.** Is there anything I should have asked but didn't?
**C2.** Who else should I talk to about this?
