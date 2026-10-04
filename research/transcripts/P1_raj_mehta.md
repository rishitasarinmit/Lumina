# Interview Transcript — P1: Raj Mehta

| Field | Value |
|---|---|
| Persona ID | P1 |
| Name | Raj Mehta |
| Segment | Patient (post-laparoscopic sigmoid colectomy, day 5 post-discharge) |
| Adoption position | Innovator |
| Script version | Stage 2 Interview Script v1 (Patient/Caregiver variants) |
| Format | Video call, ~45 min; interviewee at home in suburban Austin, TX |

> **SYNTHETIC TRANSCRIPT — cannot predict real human behavior; validate with real users**

---

## Section A — Warm-Up

**Interviewer:** Thanks for making time, Raj. To start, tell me a little about yourself and what life looks like for you right now.

**Raj:** Sure. I'm 67, retired about three years ago after thirty-five years doing distributed systems at a semiconductor company, mostly infrastructure and monitoring. My wife Priya still works part-time, so right now she's the one driving me around and handling most of the cooking. Normally I'm on the bike fifty-plus miles a week, but at the moment my big achievement is walking around the cul-de-sac three times a day, like the discharge sheet says. Honestly the hardest part is being bored and not trusting my own body. I'm used to having a dashboard for everything, and my body right now is a system I don't have good observability into.

**Interviewer:** How did the surgery come about, and how have things gone since coming home?

**Raj:** Diverticulitis. I had two bad flares, the second one got me a CT and a course of antibiotics, and the surgeon said the math favored an elective sigmoid colectomy before a third one turned into an emergency. So I did it laparoscopically at the academic center, about 35 minutes from here. The surgery itself went fine, and I was home after three nights. Since then it's been mostly okay: sore, tired, eating small meals, the incisions look clean. But there was one night that rattled me, which I assume we'll get to.

**Interviewer:** We will. Tell me a bit more about "mostly okay."

**Raj:** Pain is manageable, I stopped the oxycodone on day two at home and I'm on Tylenol. Bowels are working, which, if you've had this surgery, you know is the thing everyone asks about. What's not okay is the fatigue. I'll sit down after a walk and just be out for an hour. I don't know if that's normal or if it's the first sign of something.

---

## Section B — Problem Discovery

**Interviewer:** Walk me through the first two weeks after leaving the hospital. I know you're five days in, so walk me through what you've had so far. What stands out, day and night?

**Raj:** Days are fine, actually. I have structure: walk, eat, log my temperature, walk, nap, message the surgical PA if I have a question. Nights are the problem. I'm sleeping in the recliner half the time because getting in and out of bed hurts, and I wake up every couple of hours. And at 3 a.m. every twinge becomes a hypothesis. The discharge instructions say call if you have fever over 101, worsening belly pain, and so on, but those are binary thresholds on single readings. I spent my career telling people single-sample thresholds are how you get paged for garbage and miss the real incident.

**Interviewer:** Tell me more about that.

**Raj:** Well, the real failure mode in production is a slow drift that stays under every alarm threshold until it falls off a cliff. That's what I'm afraid of with the anastomosis, the place where they reconnected the colon. A leak, from what I've read, doesn't necessarily announce itself on day one with a 103 fever. It might be a low-grade fever, a heart rate that creeps up, feeling a bit worse each day. And "feeling worse" is exactly what I'm bad at judging because I feel bad anyway. My fear isn't the dramatic scenario; it's that I tough it out for a day and a half because none of the individual numbers crossed a line.

**Interviewer:** Tell me about a time during recovery when something felt "off." What did you notice, what did you do, and how did it turn out?

**Raj:** Day three at home. I woke at 3 a.m. with chills, took my temperature, and it was 100.2. Under the 101 threshold, but I don't run fevers, ever. So I sat in the kitchen for about two hours reading about anastomotic leaks, the typical timeline, the symptoms, a couple of surgical forums. I rechecked at 4 and it was 100.0, and I took Tylenol, which of course then contaminates the next reading. By 5:30 I decided it was probably okay and went back to sleep. It was fine. By noon I was 98.9.

**Interviewer:** What happened next?

**Raj:** I sent a MyChart message in the morning to the PA, Jessica, who by now knows me by name, probably not in a good way. She said low-grade temps can be normal in the first week, keep monitoring, call if it goes over 101 or I get belly pain. Which was reasonable. But here's the part that bugs me: when I looked at my Oura data afterward, my resting heart rate that night was up about 12 beats over my baseline, and the temperature deviation was clearly elevated for the night before too. So the data "knew something" was going on, maybe hours earlier. Nobody on the care team could see it, and even I couldn't interpret it, because I don't know what a normal post-op deviation looks like. Was 12 bpm a warning or just what healing looks like?

