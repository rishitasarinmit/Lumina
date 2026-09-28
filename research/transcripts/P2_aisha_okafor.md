# Synthetic Interview Transcript — P2

| Field | Value |
|---|---|
| Persona ID | P2 |
| Name | Dr. Aisha Okafor, MD, MPH |
| Segment | Buyer/Champion — Chief Medical Information Officer & VP Digital Health, 12-hospital academic health system (Philadelphia metro) |
| Adoption position | Early adopter |
| Script version | Stage 2 Unbiased Interview Script (v1), Clinician/Buyer variants |
| Format | 45-minute video call, back-to-back meeting slot |

> **SYNTHETIC TRANSCRIPT — cannot predict real human behavior; validate with real users**

---

## Section A — Warm-Up

**Interviewer:** Thanks for making time. To start, tell me about your role and what a typical week looks like for you.

**Dr. Okafor:** Sure — and I should warn you, I have a hard stop at the top of the hour because I'm going straight into steering committee. I'm the CMIO and I also carry the VP of Digital Health title, so half my week is classic informatics: Epic optimization, clinical decision support governance, build requests, alert burden. The other half is running our virtual care portfolio, which is Hospital-at-Home plus remote monitoring for heart failure and COPD. A typical week is probably thirty-plus meetings. Tuesday mornings are the digital health steering committee, which is where everything I'm responsible for either lives or dies. And somewhere in there I'm answering vendor emails, most of which I don't answer, honestly.

**Interviewer:** Where do post-surgical patients fit into the work you and your team do?

**Dr. Okafor:** Right now, mostly they don't, and that's kind of the problem. Our virtual care programs grew up around medical patients — CHF, COPD — because that's where the readmission penalties and the evidence were. Surgical patients belong to the surgical departments, and once they leave the building they're essentially in the surgeons' offices' hands until the post-op visit. I've been saying for about a year that post-surgical is the next frontier for us, but I don't have a surgical champion who's fully bought in. So it's more of an aspiration on my slide deck than an operating program.

**Interviewer:** Tell me more about not having a champion.

**Dr. Okafor:** Our Chair of Surgery and I have a good working relationship — we're collegial, we sit on the same committees. But he's lukewarm on anything that sounds like more inbound messages to his residents and APPs. His position, roughly, is "my patients get a phone call and they know to go to the ED." And to be fair, he's not entirely wrong that the data for doing more is thinner in surgery than in heart failure.

---

## Section B — Problem Discovery

**Interviewer:** Walk me through what happens to a typical surgical patient between discharge and their first follow-up visit.

**Dr. Okafor:** They go home with a discharge packet that's ten pages long and that nobody reads fully, and a follow-up appointment roughly ten to fourteen days out. Somewhere in the first 48 hours they're supposed to get a post-discharge phone call — a nurse or sometimes an MA running a script. Completion rates on those calls are, let's say, not what we report to the board aspirationally. After that call, it's a black hole. I genuinely use that phrase internally. We don't know anything until the patient calls the clinic, shows up in one of our EDs, or shows up in somebody else's ED, which is the worst version because then we find out late through claims or an HIE notification.

**Interviewer:** What happens in the cases where they call the clinic?

**Dr. Okafor:** It goes into a phone-note queue or a patient-portal message pool. It gets triaged by whoever is covering, which may be a nurse or an APP who's also doing a clinic. If it's "my incision is red," they might ask for a photo. If it's "I feel crummy and I have a fever," the default advice is often "go to the ED," which is defensible medicolegally but not great care or great cost. There's no structured data flowing, it's all free text.

**Interviewer:** Tell me about the most recent post-surgical patient who came back sicker than expected. How was it discovered, and what, if anything, could have happened differently?

**Dr. Okafor:** I'll keep it de-identified and a little vague. Earlier this year we had a readmission review — a gentleman in his seventies after a bowel resection, discharged on day five, looked fine. He called the clinic line on about day eight saying he was tired and not eating much, and the note says he was advised to push fluids and call back if worse. He came into one of our community EDs roughly 36 hours later, hypotensive, with an intra-abdominal abscess, and spent time in the ICU. When we reviewed it, the thing that struck me was that in hindsight there was a trajectory — the family said he'd been off for a couple of days — but nobody had anything objective. We had a phone note with the word "tired" in it.

