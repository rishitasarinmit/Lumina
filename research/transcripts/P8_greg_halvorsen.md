# Interview Transcript — P8: Greg Halvorsen

| Field | Value |
|---|---|
| Persona ID | P8 |
| Name | Greg Halvorsen, CPA, MBA |
| Segment | Economic buyer: CFO, 3-hospital regional nonprofit system (Toledo region, Ohio; ~650 beds, ~$1.4B revenue, 1.2% operating margin) |
| Adoption position | Late majority (economic skeptic) |
| Script | 02_interview_script.md v1, Clinician/Buyer variant |
| Format | 30-minute video call |

> **SYNTHETIC TRANSCRIPT — cannot predict real human behavior; validate with real users**

---

## Section A — Warm-Up

**Interviewer (W1):** To start, tell me about your role and what a typical week looks like for you.

**Greg:** I'm the CFO for a three-hospital nonprofit system, about 650 beds and roughly $1.4 billion in revenue. We ran a 1.2% operating margin last fiscal year, which means one bad quarter of labor costs or one payer dispute puts us underwater. A typical week is a Monday flash report on volumes and contract labor, two or three meetings with service line leaders about their P&Ls, a payer contracting call, and some kind of board or finance committee prep. Nursing labor is up about 22% since 2021, so honestly a third of my week is some version of "how do we staff this without agency." I have a goal of getting us to 3% without layoffs, and every conversation gets filtered through that.

**Interviewer:** Tell me more about that filter.

**Greg:** It means I ask the same question about everything: what does it cost, when does it pay back, and whose budget does the payback land in. A lot of things in healthcare save money for somebody, just not for us. I came out of Big Four audit, so I'm allergic to projections that don't tie to our own ledger.

**Interviewer (W2):** Where do post-surgical patients fit into the work you and your team do?

**Greg:** I see them through the surgical service line P&Ls, not individually. Surgery is where our margin comes from, frankly; orthopedics and cardiac subsidize a lot of the rest of the system. Post-discharge is where that margin leaks. A readmission on a fee-for-service commercial patient is, bluntly, more revenue, but on a Medicare episode or an HRRP condition it's a cost or a penalty. So my team tracks readmissions, episode spend, and post-acute utilization by service line, and I get a quarterly review from quality and finance together.

---

## Section B — Problem Discovery

**Interviewer (Q1):** Walk me through what happens to a typical surgical patient between discharge and their first follow-up visit.

**Greg:** I'll give you the finance view, because I'm not the clinical person. They get discharged with instructions, most go home, a smaller share go to a SNF or get home health. Our care-transitions nurses, we have two FTEs, call the higher-risk ones within 48 to 72 hours, and a call vendor handles automated outreach to the rest. The follow-up visit is usually 10 to 14 days out for surgery. In between, what I see in the data is basically silence until something shows up, either a phone call to the surgeon's office, an ED visit, or a readmission.

**Interviewer:** What do you see in the data when something shows up?

**Greg:** Mostly I see the ED visit and the readmission and the cost attached. I don't see the three days before it where the patient felt lousy. The clinical team would tell you infections, wound issues, dehydration, and cardiac stuff are the big buckets. I couldn't tell you the split off the top of my head, and I wouldn't want to guess.

**Interviewer (Q2):** Tell me about the most recent post-surgical patient who came back sicker than expected. How was it discovered, and what, if anything, could have happened differently?

**Greg:** I don't get patient stories, I get variance reports. The most recent one that crossed my desk was a quarterly TEAM episode review where our major bowel episodes came in over target, and when we dug in, a handful of readmissions drove most of the overage. A couple of them were readmitted through the ED with infections and ended up in the ICU, and one ICU stay on an episode can wipe out the margin on a dozen other episodes. Our surgeon chief's view was that at least some of those patients had called the office and been told to watch it. Could something have been different? Maybe, but I've been told "earlier detection" is the answer to about fifteen things, and nobody ever shows me which of those readmissions were actually preventable versus just going to happen.

**Interviewer:** What happened next?