**Interviewer:** Why do you think you didn't call the surgeon's line that night?

**Raj:** Partly because I was under the threshold they gave me, and I follow protocols when I understand them. Partly ego, I suppose; I didn't want to be the guy who calls the on-call resident at 3 a.m. for 100.2. And partly because I honestly didn't know what I'd tell them. "My ring says my heart rate is up" isn't something I expect a resident to take seriously at 3 a.m. If I'd had a number that I knew was meaningful, I would have called in a heartbeat. No pun intended.

**Interviewer:** What are you doing today to keep track of how recovery is going? Walk me through the tools, routines, or people involved.

**Raj:** I have a Google Sheet. Temperature three times a day with a digital oral thermometer, plus any extra readings if I feel off, and I note whether I've had Tylenol in the last four hours. Pulse ox readings a couple times a day with a fingertip oximeter. Pain score, what I ate, bowel movements, walks and step counts. Then passively, I've got my Oura ring, which gives me overnight resting heart rate, HRV and temperature deviation, and the Apple Watch for daytime heart rate and steps. I pull the Oura data in manually right now; I've been meaning to hook up their API. The people side is Priya, who notices if I look gray, and MyChart messages to the surgical team.

**Interviewer:** Tell me more about how you use the spreadsheet day to day.

**Raj:** I chart it. I have a little trend line for temperature and resting HR with the pre-surgery baseline as a reference band. It's crude; the Oura baseline from before surgery isn't really valid anymore because everything's shifted. And to be fair, I'm aware this isn't normal patient behavior. My surgical PA thinks it's funny. Nobody on the team has asked to see it.

**Interviewer:** Tell me about a health device, app, or routine you were asked to use at home and stopped using, or never started. What happened?

**Raj:** The incentive spirometer, the plastic breathing thing they send you home with. I used it religiously in the hospital and for the first two days home, and now, honestly, I'm maybe doing it once a day instead of every hour. No feedback loop; I can't tell whether it's doing anything. The other one is the hospital's own app. They gave me a sheet with a QR code for some post-op education app, and I opened it once, saw it was basically PDFs and videos, and never went back. The contrast is that I've worn the Oura for over two years straight without missing more than a day or two. The difference is that the Oura gives me something back every morning.

**Interviewer:** Describe what your body, especially your hands, arms, and sleep, has been like since surgery. What have you been able or unable to wear or keep on comfortably?

**Raj:** Hands were puffy in the hospital; they pumped a lot of IV fluid into me, and I had an IV in my left hand and an arterial line in the right wrist during surgery. They made me take the ring and the watch off for the OR, obviously, and I didn't get the ring back on until the day I came home because my fingers were too swollen. So I've got a gap of about four days in my data, right when you'd most want it. The watch I wear during the day but I've stopped wearing it at night because I'm charging it then and the band was pressing on the IV bruise. Sleep is broken, like I said, recliner and bed, waking every two hours.

**Interviewer:** And the ring now?

**Raj:** It's back on, a bit tight in the mornings still, but fine. I've moved it to a different finger once. If I'd had a smaller hand or more swelling, I don't think I could have worn it for the first several days. That's worth knowing if you're designing something.

**Interviewer:** Tell me about the last time a reading, warning, or alarm turned out to be nothing. How did you feel, and what did you do the next time it went off?

**Raj:** The Apple Watch has done the "high heart rate" notification a couple of times over the years, usually when I'm sitting after a hard ride and it hasn't figured out I was riding. And Oura had a stretch where it told me my "readiness" was bad and I might be getting sick, and I was fine, I'd just had two glasses of wine. The reaction is always the same: I go look at the raw data and figure out why. What annoys me is when I can't do that, when it's a black box that says "pay attention" and doesn't show me what triggered it or what the threshold was. After a few of those, I stop reading the summary card and just look at the raw charts myself.

**Interviewer:** What about the hospital's alarms while you were admitted?

**Raj:** Oh, the pulse ox alarm went off constantly when I was asleep, because the probe slipped. Nurses would come in, silence it, and leave. I noticed by the second night they were slower to come in. I don't blame them. That's what happens when an alarm cries wolf.

**Interviewer:** How do you usually decide whether a health product or service is worth paying for, and who normally pays?