**Interviewer:** What could have happened differently?

**Dr. Okafor:** Honestly, the easiest thing is a better phone triage protocol — someone asks about temperature, heart rate if they have a pulse ox, urine output, and escalates to a same-day visit instead of "call back if worse." That's cheap, and I'd want to fix it regardless of any technology. Whether objective data would have caught it earlier, I think probably, but I'm cautious about saying that, because hindsight makes every trajectory look obvious. It's personal for me too — the reason I went into informatics is that I watched a patient on a general ward die of sepsis that was recognized about twelve hours too late, and every signal was in the chart. So I know that "the data existed" and "someone acted on it" are two very different things.

**Interviewer:** What does your organization currently do to keep track of surgical patients after they go home? Who does it, and with what tools?

**Dr. Okafor:** For surgical patients specifically: the 48-hour call, the portal, and the follow-up visit. Some service lines, like our joint replacement program, use a text-message check-in pathway through a patient engagement vendor — it asks about pain and gives PT reminders, it's not physiologic. Inpatient, we run the Epic sepsis model, but that stops at the door; it does nothing post-discharge. On the medical side we have a real RPM program — Bluetooth scales and blood pressure cuffs for heart failure, a vendor platform that our RPM nurses monitor from a central hub, TytoCare kits in a couple of pilots. So we have the infrastructure muscle, we just haven't pointed it at surgery.

**Interviewer:** Tell me more about how the RPM hub is staffed.

**Dr. Okafor:** It's a small team of RNs, business hours with some extended coverage, and after-hours escalations roll to an on-call arrangement that is — let's say it's a recurring agenda item. They're carrying a caseload that I think is at the top of what's safe. If I added a surgical population tomorrow without adding FTEs, the nurse manager would, correctly, come to my office and close the door.

**Interviewer:** What have you seen happen with patients' use of home devices over time? What drives drop-off?

**Dr. Okafor:** In our CHF program we're at roughly sixty percent adherence at thirty days, meaning sixty percent of enrolled patients are still sending readings on enough days to matter. That's actually not bad for the industry, and it's still not good enough. The drop-off drivers are pretty consistent: the device becomes a chore, the patient feels better and stops seeing the point, connectivity issues — especially older patients with no Wi-Fi or a phone that won't pair — and, frankly, nobody ever calls them about their readings, so they figure nobody's looking.

**Interviewer:** You said "nobody's looking." Tell me more.

**Dr. Okafor:** That's the lesson from our 2022 pilot, and it's a sore spot. We did a wrist-wearable pilot with a vendor — I won't name them — continuous vitals for a medical population. The data went to a vendor dashboard that was not in Epic, and there was never a clear answer to "who looks at this at 2 a.m." So effectively nobody did. The data never reached a clinician in a meaningful way. Meanwhile patients stopped charging the devices within a week or two, and because nobody called them when they stopped, the silence itself was never an alert. We shut it down after a few months with no outcome data. I had to present that at steering committee. That's the thing I never want to do again.

**Interviewer:** What physical or practical barriers do post-surgical patients face with anything they are asked to wear or operate at home?

**Dr. Okafor:** Surgical patients are a different animal from CHF patients. They're in pain, they're on opioids at least early on, they're fatigued, they may have limited mobility — joint patients can't easily get up, abdominal patients don't want to bend. Many are older, some have tremor or arthritis or neuropathy. Anything that requires fine motor steps, pairing, charging, remembering to do a measurement — that's all friction at exactly the moment they have the least bandwidth. And the caregiver ends up being the actual operator of the technology, which we almost never design for. I'd also flag fluid shifts and edema post-op, and IV sites and blood draws on hands and arms in the hospital — I don't know what that does to anything worn on the body, but I'd want someone to have studied it.