**Greg:** We asked quality to do a chart review on the preventable fraction. That's still in progress, which tells you something about how much bandwidth quality has. In the meantime, the fix everyone reached for was "add another call," which is more nurse time.

**Interviewer (Q3):** What does your organization currently do to keep track of surgical patients after they go home? Who does it, and with what tools?

**Greg:** Three things. Two care-transitions nurse FTEs, loaded cost around $130,000 each. A post-discharge call vendor, automated calls with escalation to a live nurse, which runs us a low six figures a year. And a small RPM program, mostly heart failure and some hypertension, with blood pressure cuffs and scales, run out of the employed medical group. On the analytics side, Strata and Epic for financials and Vizient for benchmarking our readmission and complication rates against peers.

**Interviewer:** Tell me more about the RPM program.

**Greg:** It's roughly break-even, and I watch it closely because it could easily tip the wrong way. It only works because the patients are chronic, they stay on it for months, and we can hit the data-day requirements and bill the monthly management time. The nurse staffing to do the 20-minute management calls is the biggest cost line. If enrollment dips or patients stop transmitting, it goes negative quickly.

**Interviewer (Q4):** What have you seen happen with patients' use of home devices over time? What drives drop-off?

**Greg:** I see it as revenue leakage. In our RPM program, a meaningful share of enrolled patients in any given month don't transmit enough days to bill the device code, and historically that threshold was 16 days in a 30-day period. I've heard CMS has added a shorter-duration option, something like 2 to 15 days, for 2026, but I haven't had my revenue cycle team walk me through the rates or the rules yet, so I wouldn't bank on it. What I know is low adherence equals no revenue, and the staff time to chase non-transmitters is not billable. The clinical folks say drop-off is worst in the first month and among the oldest patients, which is exactly who we'd care about most.

**Interviewer (Q5):** What physical or practical barriers do post-surgical patients face with anything they are asked to wear or operate at home?

**Greg:** You'd get a better answer from a nurse. From where I sit: they're older, a lot of our Medicare population is rural, broadband is patchy in parts of our catchment, and they're tired and on pain meds. Anything that needs charging, pairing, or a smartphone is a support call waiting to happen, and support calls are staff time. I'd also flag device logistics, meaning shipping, retrieval, lost units, cleaning. On our cuffs we write off a certain number of devices a year that just never come back.

**Interviewer (Q6):** Tell me about the last time an alert system or dashboard produced a lot of warnings that turned out to be nothing. What happened to how your team used it?

**Greg:** I cut three digital health contracts in the last two years, and at least two fit that description. One was a patient-reported-outcomes platform that fired alerts on every out-of-range survey answer; the nurses spent hours clearing flags, and within six months they'd stopped looking at it except for audits. The vendor kept sending me engagement dashboards when what I asked for was avoided utilization. The other was a predictive analytics tool that generated risk scores nobody acted on. Both sold outcomes and delivered dashboards. For me, a false alarm is unreimbursed nurse time at best, and at worst it's an avoidable ED visit that shows up as cost in an episode or shared-savings arrangement.

**Interviewer:** Tell me more about the ED visit piece.

**Greg:** In fee-for-service, an ED visit is revenue, so a false alarm that sends someone to the ED isn't a loss on paper. Under TEAM or our MSSP ACO arrangement, it counts against us. So an alerting tool can actually make my numbers worse in exactly the contracts where I'm supposed to be saving money, if it pushes people to the ED who didn't need to be there.

**Interviewer (Q7):** Walk me through how the last post-discharge or remote monitoring program was funded, approved, or cancelled. Who had to say yes, and what numbers mattered?

**Greg:** The most recent cancellation was the outcomes platform I mentioned. It came in through the CNO's office as a one-year pilot, funded out of an innovation budget, under $250,000, so it was within my authority, and I signed it on the condition that we'd see measurable readmission reduction by renewal. At renewal they had enrollment numbers and satisfaction scores, no readmission delta we could attribute, and the nursing time to run it was never in the original budget. I declined the renewal. What mattered was total cost including our labor, the readmission change against a comparison group, and which contract the savings landed in. Anything over $1 million goes to the board, and the board wants a payback period, preferably inside 12 months, and anything that fits in the July fiscal year budget cycle.

