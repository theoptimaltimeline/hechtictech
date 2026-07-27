# HechticTech — Launch Kit

Manufacturing & production automation for Bay Area EMS / electronics / medical-device
manufacturers. Owner: Rhiannon Hecht (HechticTech LLC) — 7 yrs semiconductor mfg ops,
M.S. Computer Science.

## Live
- Landing page: https://theoptimaltimeline.github.io/hechtictech/
  (Book a Production Review — $2,500, credited toward any package)
- Source of the page: `landing.html` (deployed copy in `site/index.html`)

## How it fits together (the workflow)
Send → Book paid Review → Run the call → Send agreement → Deliver in 2–3 weeks.

1. OUTREACH — find a prospect, send a connection note / cold email.
2. PAID REVIEW ($2,500) — a working session that diagnoses one real pain point.
   The fee is CREDITED toward any package if they move forward.
3. CALL — run the framework, demo the tools, scope a package + price.
4. AGREEMENT — send the filled template same day (credit applied).
5. BUILD — deliver the dashboard / tracker in 2–3 weeks.

## Files
| File | What it is |
|------|------------|
| `landing.html` / `site/index.html` | The live landing page (deployed to GitHub Pages) |
| `demo_production_dashboard.py` | **Working demo**: SPC / yield / throughput dashboard + auto morning report (Streamlit). Run: `python3 demo_production_dashboard.py` |
| `issue_tracker.py` | **Working demo**: Redmine-style production issue & change tracker (Flask + SQLite). Run: `python3 issue_tracker.py` (note: Flask must be on the active Python; macOS port 5000 is taken by AirPlay — uses 5055) |
| `prospects.md` | 50-target list (Tier 1 = Bay Area EMS is your sweet spot) |
| `outreach.md` | Cold email + LinkedIn DM scripts + the offer one-pager |
| `linkedin_dms.md` | 20 personalized LinkedIn connection notes + follow-up DMs (Tier 1) |
| `linkedin_emails.md` | 20 personalized cold emails (Tier 1), one per company |
| `linkedin_outreach.csv` | TRACKABLE sheet: all 20 companies × (ConnectionNote, FollowUp, Email) + Status column. Update Status as you go. |
| `paid_review_framework.md` | The paid-call playbook: open → diagnose → demo → price → close → after-call → objections → math |
| `agreement_template.md` | Blank services agreement with the $2,500 credit clause. Copy + fill per client. |
| `agreements/` | Folder for filled/signed agreements (sample: `AbsoluteEMS_SAMPLE.md`) |
| `HOSTING.md` | How the GitHub Pages site is set up (for reference) |

## Pricing (fixed, not hourly)
- Production Reporting Automation ...... from $3,500 (2–3 wks)
- Issue & Change Tracking Setup ........ from $2,500 (1–2 wks)
- Custom Workflow Automation ........... from $4,000 (scoped)
- Production Review .................... $2,500 (credited toward any package)

## Status flow to track in linkedin_outreach.csv
Not sent → Sent → Connected → Replied → Review booked ($2,500) →
Proposal → Closed ($X)

## The math to $10k
~20 sent → ~5 paid Reviews ($12,500 booked) → ~3 convert to packages
(~$3,500–$5,500 each; $2,500 already in). Paid Review filters to buyers
and pays you while you sell.

## Run the demos
- Dashboard: `python3 demo_production_dashboard.py` → http://localhost:8501
- Tracker:  `python3 issue_tracker.py` → http://localhost:5055
(Mac: disable AirPlay Receiver or use 5055 if 5000 is busy. Use the Homebrew
Python at /opt/homebrew/opt/python@3.11/bin/python3.11 if `flask`/`streamlit`
aren't found.)