**Raj:** For gadgets, I pay myself; I've got a mental cap of around 400 bucks for something I'm curious about, like the Oura or the Watch. My test is: does it give me a signal I can't get otherwise, and can I get at the raw data? I will pay for a subscription if it's small, like the Oura membership, but I resent subscriptions that are just a paywall on my own data. For medical stuff, I'm on Medicare with a Medigap Plan G, so my expectation is that if a doctor orders it, it's covered, and I basically pay the Part B deductible and nothing else. I haven't had to think very hard about medical bills since I went on Plan G, frankly.

**Interviewer:** Tell me more about the difference between those two buckets.

**Raj:** If it's something I'm choosing for myself, I'm the buyer and I'm pretty price-insensitive within that range. If it's something my surgeon wants me to use as part of care, then it's their tool and I'd expect them or Medicare to pay. I'd be a little suspicious of a hospital asking me to pay out of pocket for something they're using to monitor me. That starts to feel like they're offloading their costs onto me.

**Interviewer:** If you could change one thing about those first two weeks after discharge, what would it be, and why that?

**Raj:** I'd want somebody on the care team to be able to see my trend data and tell me what normal looks like. Not a person calling me every day, I don't need hand-holding, but someone who can look at a chart and say, "Your heart rate is up, but that's typical for day three," or, "That trend worries us, come in." What I lacked that night wasn't data; I had plenty of data. I lacked a reference for what normal recovery looks like and a way to get that in front of someone qualified without it being a 3 a.m. phone call. Closing that loop is the thing.

**Interviewer:** Why that over anything else?

**Raj:** Because everything else is solvable by me. I can manage pain, the walks, the diet. I can't solve "is this deviation clinically meaningful," because I'm not a surgeon and there's no public baseline for how a post-colectomy 67-year-old's resting heart rate should behave. That's the missing piece.

---

## Section C — Neutral Concept Exposure

**Interviewer:** I'm going to read a short description now, and then I'd like your honest reaction.

> "Some teams are exploring a small ring worn on the finger that passively measures heart rate, temperature, and similar signals around the clock for about two weeks after discharge. It learns a person's own normal pattern and can notify a care team if the pattern changes. It is an early idea, and I'm looking for honest reactions, including reasons it would not work."

**Interviewer:** What's your first reaction? What, if anything, concerns you about it?

**Raj:** First reaction: I'm already wearing that ring. It's called an Oura. So the question I'd immediately ask is what you're doing that Oura doesn't already do on me. Is your algorithm better than the one Oura already runs, and how would I know? The part that's genuinely new is "notify a care team." That's the loop I just told you is missing, so that part interests me a lot. But I don't want to wear a second ring. I'm not going to wear two rings on my hand for two weeks, and I'm certainly not going to give up two years of Oura baseline for a new device that has to learn me from scratch.

**Interviewer:** Tell me more about the "learns a person's own normal pattern" part.

**Raj:** That's actually my biggest technical concern. When does it learn my normal? If you put it on me at discharge, the "normal" it learns is day-one post-op, which is already abnormal. I'm on pain meds, I've had IV fluids, I'm anemic probably, my heart rate's elevated from surgery itself. So it's baselining on a sick person. If you want a real baseline, you'd have to put it on me weeks before surgery, and then you hit the problem I had where they take it off for the OR and my fingers are too swollen to put it back on for days. And I'd want to know how it separates normal post-op inflammation from an actual infection. Surgery itself makes your body look like it's fighting something for a few days.

**Interviewer:** Anything else that concerns you?

**Raj:** Who sees the data. Care team, fine. The hospital's research database, probably fine if they ask. My insurer, or some data broker, absolutely not. And I'd want the raw data exported to me. If it sends my surgeon an alert and I can't see what triggered it, that's going to make me crazy.

**Interviewer:** Walk me through how something like this would fit, or not fit, into a normal day and night for you over those two weeks.

**Raj:** For me personally, it'd fit trivially, as long as it's replacing the Oura rather than adding to it. I wear a ring 24/7 already; I'd charge it while I shower. Where it wouldn't fit is those first few days, which, frustratingly, are exactly the days that matter. If my fingers are swollen from IV fluids, the ring doesn't go on, or it goes on a pinky and fits badly and the readings are junk. And somebody has to size it. Oura sent me a sizing kit and it took a week. Is that happening before surgery, in the hospital, at discharge? When I was discharged I was holding a bag of prescriptions and trying not to throw up in the car. Nobody was going to fit me for a ring right then.

**Interviewer:** What about for someone who isn't like you?