**Interviewer:** Tell me about the last time an alert system or dashboard produced a lot of warnings that turned out to be nothing. What happened to how your team used it?

**Dr. Okafor:** The Epic Sepsis Model is my cautionary tale, and it's everyone's in informatics. When the external validation came out a few years ago showing it performed much worse than advertised — poor discrimination, it missed a lot of cases and fired on a lot of patients who weren't septic — that confirmed what our nurses already felt. When we turned it on originally, with vendor-default thresholds, the firing rate was high and the nurses started treating it like wallpaper. We had to retune thresholds locally, change who gets the alert, and bundle it with a nurse screen before it goes to a physician. Even now, I'd describe trust in it as grudging. The meta-lesson is that everybody quotes AUROC and nobody on the unit cares about AUROC — they care about how many times they get interrupted for nothing.

**Interviewer:** What happened next, after the retuning?

**Dr. Okafor:** Alert volume came down to something tolerable, and response times on the alerts that did fire improved, at least in our internal monitoring. But we gave up some sensitivity to get there, and that's a trade-off I'm not entirely comfortable with. It also taught me that the threshold isn't a technical decision, it's a staffing decision.

**Interviewer:** Walk me through how the last post-discharge or remote monitoring program was funded, approved, or cancelled. Who had to say yes, and what numbers mattered?

**Dr. Okafor:** The CHF RPM program is the best example. It started as a pilot I could approve within my own authority — I can sign off on pilots up to about a quarter million dollars — and it went through digital health steering committee for clinical, IT security, and privacy review. Getting a BAA signed and a security review done took months by itself. To scale it, I needed the CFO and ultimately board-level visibility, and the numbers that mattered were thirty-day readmission rates for heart failure — which is an HRRP condition, so there's a direct penalty story — plus RPM billing revenue under the standard RPM codes — the 99453/99454 setup and device codes and the 99457/99458 management-time codes —, and the fully loaded nurse cost. Our CFO's question was essentially "does billing plus avoided penalty plus avoided readmission cost exceed staffing plus devices." It roughly did, barely, and a lot of that depended on adherence, because if a patient doesn't transmit enough days you can't bill the device code for that month. We also have an integrated health plan, so for our own members an avoided readmission is real money to us, not just to a payer somewhere — that helped.

**Interviewer:** And cancelled — the 2022 pilot?

**Dr. Okafor:** Cancelled mostly on non-numbers. There was no outcome to show, the nurses didn't want it, and the cost per enrolled patient was high relative to nothing. Nobody fought to keep it. That's what pilotitis looks like at the end — not a dramatic failure, just nobody defending it.

**Interviewer:** If you could change one thing about those first two weeks after discharge, what would it be, and why that?

**Dr. Okafor:** Ownership. I would want every surgical patient to have a named team that's accountable for them from the day they leave until the follow-up visit, with a defined escalation path — who calls the patient, who decides on a same-day visit, when it goes to the surgeon. Tools come second. If I had ownership plus some objective signal, great. But if I had to choose one thing, it's a human accountable for the black hole. Everything I've watched fail, failed because no one owned it.

---

## Section C — Neutral Concept Exposure

**Interviewer:** I'm going to read a short description, then ask for your reactions.

> "Some teams are exploring a small ring worn on the finger that passively measures heart rate, temperature, and similar signals around the clock for about two weeks after discharge. It learns a person's own normal pattern and can notify a care team if the pattern changes. It is an early idea, and I'm looking for honest reactions, including reasons it would not work."

**Interviewer:** What's your first reaction? What, if anything, concerns you about it?

**Dr. Okafor:** My honest first reaction is: interesting, and I've heard versions of this pitch before. The passive part is appealing — no pairing a cuff, no stepping on a scale — because that addresses one of the drop-off drivers I described. Consumer rings already do resting heart rate, HRV, and skin temperature trends reasonably well for sleep and wellness; the question is whether that translates to a clinical-grade signal in a sick, post-op, older population. Concerns, in rough order: first, "learns a person's normal" — normal when? They've just had surgery; their baseline in the first days home is not their normal, it's inflammation, pain, opioids, and deconditioning. Second, PPG accuracy across skin tones — the pulse oximetry literature is a real equity issue and I will ask for subgroup performance data, full stop. Third, where does the notification go, and who owns it at 2 a.m.? That's the question that killed my last pilot.