**Interviewer:** What would have made you renew it?

**Greg:** A documented reduction in readmissions or episode spend on our own data, net of our nursing cost. Or a payer paying for it. Or the vendor taking risk, where they get paid out of savings. None of those were on the table.

**Interviewer (Q8):** If you could change one thing about those first two weeks after discharge, what would it be, and why that?

**Greg:** I'd want to know earlier which patients are heading for trouble, so the nurses I already have spend their time on the right 10% instead of calling everyone. My constraint isn't a lack of ideas, it's a lack of nurse hours. So the change I'd want is better targeting, not more activity. If something added work for my nurses, even if it was clinically good, it'd be a hard sell to me right now.

---

## Section C — Neutral Concept Exposure

**Interviewer (reading verbatim):** "Some teams are exploring a small ring worn on the finger that passively measures heart rate, temperature, and similar signals around the clock for about two weeks after discharge. It learns a person's own normal pattern and can notify a care team if the pattern changes. It is an early idea, and I'm looking for honest reactions, including reasons it would not work."

**Interviewer (Q9):** What's your first reaction? What, if anything, concerns you about it?

**Greg:** First reaction is "where's the money." If this is pitched as avoiding readmission penalties, I'd point out that sepsis isn't an HRRP condition, and neither is colectomy. HRRP only hits us on a handful of conditions and procedures, including CABG and elective hip and knee, and the penalty is capped at 3% of base DRG payments; we're paying about 0.6%. A readmission for infection after a CABG or a joint would count, but that's a slice of a slice. Second, two weeks doesn't fit the RPM billing model I know, which historically needed 16 days of data in a 30-day period, and even if the new shorter option helps, it's a smaller payment and you still need a billing practitioner and staff time. Third, cybersecurity: another device vendor with patient data in the cloud is another breach exposure and another security review. The idea itself, catching deterioration early, I don't have a problem with. I just don't see the funding mechanism yet.

**Interviewer:** Tell me more about where you would look for the money.

**Greg:** Honestly, TEAM is the only place it clearly lands. We're in the mandatory model as of January, and it covers episodes like major bowel procedures, CABG, joints, and spinal fusion, with 30 days post-discharge on our tab. CJR is over and BPCI Advanced wound down at the end of last year, so TEAM is where episode risk lives now. Second would be our ACO attributed lives and possibly Medicare Advantage, if an MA plan would pay for it or share the savings; most of our MA contracts are basically fee-for-service with worse terms, so an avoided readmission there isn't obviously a gain for us. For commercial fee-for-service, avoiding a readmission can actually cost us revenue. I'm not proud of that, but it's how the math works.

**Interviewer (Q10):** Walk me through how something like this would fit, or not fit, into a normal day and night for your patients and team over those two weeks.

**Greg:** For the patients, I'll defer to clinical, but I'd expect the same adherence drop-off we see on our cuffs, maybe worse after surgery with swelling and fatigue. For my team, the question is who watches it at 2 a.m. My care-transitions nurses work days. If notifications come in overnight, either I'm staffing a 24/7 monitoring function, which is several FTEs I don't have, or the vendor is, and then I'm paying for that. Then there's enrollment at discharge, shipping or handing out devices, getting them back, and documentation in Epic. If it doesn't live in Epic, it won't get used. Each of those steps is either my labor or your fee, and I'd want every one of them priced out before I believe any ROI number.

**Interviewer:** What would it displace, if anything?

**Greg:** That's the right question. If it let me stop calling low-risk patients and redirect the two FTEs, or reduce the call vendor contract, that's a hard-dollar offset I can put in a model. If it's purely additive, it's just a new cost center.

**Interviewer (Q11):** What would need to be true for you to trust a notification from something like this? What would make you stop paying attention to it?