**Raj:** I shouldn't speak for them, but my neighbor had a hip replacement last year and he can't figure out his hearing aid app. I'm the easy case. If it only works for people like me, your market is small.

**Interviewer:** What would need to be true for you to trust a notification from something like this? What would make you stop paying attention to it?

**Raj:** To trust it, I'd want to see the inputs and the thresholds. What signals, what deviation, over what window, versus what baseline. I'd want to know it's been validated on actual post-surgical patients, not healthy people who ran a marathon, with numbers on how often it fires when nothing's wrong and how often it misses a real leak or infection. And I'd want to know a human with some clinical training is on the other end, and what their response time is. An alert that goes to a queue that someone checks Monday morning is worse than useless, because it gives me false reassurance that someone's watching.

**Interviewer:** And what would make you stop paying attention?

**Raj:** Two or three false alarms that I can't explain. If it notifies my care team and they call me and I'm fine, and it happens again, I'll start to feel like I'm wasting their time, and I'd honestly expect them to start ignoring it too, like the nurses with the pulse ox alarm. Also if it's opaque. If it says "risk elevated" with no reason, I'll go look at my own Oura data instead and decide for myself, which puts me right back where I am today.

**Interviewer:** Tell me more about "wasting their time."

**Raj:** I already feel like I message the PA too much. If a device is effectively auto-messaging her on my behalf every time my heart rate wiggles, I'm going to be a little embarrassed, and I think the team will resent it. The value only holds if the false alarm rate is low enough that a call from them actually means something.

---

## Section D — Value & Willingness to Pay

**Interviewer:** How would you expect something like this to be paid for? For the two-week period: at what price would it seem so cheap you'd doubt it works, a good deal, getting expensive, and too expensive to consider?

**Raj:** My honest expectation is the hospital or Medicare pays, because it's a clinical monitoring service, and the value is in the care team watching it, not in the hardware. I'm not going to pay for a ring I'd give back after two weeks when I already own one. If I were paying out of pocket for the two weeks, I'd think about it like this: the product I'd actually pay for is the service, software that takes my existing Oura and Watch data and gets it to my care team with a real post-op baseline. For a two-week hardware-plus-monitoring program though, since you're asking me to put numbers on it:

- **Too cheap, I'd doubt it works:** under about $25. At that price nobody clinical is looking at it; it's just an app.
- **Good deal:** roughly $75 to $100 for the two weeks, if a real clinician is on the other end.
- **Getting expensive:** around $200. That's half my gadget budget for something I'd use once.
- **Too expensive to consider:** $350 or more, out of pocket. At that point I'd just keep using my spreadsheet and my Oura and send more MyChart messages, which cost me nothing.

**Interviewer:** Tell me more about how you arrived at those.

**Raj:** Mostly against my gadget budget and what I pay Oura, which is a few bucks a month. And to be clear, I have Plan G; I'm used to medical things being covered. If my surgeon said, "we're enrolling you, Medicare covers it," I'd say yes without thinking about price. If the hospital asked me to put in a credit card, I'd hesitate, not because of the money, but because it would tell me they aren't confident enough in it to pay for it themselves. And if it were only software on top of my existing Oura, I'd go no higher than maybe $10 or $15 a month.

---

## Section E — Close

**Interviewer:** Is there anything I should have asked but didn't?

**Raj:** You didn't ask what happens after the alert. That's the whole ballgame. Who gets it, how fast, and what do they do: call me, send me to the ED, order a CT, tell me to recheck in two hours? If the answer is "it goes to the surgeon's inbox," that's going to fail. And ask about the pre-surgery window. Most colectomies like mine are elective, scheduled weeks out. That's your baseline opportunity, not discharge day. Also, you should ask whether you can just integrate with Oura and Apple Health rather than ship hardware. People like me would adopt that tomorrow. Whether that's a business is your problem, not mine.

**Interviewer:** Who else should I talk to about this?

**Raj:** Jessica, my surgical PA, is the one who actually fields these messages, so she knows what the volume looks like. Better yet, whoever answers the after-hours surgical line. I'd also talk to my wife, honestly. She was up with me at 3 a.m. and she had a completely different view: she wanted to just call someone, and I was the one reading papers. And talk to people who aren't engineers. There are a few folks on r/QuantifiedSelf who've posted their post-op Oura data, but they're going to tell you what I told you. You need the people who'd never buy an Oura in the first place.

**Interviewer:** Thank you, Raj. This has been really helpful.

**Raj:** Happy to. If you build the API integration, I'll beta-test it. If it's a second ring, probably not.

---

*End of transcript.*