**Interviewer:** Tell me more about the baseline concern.

**Dr. Okafor:** Post-op physiology is noisy. Tachycardia, low-grade temperature, poor sleep — those happen in plenty of patients who are recovering just fine. If the system starts learning on day one or two at home, it's learning an abnormal state. If it needs several days to establish a baseline, you may already be past the window where some complications show up. Unless you somehow have pre-operative data, which most patients won't. I'd want to know how you handle that, and not in a pitch-deck way — in a methods-section way.

**Interviewer:** Walk me through how something like this would fit, or not fit, into a normal day and night for your patients over those two weeks.

**Dr. Okafor:** For the patient, in theory it fits better than most things — put it on, leave it on. In practice: who sizes it? Fingers swell after surgery and after days of IV fluids, so a ring sized at discharge may be tight on day two and loose on day ten. Who charges it, and how often — because every time it comes off to charge, that's a chance it doesn't go back on. Where does it sync — a patient's phone? Many of our older patients, especially in some of our lower-income zip codes, don't have a smartphone that'll reliably do that. That's an equity problem I'd need solved, probably with a hub or cellular option. On our side: someone has to enroll the patient before discharge, which means it has to be in a discharge workflow that already exists, ideally triggered from an Epic order. And the data has to land in Epic, not in a separate vendor portal. If it's another login, I already know how the story ends.

**Interviewer:** What about the night?

**Dr. Okafor:** Night is where the value is and where the operational problem is. Overnight data is probably the cleanest signal — patient at rest — and a lot of deterioration gets noticed in the morning when it started overnight. But my RPM hub doesn't have robust overnight clinical coverage. So either the alert waits until 7 a.m., which undercuts the premise, or it goes to an on-call clinician who doesn't know the patient, or it goes to the patient with instructions, which pushes risk and anxiety onto them. Somebody has to design that, and a device company alone can't.

**Interviewer:** What would need to be true for you to trust a notification from something like this? What would make you stop paying attention to it?

**Dr. Okafor:** To trust it: prospective validation, in a post-surgical population that looks like mine, ideally published or at least peer-reviewable. I want positive predictive value and alerts per 100 patients per day — not AUROC. Show me PPV and nurse workload per 100 patients. I want lead time versus current detection — how many hours earlier than the ED visit or the phone call. I want performance broken out by skin tone, age, and procedure type. FDA clearance for whatever claim they're making, and a clear intended-use statement, because a "wellness" ring that sends clinical alerts is a regulatory problem I don't want. And a tiered escalation protocol — what's a nurse call versus a same-day visit versus an ED referral, with a named owner at each tier.

**Interviewer:** And what would make you stop paying attention?

**Dr. Okafor:** The same things that made us stop paying attention to the sepsis model at launch. If the first month produces a lot of alerts where the nurse calls and the patient says "I'm fine, I just didn't sleep," that's it — the team will mentally down-weight it, and by month three it's wallpaper. Also silent data gaps: if the ring isn't transmitting and nobody knows, it's worse than nothing, because it creates false reassurance and potential liability. And if the alert is a black-box "risk score went up" with no explanation of which signal changed, clinicians won't act on it. I'd honestly rather have fewer, more specific alerts and miss some things than a sensitive system nobody listens to — although, again, that's a trade-off I'd want my surgeons to weigh in on.

---

## Section D — Value & Willingness to Pay

**Interviewer:** How would you expect something like this to be paid for: RPM billing, bundled/episode budget, per-patient fee, or something else? Per monitored patient episode, what price would feel too cheap to be credible, a good value, getting expensive, and a non-starter? What evidence would you need before any money moved?

