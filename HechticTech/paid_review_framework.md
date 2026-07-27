# HechticTech — Paid Production Review: Call & Close Framework
# The Production Review is $2,500 and is CREDITED toward any package if the
# prospect moves forward. Position it as a paid working session, not a sales call.
# Goal of the call: leave with (a) a scoped package + price, and (b) a verbal yes
# or a scheduled kickoff. You are not "giving away" the review — you're being paid
# to diagnose, and the fee removes tire-kickers.

══════════════════════════════════════════════════════════════════
0. BEFORE THE CALL (5 min prep)
────────────────────────────────────────────────────────────────
- Pull up the prospect's site + LinkedIn. Note: what they make, approx size,
  any quality certs (ISO 13485, AS9100), any "careers/mfg engineer" posts
  (signals they're hiring = growing = budget).
- Have the live dashboard open: https://theoptimaltimeline.github.io/hechtictech/
  AND a local run of demo_production_dashboard.py ready to share screen.
- Have issue_tracker.py running locally to show the Redmine-style tracker.
- Open a blank notes doc. You will leave them with this as the "fix plan."
- Mindset: you are the expert in the room. They booked a paid session. Lead it.

══════════════════════════════════════════════════════════════════
1. OPEN (2 min) — set the frame
────────────────────────────────────────────────────────────────
Say:
  "Thanks for booking the Review. Quick framing: this is a paid working session.
   We'll dig into one real reporting or tracking pain point, I'll show you what
   an automated version looks like, and you'll leave with a concrete fix plan.
   The $2,500 you paid applies to any package if we move forward — so think of
   it as a down payment on the fix, not a cost. Sound good?"
Then: "Before I show anything — walk me through how production and yield numbers
actually get from the floor to the people who make decisions today."

RULE: shut up and listen. Let them describe the pain in their words. Take notes.

══════════════════════════════════════════════════════════════════
2. DIAGNOSE (10 min) — the 4 questions
────────────────────────────────────────────────────────────────
Q1. "Walk me through how [production/yield/SPC] numbers get from the floor to
     the decision-makers."  → listen for: manual copy-paste, late numbers,
     one person who "is the spreadsheet," blind spots between shifts.
Q2. "What's the ONE report or tracker that wastes the most time?"  → this is
     your scope. Nail it down to a single process.
Q3. "If that were automatic and live, what changes?"  → quantify value:
     hours/week saved, defects caught earlier, audit prep time. Get a number.
Q4. "Who else feels this pain — ops, quality, the PM?"  → find the economic
     buyer / champion so you know who signs.

NOTE TAKING: write the prospect's exact words. Later you echo them back in the
proposal ("you said shift handoffs lose 4 hours of yield visibility…").

══════════════════════════════════════════════════════════════════
3. DEMO (8 min) — prove it's real, not a deck
────────────────────────────────────────────────────────────────
- Share screen on demo_production_dashboard.py with the SAMPLE data.
- "This is the shape of what you'd get — live SPC, yield by line, throughput,
   and a one-click morning report. I'd wire it to YOUR data sources in week one."
- Then show issue_tracker.py: "And if tracking issues/changes is part of the
   pain, this is the structured intake + status view — same system I ran for 7
   years on a wafer-equipment line."
- DO NOT over-build live. You're showing the DELIVERABLE SHAPE, not their data.
- Tie each chart back to Q2/Q3: "This is exactly the 4-hour blind spot you described."

══════════════════════════════════════════════════════════════════
4. PACKAGE & PRICE (5 min) — scope it on the call
────────────────────────────────────────────────────────────────
State the scoped package out loud (use your fixed pricing as the anchor):
  - Production Reporting Automation ...... from $3,500 (2–3 wks)
  - Issue & Change Tracking Setup ........ from $2,500 (1–2 wks)
  - Custom Workflow Automation ........... from $4,000 (scoped)
  - (combo) Reporting + Tracking .......... ~$5,500

Say:
  "Based on what you described, the right starting point is [PACKAGE] at
   $[PRICE], delivered in [TIMELINE]. Your $2,500 Review fee applies, so the
   remaining is $[PRICE − 2500]. I'd have a working demo against your data in
   week one."

PRICING TACTICS:
- Anchor on the fixed price list. Don't discount below it on the call.
- If they balk, trade scope, not price: "We can start with just the reporting
  piece at $3,500 and add tracking later." Never drop below your floor.
- The $2,500 credit is your close lever: "You've already invested $2,500 in
  fixing this — let's put it to work."

══════════════════════════════════════════════════════════════════
5. CLOSE (3 min) — ask for the yes
────────────────────────────────────────────────────────────────
If warm:
  "Want to kick off [PACKAGE]? I'll send the agreement today, you sign, and I
   start pulling your data sources this week. The $2,500 is already applied."
If unsure:
  "What would need to be true for this to be a yes? [listen] — can we get [X]
   resolved in a follow-up with [champion]? I'll set that up."
Always end with a next step + date. No "I'll follow up sometime."

══════════════════════════════════════════════════════════════════
6. AFTER THE CALL (same day)
────────────────────────────────────────────────────────────────
- Email the "fix plan" within 2 hours: a short recap of their pain (their words),
  the scoped package + price, the $2,500 credit applied, and the kickoff date.
- Attach the one-pager (outreach.md OFFER ONE-PAGER section).
- Send the agreement: copy agreement_template.md to agreements/[Client].md, fill
  the [BRACKETED] fields (Package, price, the $2,500 credit applied), delete the
  guidance comments, export to PDF, and send for signature same day.
- Log it in linkedin_outreach.csv: Status → "Proposal" or "Closed."

══════════════════════════════════════════════════════════════════
7. OBJECTION HANDLING (keep these short)
────────────────────────────────────────────────────────────────
"I can just build this myself."
  → "Most can — the question is whether your engineers' time is better on the
     product. This is a 2–3 week fix from someone who's done it on a line. The
     $2,500 Review already scoped it; the build is the cheap part."
"We don't have budget right now."
  → "The Review fee you paid is the budget — it's applied to the build. There's
     no new outlay to start. And the manual time it kills pays for itself fast."
"Send me a proposal and I'll take it to my boss."
  → "Happy to. To make it land, who's the economic buyer and what do they care
     about — cost, yield, audit risk? I'll frame it for them."
"Why not just buy an MES?"
  → "A full MES is $100k+ and 6–12 months. This kills the 20% of the pain that's
     actually hurting you in 2–3 weeks, no rip-and-replace."

══════════════════════════════════════════════════════════════════
8. THE MATH (why paid review beats free)
────────────────────────────────────────────────────────────────
Free review: 20 sent → 20 accept (low intent) → ~6 talks → ~3 paid builds.
Paid review: 20 sent → ~5 book at $2,500 = $12,500 booked BEFORE any build,
  of which ~3 convert to packages (revenue = $3,500+ each, $2,500 already in).
The paid review filters to buyers and pays you while you sell.

Status flow to use in linkedin_outreach.csv:
  Not sent → Sent → Connected → Replied → Review booked ($2,500) →
  Proposal → Closed ($X)