**Greg:** I don't personally trust or distrust the notification, the nurses and surgeons do, and if they stop trusting it the program is dead regardless of what I think. What I'd need is the positive predictive value and the alert volume per 100 patients, measured on surgical patients like ours, not healthy volunteers or ICU patients. I'd want to know how many alerts turn into a phone call, how many into an ED visit, and how many of those ED visits were actually needed. What would make me stop paying attention is simple: if a pilot shows more ED visits without fewer readmissions or lower episode spend, I cancel it. I don't care whether it's AI or a rules engine, I care about the results on our data.

---

## Section D — Value & Willingness to Pay

**Interviewer (Q12):** How would you expect something like this to be paid for: RPM billing, bundled/episode budget, per-patient fee, or something else? Per monitored patient episode, what price would feel too cheap to be credible, a good value, getting expensive, and a non-starter? What evidence would you need before any money moved?

**Greg:** It would come out of the episode budget, meaning TEAM and ACO, not RPM. I'd assume RPM billing covers a fraction at best for a 14-day episode; I'm not going to build a business case on a code my revenue cycle people haven't confirmed, and I'd have to net out the 99457/99458 nurse time needed to bill management anyway. So I'd only deploy it on TEAM and attributed-ACO patients, which for us is maybe 1,000 to 1,200 episodes a year. Here's my back-of-envelope: a complicated readmission on an episode costs us roughly $15,000 to $25,000 in episode spend. At $200 an episode across 1,100 patients, that's about $220,000, plus maybe one nurse FTE for alert triage at $130,000, so call it $350,000 all-in. I'd have to avoid something like 15 to 25 readmissions a year, net of any extra ED visits, just to break even, and I'd want to see at least 1.5x before I'd call it worth doing.

**Interviewer:** And the four price points?

**Greg:** Per monitored patient episode, all-in including the device, logistics, and any vendor monitoring: under about $50 I'd assume it's a consumer ring with a dashboard bolted on and nobody clinical behind it, so too cheap to be credible. Good value is around $100 to $150. Getting expensive is around $250. A non-starter is $400 and up, because at that price I need to prevent a lot of readmissions that I'm not convinced are preventable. Those numbers assume the vendor handles overnight monitoring; if my nurses have to do it, knock $75 or so off every number.

**Interviewer:** What evidence would you need before any money moved?

**Greg:** Three things, in order. One, a retrospective look using our own data: how many of our TEAM episode readmissions over the last two years were infection or deterioration that a signal could have plausibly caught, and what they cost. Two, published or at least credible peer-reviewed data on alert performance in post-surgical patients. Three, a prospective pilot on a few hundred patients with a matched comparison group, measured on readmissions, ED visits, and total episode spend, with our finance team doing the analysis, not yours. And frankly, my preferred structure is that I pay nothing upfront: a risk-share where the vendor gets a percentage of documented episode savings above an agreed baseline. If a vendor won't take any risk, that tells me how confident they are in their own numbers.

---

## Section E — Close

**Interviewer (C1):** Is there anything I should have asked but didn't?

**Greg:** You didn't ask about implementation cost, and that's where these things die. IT integration into Epic, a security review, legal and BAA work, training, and the device logistics can easily be six figures before the first patient is enrolled, and those costs are never in the vendor's ROI slide. You also didn't ask what I'd stop doing to pay for this, and in a 1.2% margin year that's the real question. And I'd ask whether the surgical global period creates any billing problems with RPM; my revenue cycle team has raised questions on that before and I don't know the answer.

**Interviewer (C2):** Who else should I talk to about this?

**Greg:** My VP of revenue cycle, for whether any of the RPM codes realistically apply to a two-week post-surgical episode. Our director of care transitions, because it's her nurses who would carry the workload. Our chief of surgery, who will tell you whether surgeons want to be notified at all. Our CISO, because they can kill this in a security review. And one of our Medicare Advantage plans' medical directors, because if a payer would fund this, the whole conversation changes for me.

**Interviewer:** Thank you, Greg. This was really helpful.

**Greg:** Sure. Send me something built on my numbers, not national averages, and I'll look at it. No promises beyond that.

---

*End of transcript. SYNTHETIC TRANSCRIPT — cannot predict real human behavior; validate with real users.*