**Dr. Okafor:** Payment first, because I think vendors often get this wrong. RPM billing is not a clean fit for a fourteen-day episode. The traditional device-supply code required sixteen days of data in a thirty-day period, which a two-week episode doesn't meet, and even with CMS's newer shorter-duration device and ten-minute management codes, the reimbursement is modest, and it depends on adherence and on clinical staff time actually being logged. Then there's the interaction with the surgical global period, and whether commercial payers follow Medicare — I'd need my revenue cycle team to tell me how that works for us, and I wouldn't trust a vendor's slide on it. On readmissions: sepsis isn't itself an HRRP condition, though CABG and hip and knee replacement are, and we're watching the CMS TEAM episode model for surgical episodes closely — that's probably the more compelling frame. So realistically, I'd see this funded out of an episode or value-based budget, plus our health plan for our own members, with RPM billing as a partial offset, not the business case.

**Interviewer:** And the price points, per monitored patient episode?

**Dr. Okafor:** I'll give you ranges, with a big caveat: it depends entirely on whether you're selling me a device and a dashboard, or a device plus monitoring staff plus Epic integration. Device and software only, where my nurses carry the load: under about $75 per episode, I'd assume it's a consumer ring with a clinical sticker on it, or that you'll be out of business before my contract ends. A good value is maybe $150 to $250 per episode. It starts getting expensive around $350 to $400, because by then the math gets hard to defend against a readmission rate that's in the low double digits for most of these procedures and the incremental nurse FTEs I'd need. Above about $500 to $600, it's a non-starter for device-only. If a vendor includes a staffed monitoring service with 24/7 clinical triage and Epic integration, I'd tolerate higher numbers — maybe the "expensive" line moves to $600 or $700 — because then you're actually solving my staffing problem. But please don't read these numbers as a commitment; they're my gut, and our CFO would discount them further.

**Interviewer:** What evidence would you need before any money moved?

**Dr. Okafor:** For a pilot inside my authority: a peer-reviewed or at least credible prospective dataset in post-surgical patients, FDA status clear, subgroup accuracy data, a signed BAA with clear data residency and a prohibition on secondary use or model training on our patients' data without a separate agreement, and an Epic integration plan that my team has actually reviewed. And the pilot has to be designed like a study from day one — a defined population, a comparison group, prespecified outcomes: thirty-day readmissions, ED visits, time to detection, PPV, nurse minutes per patient, adherence by day. If a vendor won't agree to prespecified success criteria and a kill criterion, I won't run it. To go enterprise-wide, the CFO needs to see a net financial effect in our own data, not the vendor's, and my realistic procurement timeline even for a pilot is six to nine months.

---

## Section E — Close

**Interviewer:** Is there anything I should have asked but didn't?

**Dr. Okafor:** You didn't ask about what happens when the ring is right and the patient still doesn't come in. Detection is half of it; the other half is whether you can get a post-op patient seen same-day without sending them to the ED — that's an access problem, not a technology problem, and our surgical clinics don't have much slack. You also didn't ask about liability: once we're collecting continuous data, we're arguably on the hook for having seen it, and our risk management people will ask that before I do. And I'd ask how you think about caregivers, because they're going to be the real operators for a lot of these patients.

**Interviewer:** Who else should I talk to about this?

**Dr. Okafor:** Our RPM nurse manager — she'll tell you in five minutes whether this is feasible for her team, and she has veto power in practice even if not on paper. The Chair of Surgery, or better, a colorectal or cardiac surgeon who's lukewarm, because if you can't convince the skeptics, you don't have a program. Our CFO or someone in finance who handles value-based contracts and episode models. Risk management and our privacy officer. And patients — especially older patients from our lower-income neighborhoods, not just the tech-savvy ones who'll volunteer for anything. I'd also ask peers at other systems that have tried post-surgical RPM what happened, because I suspect several of them quietly shut it down. Okay — I have to jump to steering committee. Send me something in writing and I'll look at it, but I'll be honest, it goes in the same pile as everyone else until I see outcome data.

---

*End of transcript. SYNTHETIC TRANSCRIPT — cannot predict real human behavior; validate with real users.*
