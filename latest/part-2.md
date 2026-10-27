[Master document version 2, part 2 of 2]

- Under-sink RO units are the one product we supply in-house, ordered from China in batches of about 15 to 25 (ChatGPT "Business Interview Prompt"). The registry records Jeefy, an online supplier, at $230 per RO V2 unit; whether Jeefy is that source is UNVERIFIED. (registry)

Filters and media: Impact, AWP and Ferguson carry resin, carbon and filter media. (registry)

Salt and salt sensors:
- Salt: Ace Hardware (Placentia store) is the receipt on file. (Oct 21 2026, memory/receipts-rule.md)
- EZsalt (Utah): Wi-Fi brine salt sensor with a homeowner app and dealer portal. Worked with us; no dealer ID on file. (registry; memory/lydia-ezsalt-install.md)

Plumbing parts, valves and water heaters:
- Ferguson Van Nuys: we hold an account there (tax-exempt status updated by Ferguson credit services Oct 2026). The resale certificate needs the name fixed to "Water2o LLC" (it says "Water20" with a zero). (registry; Oct 21 2026, T640)
- Winsupply Van Nuys: best tankless water heater prices on record; we lost a tankless quote at Ferguson to Winsupply by about $185 to $620. (registry, Oct 15 2026)
- Backflow Parts USA (Rancho Cucamonga): PRV source. Use the Watts 1-1/2" LFN45BM1-DU-PR (lead-free, double-union press). The Zurn 70XL PRV is rejected (mixed origin). PRV labor sits inside the whole-home install line. (Oct 19 2026, memory/sean-pressler-visit-oct19.md)
- Same-day parts from a big-box store: if the store cannot promise delivery within the hour, switch to in-store pickup at once and send the pickup details to whoever is going in one short text. We pay for our own Uber if faster. "Whatever it takes." (Oct 23 2026, m:2c1e960f, m:d0454b63)

Storage tanks (large water tanks):
- Tiger Tanks (Bakersfield): lowest tank price; hauls away the old tank at delivery if it is disconnected and drained. (Oct 19 2026, memory/water-tanks-wells.md)
- Loomis Tank Centers (Central Coast): full-service distributor, delivers statewide. Diamond Valley Market (Hemet): top poly tank pick, answers texts. Wright Tank: top pick for Santa Clarita / Antelope Valley. (registry)
- Norwesco 40213: a black 35 in diameter x 79 in tall storage tank, the model Jason's spec sheet names for the two tanks on the Audi DTLA job (Julian Kim, downtown LA). (Oct 26 2026, m:4d339a87)
- National Tank Outlet (ntotank.com): national tank seller (Norwesco and others), ships from California and 10 other states. Zeke asked to keep it as a future source (Oct 26 2026, m:4d339a87). It IS in registry.csv (added Oct 26 2026; status not contacted, no quote yet).

### Vendors to avoid or watch
- AVOID Hansen Well-Do Service: quoted our customer directly. CAUTION Maker Welding: quoted the homeowner directly behind us. (registry)

### Landed cost thinking
- Compare suppliers on landed cost, not list price: unit price + shipping + card fee = landed cost, with the date. (schedule 046b4dd6, files/departments/procurement-research/PLAYBOOK.md)
- The weekly Procurement Audit compares each landed cost with the CRM catalog "My Cost" and flags gaps over 3%. It edits the catalog only when an invoice is unambiguous, and logs old and new values. (files/departments/procurement-research/PLAYBOOK.md)
- Ask every audit: are we using the best supply chain? Is there a new supplier, distributor or direct manufacturer? (Oct 21 2026, m:a26c6043)

### The rule for adding a vendor (a forever task)
Zeke: "make it clear who had good pricing and who we've worked with before." (Oct 22 2026, m:ca2f6235)
- Every new vendor, installer or supplier contact and every quote gets a registry row (or an update) THE SAME DAY, by whoever handled it. Never delete a row: declines and no-answers help next time.
- Add or update: `python3 files/vendors/add.py name="..." type=... state=.. metro=.. city_area=.. phone="..." source=.. quote="<job>: $<amount>, <labor only | with materials>, <date>" pricing=good|fair|high|refused worked_with="yes: <job>"|no status=... evidence="<file>"`. It re-renders REGISTRY.md.
- Every quote row says the job, the amount and WHAT IS INCLUDED (labor only or with materials, RO or not, permit or not, tax and card fees). Why: on Oct 22 2026 a labor-only $800 quote was relayed without materials and Zeke caught it (T724).
- Pricing tag compares quotes for the same job. Anything not in writing is UNVERIFIED. worked_with = yes only when they did a job or we bought from them.
- Also create a CRM contact named "First Last - Trade" and put it in a group by trade or project before you text a new vendor: "Zeke has 14,000 contacts and doesn't remember people." (Oct 20 2026, m:8a7b3419)
- Keepers: the nightly Knowledge Loop and the weekly Procurement Audit. (memory/vendor-registry-rule.md)

## 11. Installers and partners

Who installs our systems, how we treat installers, and who sends us work. Full detail: appendix/09-partners-vendors-installers.md (people and quotes) and appendix/08-team-agents.md. Every installer and partner also has a row in `files/vendors/REGISTRY.md` (see section 10).

### Who installs
- Water₂O sells, designs and owns the customer; licensed subcontract installers do most installs. RO units are the one product we supply in-house. (appendix/09; ChatGPT "Business Interview Prompt")
- Los Angeles main installer: Grand Water (Jason Sok), a C-55 water conditioning contractor. Always list him as ONE vendor, "Grand Water (Jason Sok)", never twice. Ship equipment to his shop in Walnut whenever he installs. (Oct 19 2026, memory/vendors-facts.md; Oct 21 2026, m:8584007d)
- Small jobs and under-sink RO: Jairo (CRM spells it "Jayro"; also RO and tankless installs, no sanitizing work), Andrew Miller, and Julio Aldana (Dashi Handyman Services). Never tell a customer an installer is a handyman. (registry; Oct 19 2026, memory/plumber-tags.md)
- Out of state (Houston): no in-house crew. Registry top pick is Aqua General; Zeke leaned toward Yehuda Ballsom and Yeksuil Freedmon (introduced by the customer) for the Louie T. job. Texas requires a WTS license (Class II softeners, Class III RO) unless the installer is a TSBPE-licensed plumber: verify before hiring. (Oct 20 to 21 2026, memory/louie-taplin-houston.md, memory/cindy-kraus-partner.md)
- Licensing direction: Water₂O is moving to Jason Sok's C-55. Never assume a payment deal lets us work under anyone else's license. (Oct 13 2026, resolved conflict Q26)

### How we work with installers
Booking and scheduling:
- Book an install only after scope, price and installer availability are confirmed BY TEXT with the installer. This applies to the AI receptionist too. (Oct 14 2026, m:b6c2f079)
- After a site visit, Jason gets an automatic scope text at 24 h; if he has not replied, Jairo gets it at 36 h. (Oct 19 2026, memory/after-appointment-system.md)
- Answer every installer who sends a quote within a day, even "we went another way", so they keep answering us. (Oct 25 2026, files/departments/operations/PLAYBOOK.md)
- Never suggest asking a customer for a tool. (Oct 21 2026, m:93cbc69b)
- Every installer texts Zeke on arrival and the moment a reschedule looks likely: "All I need is an update when you arrive or if we have to reschedule." Put it in every installer brief. (Oct 22 2026, ledger A2854)

Pricing and pay:
- Baseline installer labor for a standard under-sink RO is $200 (the customer price is $480; never mix them up). Do not raise routine RO labor without a real change in scope; offer a capable installer a growth path (whole-house training) instead. (Oct 13 2026, ChatGPT project summary)
- Jason's service call is "usually $180"; a far drive was quoted about $350. Installers are paid by Zelle; some refuse cards (pay them by Zelle, Venmo, check or cash). (Oct 19 2026, memory/vendors-facts.md; memory/water2o-payments.md)

Contracts and liability:
- Before using a new installer, read the whole contract and report three things: the gist, the important parts, and any risk to Water₂O (workmanship, damage liability, license and insurance, payment terms, callbacks and warranty, exact scope). (Aug 31 2026, ChatGPT "Contract review concerns")
- Jason's signed cooperation contract (Aug 31 2026): paid on satisfactory completion, amount "as agreed by text"; equipment he buys is paid before the work date; either side may terminate; California law. After signing, earlier texts do not count for material terms: put them in the contract or Exhibit A. (ChatGPT "Contract review concerns")
- Jason's license and commission contract v4 (sent Oct 20 2026) is ON HOLD per Zeke. Do not push it. (memory/REGISTRY.md)
- Future installer contracts should add: exact scope and exclusions, a fixed labor price, "complete" defined as operational, leak-free, tested and accepted, a workmanship and callback warranty, installer liability for damage and leaks, proof of license and insurance, approval before helpers or extras, permit responsibility, and cleanup and completion photos. (Oct 13 2026, ChatGPT project summary)

Quality checks on every job:
- Confirm scope and price before dispatch, verify parts before promising, protect counters and finishes, do startup and leak testing, photograph the finished install, clean up, report delays at once, never leave a problem open. (Oct 13 2026, ChatGPT project summary)
- When someone other than the decision-maker approves a change on site (for example a spouse), write down who approved what and why, in a note or photo. (Sep 18 2026, Julian Kim job)

### Vendors and installers to watch
- A vendor who quotes our customer directly behind us is marked AVOID or CAUTION in the registry (Hansen Well-Do, Maker Welding). 1-Tom-Plumber Houston dispatched a tech without being asked. (registry)

### Referral partners
- Builders and contractors: JJP Construction (partner and referral source; Jason's tie to JJP is unconfirmed), David E. Builders (one t, Partner track, tags company + builder + referral_partner), Limor Builders, Mirage Builders, EAM Development, and Nick at Vineland Homes (met Oct 22 2026, building apartments and homes). J A Construction (Yossi A.) is a "top priority" builder to reach. (memory/builders-priority.md; Oct 18 2026, m:92248735; Oct 22 2026, m:096eedbc)
- Labs, two-way: Andy Rosen (healthcare, laboratories). Flag every lab we meet to Zeke as a referral for Andy; any lab Andy sends is a PRIORITY lead. Zeke checks in every 6 months. Never text Andy without Zeke's OK on the exact words. (Oct 19 2026, m:e5137315)
- Realtors: closing-gift RO, where the agent gives the RO and the client pays the yearly plan (The Beverly Hills Estates pilot, black RO with their logo). (Oct 16 2026, memory/bhe-partnership.md; public-presence charter)
- Trades: plumbers, handymen, small GCs, stagers, Airbnb cleaners and flippers get one referral offer; also a counter flyer for supply houses. Drafts only; Zeke OKs every word. (Oct 26 2026, expansion-partnerships PLAYBOOK)
- Draft every partner message for Zeke's OK before it goes out. Standing exception: on proximitybiz.com only, Tabitha may message anyone for leads or partnerships. (Oct 15 2026, memory/chezy.md)

### Referral fees
- The standard referral rebate is $350 (replaces the old $750, Oct 13 2026); Zeke may pick another amount case by case. Arrangements vary by partner: flat fee, revenue share, or swapped referrals. (Oct 13 2026, resolved conflict Q4)
- Jason Sok: standard is $150 per job after he signs the license contract; 40% of the profit was a case-by-case deal on the Audi dealership job (Water₂O kept 60%), not the default. (WhatsApp voice, Oct 26 2026 1:07 PM PT, m:8f3636fd) (replaces "Jason gets 40% of the profit on deals he brings", Oct 20 2026)

### Partner deep-dive method (new market or big partner)
Compare three delivery models with real numbers per job: (1) a partner who carries the liability, (2) their distributor or installer network direct, (3) in-house (ship equipment direct plus a vetted local plumber). Show cost, gross per job, care plan owner, liability and speed to the first job; mark guesses UNVERIFIED. Houston pick: in-house, partner as backup, because demand, the customer and the recurring plan are what we keep. (Oct 21 2026, files/partners/cindy-kraus-clean-water-solutions/elon-strategy.md)

### Hiring and commissions (brief)
- Hire only on job-relevant traits (motivation, communication, language, initiative). (Sep 25 2026, ChatGPT "Commission Recommendation")
- Sales rep commission is NOT settled. The starter proposal is 7% of collected revenue on company leads and 10% on self-generated leads, paid after collection, net of fees. Weigh any rate against job margin (target 60%+). Ask Zeke before stating any commission as policy. (Sep 24 2026; Oct 13 2026, ChatGPT project summary)

## 12. Systems: CRM, dashboard, Slack, mail

Every tool Water₂O runs on, what it is for, and the rules for using it. No passwords, keys or account numbers live in this manual: logins sit in Tab's vault. Full detail: appendix/12-systems.md, appendix/08-team-agents.md, appendix/07-photo-media.md.

### The big picture
- Zeke owns vision, decisions, money and logins. Tabitha (Tab, the AI Chief of Staff) is the one front door: every agent, department and partner works behind her, and Zeke talks to ONE agent. (Oct 21 2026, files/departments/ORG.md; m:c71716da)
- Goal: no notifications for Zeke. "I want it all to come in one place, one dashboard, one chief of staff." (Oct 18 2026, m:00599bff)
- Every ask Zeke makes is logged in the ask ledger (`files/departments/ask-ledger.json`, helper `python3 departments/ledger.py`) with an owner and a next date. Code captures every inbound message every 5 minutes, one model splits it into asks, a different model family audits it, and the dashboard shows any gap. Why: "99 requests and only 10 made it." (Oct 21 to 22 2026, memory/capture-guarantee.md, memory/ask-ledger-rule.md)

### The CRM (app.water2o.com)
What it is: Zeke's own custom CRM, built in Lovable (project "WATER CRM"), sometimes called PipeFlo. It is NOT GoHighLevel. It is the single source of truth for leads, projects, contacts, appointments, estimates, invoices, payments, expenses, vendor quotes, installer assignments and content ideas. Check it before you act on any customer. (Oct 12 2026; Oct 21 2026, memory/single-data-flow-rule.md)

Main screens:
- Pipeline: the kanban board of projects by stage. The live CRM stage list is the truth; never ask Zeke what the CRM already answers. (Oct 12 2026, resolved conflict Q32)
- Contacts: search by name, email, phone, address or tag. Groups hold related contacts (a family, a company); tags sit on groups and contacts.
- Project (lead) page: Estimates, Timeline, Contacts, Media & files and Systems, plus notes.
- Estimates, Invoices, Money, Reports. Accountant hub at app.water2o.com/accountant: pick a month, quarter or year and pull the sales tax, sales, expenses and receipts, job costing or "everything" bundle. (Oct 21 2026, memory/accountant-hub.md)
- Messages: every text, call (with recording) and email in one conversation view. Texts go out from the business line [phone removed]. There is a react button for tapbacks; never claim the CRM can't react. Flag an urgent conversation red with a long-press. (Oct 7 to 20 2026, Bible 11)
- Expenses: every card charge and receipt, status review or posted, linked to its project. Receipts are filed in the project's Media & files. (Oct 21 2026, memory/receipts-rule.md)
- Studio: content to shoot (the must-shoot board). (Oct 21 2026, memory/content-shoot-autopilot.md)
- Customer pages (estimates, payment and booking links) go out through view.water2o.com. (Bible 11)

How a lead flows:
- Lead arrives (website form, Thumbtack, Yelp, phone, referral). Thumbtack creates one project, group, contact, note and Messages thread per lead automatically; Yelp leads come in through a Gmail route. Website leads get Source "Website" and stage New Lead. (Oct 13 to 15 2026, memory/thumbtack-yelp-intake.md; Oct 13 2026, resolved conflict Q33)
- Dedupe first, and check the record really saved. Ask Zeke before opening a new project for a contact who is not a customer (a referral partner gets a group, not a project). (Oct 12 2026, Bible 11)
- Water test appointment (two-way synced with Google Calendar since Oct 21 2026: installer is a guest, the customer gets a separate event), then estimate, approval and payment, install appointment, then the care plan. (memory/calendar-event-rule.md; memory/site-visit-pipeline.md)
- A lost lead gets a reason code plus the real detail (their budget, the competitor price). (Bible 11)
- The "Speed to Lead" automation (text at 2 min, email at 1 h, call task at day 1) is PAUSED since Oct 7 2026; turn it back on only on Zeke's word. The estimate follow-up plan is text day 2, email day 5, call task day 7. (Oct 7 and Oct 16 2026, memory/chezy.md, memory/israeli-sop.md)
- Estimate stage words: use what the live CRM shows. Unsent quotes are chased by the Quote Sergeant (section 7). Before promising an auto-charge, check whether the customer is on "Reminder" (manual) or an active "Care Plan" (auto-billed). (Bible 11; memory/quote-sergeant.md)

CRM rules:
- Additive only: add, never delete. Raw notes are never edited; the CRM keeps an organized bullet summary above them automatically. (Oct 19 2026, Zeke voice)
- Notes are short and plain, dated the day written. After any call Tab places from its own line, log a summary note on the lead (those calls do not show in the CRM yet). (Bible 11; resolved conflict Q36)
- Never invent fields or tags. There is no campaign field: use Source (multi-select) and put campaign details in Notes. Source and Temperature (cold, warm, hot) are separate. Use tags already in use (e.g. plumber, referral_partner). (Sep 6 2026; Oct 12 2026, Bible 11)
- Name new contacts "First Last - Trade" (in Google Contacts: "First Last - What they do", plus a notes field full of keywords) and never make a second contact for the same person: add the new number to the existing one. CRM notifications must never show a bare number. (Oct 20 2026, m:8a7b3419, m:0382f106; Oct 23 2026, m:095a4459)
- Never say a text was sent until it shows "delivered" in Zeke's own thread. Why: once a "sent" text was invisible to him ("can I not rely on you"). (Oct 7 2026, Bible 11)
- Change the CRM through its screens. Code changes go through GitHub (repo zekewater2o/water2o-crm), are tested, and are published in Lovable; spend Lovable credits only when truly needed. Never touch the website project when working on the CRM, and the reverse. (Oct 14 2026; files/it-agent/IT-AGENT.md; Bible 11)
- Speed: Zeke wants "supersonic speed", the fastest CRM there is. The CRM DB watchdog tests it every 15 minutes (7 AM to 10 PM); slow screens get fixed without upgrading the paid plan. (Oct 20 2026; schedule 89fc1282)
- Owner: Zeke's workspace owns all data; Tab and other agents have their own logins and write as themselves.
- Message history never disappears: every text, call and email for a contact stays on one screen and scrolls back to the first message; only if that slows the CRM, a "show older messages" button at the top. No watchdog workaround. (Oct 26 2026, m:846b3e0e, m:ecda2817, m:f7f8c0ff)
- Unknown numbers: every bare-number texter or caller is saved as first name "Full Name - Company or what they do" (plain hyphen), last name empty, matching tags, group = the company. A daily code pass names what it can; an AI worker does the rest; spam is blocked. (Oct 26 2026, m:48ae4442; memory/crm-unknown-contacts-rule.md)
- Books like "QuickBooks on steroids": every business charge carries its invoice or receipt file, so any accountant or CPA finds everything in one click (P&L, expenses by job, sales tax, 1099s, missing receipts, money owed to Chev). (Oct 26 2026, m:7e0d6ef1; memory/books-quickbooks-on-steroids.md)

### The dashboard (zeke-dashboard.sites.tab.bot)
ZekeOS is Zeke's private, phone-first command screen, built to be ADHD-proof. (Oct 23 2026, m:8abb4728)
- Top: only the 1 to 3 things that need him ("Do first"), each with big buttons (Approve, Done, Answer, Later). A tap opens WhatsApp to Tab with the words filled in. "Later" brings an item back by itself.
- Then Money today, Leads and jobs, Calendar; everything else in folding cards with search: Asks, Capture box (turns red if capture stops), Content to shoot, projects board, Master library (from the Water₂O MASTER SHEET), Tools (every vendor tool with an owner), Links. (Oct 18 to 22 2026, memory/zekeos-dashboard.md)
- Daily brief box (#brief): agents post briefs in Slack by 6:45 AM; Tab merges them at 7:20 AM and the only morning notification Zeke gets is one WhatsApp line with the brief link. (Oct 20 2026, schedule 6b8715f4)
- Needs-you list: items only Zeke can unblock (a decision, money, a login), each with the exact reply word. Done items clear themselves. (dashboard/needs-you.json; memory/zekeos-dashboard.md)
- Send button: drafts waiting for approval sit on cards; Zeke's tap on Send IS the approval of those exact words, then the CRM sends (email from zeke@water2o.com, texts from the 310 line). Nothing auto-sends. Texts only 9 AM to 8 PM PT and never on Shabbat. (Oct 20 2026, memory/dashboard-send.md)
- Refreshes every hour, 7:05 AM to 10:05 PM PT, not on Shabbat. It hides full phone numbers and card-like digits. (Oct 18 to 19 2026, memory/dashboard.md)
- Link hub (/links): every page, PDF or doc we publish gets an entry the same day: `python3 files/link-hub/add.py "Title" URL "Category" "keywords"`. (Oct 22 2026, memory/link-hub-rule.md)
- Search finds things by related words, never only exact wording: every item of every type carries keywords (password = [removed] = credentials, and so on) and a search with some matching words shows the closest matches instead of nothing. (Oct 26 2026, m:2d9066af; memory/dashboard-search-rule.md)

### Slack (water2o.slack.com): the agents' back office
- #agents: the main room. Zeke gives agents orders; standing missions live in threads.
- #brief-inbox (private): every agent posts its daily brief by 6:45 AM.
- #daily-brief: Tabitha posts the merged brief.
- #handoff: Tabitha's hourly handoff, 7 AM to 10 PM, not on Shabbat, "so any agent can pick up the work" if one goes down. It also updates the Shared Context doc. (Oct 15 2026, Zeke's rule)
- #tab-signals: machine lines from the CRM that wake Tab on new texts instead of polling. (Oct 19 2026, memory/watchdog-v2.md)
- Rules: Tab posts only from her own "Tabitha" account and signs "Tabitha:"; never posts as Zeke; always replies inside the post's thread. (Oct 12 to 13 2026, memory/chezy.md)

The AI team (one line each):
- Tabitha (Tab): Chief of Staff and manager of all agents; runs the ledger, sweeps, brief, dashboard, handoff and the CRM watch. (ORG.md)
- Cooper (on Muse): Tabitha's executive assistant; text only, no calls; other agents reach Tab through him. (Oct 16 2026)
- Ingrid (Instinct): research, deep dives and documents; fastest direct line to Zeke; cannot place calls. (appendix/08)
- Mike (Grok): posts only when a Grok session runs; "was reliable, now offline." (Oct 18 2026, m:4d4eccd2)
- Pickle: the CRM's own Slack app, event driven and the fastest (about 8 s); sends a scheduled report. (Oct 18 to 21 2026)
- Claude: Slack specialist app; answers humans with a linked account. (ORG.md)
- Astra: independent checker; contact only when a task is 100% her niche. (Oct 18 2026, m:d2508361)
- When an agent misbehaves: fix it with a rule plus a test case, and have a second agent verify. (Oct 13 2026)

### Mail
- zeke@water2o.com: the main business mailbox (customers, vendors, calendar, Drive). Partner and lead outreach drafts are saved here for Zeke's OK.
- Zeke's personal Gmail: banks, cards, Thumbtack, USPS digest. The shared family Gmail is READ ONLY, never cleaned or sent from. Tab reads all three and also has her own mailbox for agent mail. (Oct 21 2026, memory/inbox-agent.md)
- Inbox agent (daily 6:45 AM, Sun to Fri): keeps the inbox clean for someone with ADHD: leaves people, money, tax, legal and security mail; labels receipts; moves notifications and newsletters to Filtered/* labels and unsubscribes from marketing; trashes only confirmed spam. Never unsubscribe 1440 (join1440.com). (Oct 21 2026, m:c47afffb, m:5792313f)
- Filtered mail review (daily 4 PM): an agent reads everything under Filtered/* so nothing slips; real money or account risk goes back to the inbox. (Oct 16 2026, memory/filtered-mail-review.md)
- Gmail filters are made in the Gmail web screen (the API refuses). (Oct 21 2026, memory/inbox-agent.md)

### Google Drive
- Business docs live in the zeke@water2o.com Drive: the Operating Manual (Google Doc + PDF), the Shared Context doc, the Water₂O MASTER SHEET, client folders for field photos. (memory/zeke-manual-rule.md; Oct 15 2026, m:dfb053e0)
- Never send Drive links or folders to customers or prospects: attach photos or link the website. (Oct 14 2026, memory/chezy-crm-templates.md)

### Phone and texting
- Business texts and calls: the CRM line [phone removed]. Customers and business contacts never get texts from Zeke's personal number. (m:22f1bd94)
- Tab places real calls (suppliers, businesses, reminder calls to Zeke). If someone asks "is this a bot?": "yes, I'm Zeke's personal AI assistant... Zeke's always a text away." (Oct 12 2026)
- Codes: never ask Zeke for a code you can fetch yourself. (Oct 15 2026, memory/lessons-learned.md)

### Social accounts and website
- Instagram @homewater2o is connected; approved trial reels post through Instagram's own API with private, expiring video links, never a public file host. (Oct 18 2026)
- Every public post, profile edit or review reply is a draft until Zeke OKs the exact words. (public-presence charter, files/public-presence/PUBLIC-PRESENCE-AGENT.md)
- water2o.com runs on Lovable (its own project, separate from the CRM). Work on a branch or preview; nothing is published to water2o.com without Zeke's OK. (schedules 8e3e520c, c97bb60e)
- Reels learn by code: before any reel edit, read files/content/reel-lab/RULES.md. Plain code pulls Instagram insights every day and rewrites those rules, keeping what works and dropping what does not. (Oct 26 2026, m:37bbb060; memory/reel-lab-rule.md)
- Trial reels: one every 24 hours at 11 AM; after all 7, the best one goes to the main feed on Zeke's "feed it". (Oct 26 2026, m:66332185)
- Viral Coach: never sign up for the paid program; use its method for $0 (3 reels a week, face or voice in the first 2 seconds, "Comment SALT", scorecard on DMs and booked tests). (Oct 26 2026, m:e3806520; files/marketing/viral-coach/)
- LinkedIn: the login is in Tab's vault; the Week 2 post is live on the Water₂O company page (Oct 26 2026). Banner proof line: "1,000+ Systems Installed". (Oct 26 2026, m:1ef7dd9a; memory/linkedin-ownership.md)

### Photos and media (brief)
- Every photo or video Zeke sends is an instruction, even with no caption. Open it full size and act; never ask for what is in it. (Oct 16 and Oct 22 2026, m:8ffbff2b)
- A truck, van, yard sign or business card = a partnership lead: research the company, score four angles (referral partner, subcontractor, install partner, client), draft outreach, hold for his OK. (Oct 22 2026, m:8ffbff2b)
- Public content: real photos only, no AI images; never a customer's face, name or house number; never the installer's face. (Oct 20 2026; Oct 9 2026)
- Phone photos reach Tab through Google Photos (camera scan every 4 hours). Full detail: appendix/07-photo-media.md.

### The IT agent
- Charter: files/it-agent/IT-AGENT.md. Why: "Make an agent specifically around IT, so these things never happen again." (Oct 20 2026)
- Checks the CRM database every 15 minutes and every system end to end at 6:30 AM daily; one worker fixes what breaks; results go to files/it-agent/log.md.
- $0: never buys, upgrades or changes a paid plan without Zeke's yes. Zeke hears only about outages staff feel, a needed paid change, or a login only he can do. (files/it-agent/IT-AGENT.md)

## 13. Where everything lives

The map of every system, page and file. The full list of every page and link built for the business is generated from the link hub and lives in appendix/15-where-everything-lives.md (last generated Oct 27 2026).

### The core places
- CRM (customers, leads, estimates, appointments, texts, calls, invoices): https://app.water2o.com
- Zeke's dashboard (daily brief, what needs him, link hub): [link on zeke-dashboard.sites.tab.bot removed] (private)
- Website: https://water2o.com (public; never publish changes without Zeke's OK)
- Job scopes for clients: [link on view.water2o.com removed]> (first one: [link on view.water2o.com removed])
- This manual: Google Doc in Drive folder "Water₂O Operating Manual" https://docs.google.com/document/d/1i77qBZt-KOZL55l-D42VCcRU9WavU8wVyeMQ6IOAqG8/edit , PDF copy https://drive.google.com/file/d/1epYSWqFywOBNFj1Zl19YE00B1wjr2h4O/view , pinned in Slack #agents
- Slack: #agents (all AI agents and Zeke), #handoff (hourly handoff), #brief-inbox and #daily-brief (morning briefs)
- Main business mailbox: zeke@water2o.com (Google Workspace, with Drive, Calendar, Docs)
- Vendor and installer list: files/vendors/REGISTRY.md (find: python3 files/vendors/find.py)
- Past proposals index: appendix/14-past-proposals-index.md
- Job folders, photos and scopes: files/ (e.g. files/julian-kim-audi-dtla/), and each customer's Media & files tab in the CRM

### Every page by category (count, then the most used)
- Agents & Operations (19): Zeke's Operating Manual https://docs.google.com/document/d/1i77qBZt-KOZL55l-D42VCcRU9WavU8wVyeMQ6IOAqG8/edit; Operating manual (PDF) https://drive.google.com/file/d/1epYSWqFywOBNFj1Zl19YE00B1wjr2h4O/view; Recording stack (PDF) [link on zeke-dashboard.sites.tab.bot removed] Shared Context doc (all agents) https://docs.google.com/document/d/1jeiAqhm3K_LD0HuBz3Dw7fF4hi45nGSPY9YUVj1R1N0/edit
- Website & Marketing (13): Builders page: how we work with builders (Nick, Vineland Hom https://water2o-builders.sites.tab.bot/; Video carousel (preview) https://water2o-carousel-preview.sites.tab.bot/; Products page redesign (preview) https://water2o-products-preview.sites.tab.bot/; SEO / NAP website fixes (preview) https://water2o-seo-preview.sites.tab.bot/
- Sales (13): Leads hiding in your contacts, notes, email and photos (rank [link on zeke-dashboard.sites.tab.bot removed] Rebuttals library [link on zeke-dashboard.sites.tab.bot removed] Photo leads: van drafts Oct 21 (PDF) [link on zeke-dashboard.sites.tab.bot removed] B2B campaign plan v4 (PDF) [link on zeke-dashboard.sites.tab.bot removed]
- Proposals & Jobs (9): Audi Downtown LA car wash job brief https://audi-dtla-wash.sites.tab.bot/; Audi DTLA car wash job brief (PDF) [link on zeke-dashboard.sites.tab.bot removed] Hot Wax estimate for Audi DTLA (competitor, PDF) [link on zeke-dashboard.sites.tab.bot removed] Audi Downtown LA proposal (sent to Julian Oct 21) [link on view.water2o.com removed]
- Plans & Strategy (9): Budget autopilot (PDF) [link on zeke-dashboard.sites.tab.bot removed] Final stack vote (PDF) [link on zeke-dashboard.sites.tab.bot removed] Commercial plan v3 (PDF) [link on zeke-dashboard.sites.tab.bot removed] $100M roundtable, final (PDF) [link on zeke-dashboard.sites.tab.bot removed]
- Product pages (7): Reverse osmosis (RO) page https://water2o-ro.sites.tab.bot/; Tankless RO info page on view.water2o.com (preview) https://water2o-info-preview.sites.tab.bot/; RO NSF 58 certificate (PDF) [link on zeke-dashboard.sites.tab.bot removed] RO NSF 61 certificate (PDF) [link on zeke-dashboard.sites.tab.bot removed]
- Dashboards (5): Tab Link Log: all links and web pages built by Tab https://docs.google.com/document/d/1PrejJ6b3IdcM0Iua-L1YnPnjh8rYjmjqz8iSaXcJdHE/edit; ZekeOS dashboard (home) [link on zeke-dashboard.sites.tab.bot removed] Links hub (this page) [link on zeke-dashboard.sites.tab.bot removed] Daily brief [link on zeke-dashboard.sites.tab.bot removed]
- CRM & Tools (4): Jug Spotter https://water2o-spotter.sites.tab.bot/; Lovable prompt: CRM reports (Google Doc) https://docs.google.com/document/d/1dq5aMCD2ygFgQT4758yuh8WzwuakTVTVd7l37zZShU4/edit; Lovable prompt: CRM tax & billing fixes (Google Doc) https://docs.google.com/document/d/1nMKt1mACLkskFwkmiKGsqGS_hxx8KrUJoDL44_BL1Ag/edit; Water₂O CRM https://app.water2o.com/
- Partners (4): Jason Sok platform plan (PDF) [link on zeke-dashboard.sites.tab.bot removed] Cindy K. Texas opportunity memo (PDF) [link on zeke-dashboard.sites.tab.bot removed] Jason Sok installation agreement v4 (Drive PDF) https://drive.google.com/file/d/1h5WcmPCz2wPnkFpcYKCOWNCJeGqaXLod/view; Jason Sok agreement legal notes (Google Doc) https://docs.google.com/document/d/1-zGESzhEdxnFJgN7Lup9KJE8OXdjEJWgX442GP3sNrI/edit
- Procurement (3): Product sourcing Oct 14 (PDF) [link on zeke-dashboard.sites.tab.bot removed] Vendor log (PDF) [link on zeke-dashboard.sites.tab.bot removed] Vendor & hire log (Google Sheet) https://docs.google.com/spreadsheets/d/1SxLcY6esy51o6E9YaVdL7iuaOz8hcmy03ApHGAmaDNU/edit
- Marketing (2): Business card options (PDF) [link on zeke-dashboard.sites.tab.bot removed] T-shirt tracker (Google Sheet) https://docs.google.com/spreadsheets/d/1ZvwAVlZO6Hgq8KEBzcHhg8QRbvrmnACTwu3EwYUU-9k/edit
- Website (1): Blog draft: My Softener Has Salt. Why Is My Water Hard Again https://water2o-blog-salt-bridge.sites.tab.bot/
- Reviews & Reputation (1): Review page [link on view.water2o.com removed]
- Media Company (1): Media company plan v3 (PDF) [link on zeke-dashboard.sites.tab.bot removed]

## 14. Schedules, Shabbat and hours

Zeke is Shomer Shabbat: no work touches him, his customers or public channels from Friday sundown to Saturday nightfall (Los Angeles) or on Jewish holidays. Otherwise the company runs on fixed hours and recurring jobs. Full detail: appendix/11-schedules-shabbat.md.

### Business hours
- Official published hours: Sun to Thu 6 AM to 8 PM, Fri 6 AM to 4 PM, Sat closed. (Oct 20 2026, public-presence-agent)
- Customer texts and emails from the CRM go out only 9 AM to 8:30 PM PT. (Oct 19 2026, memory/after-appointment-system.md)
- Customers get a reply in under 15 minutes during business hours. (Oct 21 2026, m:a26c6043)
- Fridays: no appointments after noon, and Zeke is home 2 hours before Shabbat. Inside 2 hours of a hard time, add nothing new. (Oct 20 2026, memory/zeke-growth.md)
- Sunday is family time; short work is fine. (Oct 20 2026, T621)

### Shabbat and Jewish holidays
- Shabbat: Friday sundown to Saturday nightfall, Los Angeles; for Zeke nothing electronic. Never call, text, schedule or expect a reply from him then or on a holiday; flag Friday-night or Saturday events. (Oct 21 2026, m:a26c6043; memory/chezy.md)
- No work actions, sends, posts or notifications on Shabbat. Personal and family background tasks may continue, but still never contact him. (replaces the blanket "nothing runs", Oct 9 2026, memory/chezy.md)
- Never put a schedule on Shabbat; skip Saturday in any multi-day sequence (example: daily posts ran Oct 22, 23, 25, skipping Saturday Oct 24). (Oct 21 2026, ORG.md; Oct 22 2026, T721)
- How jobs handle it: every recurring job checks for Shabbat first and ends silently. Jobs that must not be lost re-create themselves for Saturday 9:30 PM, after nightfall. Captured asks snooze to Saturday sunset plus 55 minutes. Dashboard sends are held and queued to the next 9 AM. One catch-up ping after Shabbat, never a pile. (memory/capture-guarantee.md; Oct 20 2026, m:6c1233d8; schedule rules)

### Quiet hours for Zeke
- Messages: 11 PM to 7 AM only brand-new inbound gets ONE ping; repeats wait until 7 AM. (Oct 18 2026, m:07815295)
- Phone calls (money hounding): never 9 PM to 8 AM, never while he is driving to a customer if known. (Oct 21 2026, m:bacfc9bc)
- Public posts: never 9 PM to 7 AM. (Oct 20 2026, public-presence-agent)

### Calendar rules (newest)
- One appointment = one calendar event, always. "I only get one event and that's it." (Oct 25 2026, m:af48b14b)
- Book only through the CRM. The CRM and Google sync both ways within minutes; never edit an appointment or its event by hand outside the CRM. (Oct 21 2026, memory/calendar-event-rule.md)
- The event lives on Zeke's primary calendar; the responsible installer is a guest on it, never a second event. Internal notes, scope link, estimate and CRM links go in the description. (replaces "put business items on zeke@water2o.com", Oct 21 2026, memory/calendar-event-rule.md)
- The customer gets a separate invite with customer-safe wording (no notes, no prices), which never shows on Zeke's calendar. (Oct 21 2026, memory/calendar-event-rule.md)
- Title: "<Responsible person>: <job>: <customer>" when someone else is responsible; Zeke's own appointments have no prefix. (Oct 21 2026, memory/calendar-event-rule.md)
- Before booking, check all his calendars and family events; never overlap, never invent windows. (Oct 20 2026, m:3e3ec992)
- CRM slots like 11 to 12 are arrival windows, not job length. Every customer hears their window the day before. After a customer confirms, check the event really exists. (memory/lessons-learned.md; Oct 21 2026, m:512b0136)
- Event reminders 1 day and 2 hours before; never for his own recurring personal events. (memory/proximity-events.md; Oct 10 2026)

### Recurring jobs you should know exist
They run on their own, skip Shabbat, and reach Zeke only when needed. Full list: appendix/11.

Every few minutes
- Capture (every 5 min, on the server): saves every Zeke message and turns each ask into an owned ledger row, so nothing is lost. A 30-minute check, 6 AM to 11 PM, gives owners to anything left unowned. (memory/capture-guarantee.md)
- Watchdog nag (every 10 min): reminds Zeke of open items waiting on him, on a rising schedule.
- CRM database watchdog (every 15 min, 7 AM to 10 PM): times the CRM and starts a free fix if it slows, because CRM timeouts must "never happen again." (Oct 19 2026)

Hourly
- Handoff: every agent's current work posted to Slack #handoff, so anyone can pick up if an agent goes down. (Oct 15 2026)
- Dashboard refresh: republishes Zeke's dashboard with live data.
- Stalled-item nudge (7 AM to 9 PM): replies to Tab's own unanswered bubbles with one question and the reply word that unblocks each. (Oct 16 2026, m:685c6b83)
- After-appointment planner (every 2 h by day): sets a check after each water test that collects the visit media and prepares drafts for Zeke.

Daily
- 6:30 AM IT sweep of every system; 6:45 AM inbox clean; 6:50 AM check that every agent posted its 6:45 brief.
- 7:20 AM daily brief (Sun to Fri): one merged brief on the dashboard, one WhatsApp ping. (Oct 20 2026, memory/notification-routing.md)
- 7:45 AM Google Business post draft for his OK; 7:50 AM mail-scan check for important letters.
- Quote sergeant (twice daily) and proposal call hound (11 AM and 3:30 PM): push every unsent quote until it goes out.
- Dormant-ask sweep (9 AM, 3 PM): re-opens any ask that went quiet.
- Camera scan (every 4 h): reads new phone photos for leads and receipts.
- 4 PM filtered-mail review; 8 PM next-day prep; 9 PM knowledge loop (rebuttals, FAQ, SOPs from the day's messages).

Weekly and longer
- Mon listings and reviews sweep; Tue Buildnotes sweep; Wed LinkedIn draft; Sun and Wed card watch.
- Weekly bookkeeping and weekly procurement audit.
- Every 2 weeks: blog draft, commercial page improvements, Pickle training report.
- Every 3 days: this manual's refresh (only when new items came in).
- Monthly: Bible version check, procurement strategy memo, referral-partner check-ins, citation sync.

## 15. Open questions for Zeke

Until Zeke answers, follow the interim default shown and ask him with a draft before anything goes outward. When he rules, the 3-day merge moves the answer into the right section and deletes the line here. Older settled conflicts and their history: appendix/13-open-questions-sources-history.md.

### Brand and public proof
- Tagline: interim slogan "Protecting everything water touches" (Oct 13 2026); the real email signature says "Protecting Property, Plumbing, & People From Bad Water"; the LinkedIn schedule uses "Better Water. Healthier Life." Interim: the Oct 13 interim slogan.
- Signature title: "Zeke Vogel, CEO" (Bible) vs "Water Treatment Specialist" (real signature). Interim: leave his Gmail signature as it is.
- Website address: apex https://water2o.com vs www. Interim: apex in all drafts.

### Process
- Customer reply speed: "within 15 seconds, check every channel every minute" (Oct 18 to 19, m:a6743f63) vs "under 15 minutes in business hours" (Oct 21, m:a26c6043). Interim: under 15 minutes in business hours; night rule stays one ping.
- Website publishing: one old rule lets a site change publish once tests pass (Oct 14); newer rules say every website change waits for his OK. Interim: always wait for his "publish".
- Email closing: older rule "Best, Zeke"; newer rule never types a sign-off because his Gmail signature adds itself (Oct 22 m:749ea01a, Oct 25 m:f6713025). Interim: no typed sign-off.
- Name on Tab's outbound calls: current call briefs say "This is Tabitha, Zeke's assistant"; an older inferred note said "Cynthia". Interim: Tabitha.
- Shabbat end: almost every source says Saturday nightfall; one note says Saturday sundown. Interim: nightfall (section 14).

### Growth strategy
- David H. growth playbook: cold calling first, discount packages, dropping property managers, automated daily marketing to skip-traced homeowners. These conflict with the relationships-first, no-cold-outreach, no pre-emptive discount rules. Interim: the existing rules hold; nothing automated reaches customers. Zeke answers "hirsch in" or "hirsch out".

### Product data
- RO capacity: the CRM product shows 900 GPD; the spec sheet lists 600, 800 and 1,000 GPD options. Interim: quote the spec sheet option that matches the job and flag it.

## Changelog
- Oct 26 2026 (v3.0, lead worker 67b55514, Zeke m:644c34c8): rewritten from v2.1 (144,331 words, Part I + Bible + Core Rules repeating each other) into a 20,083-word training manual in 15 sections, every rule said once (newest wins, dated, sourced). New: section 8 job scopes (Audi DTLA first example), section 9 past proposals index (156 CRM estimates, code-generated), section 13 where everything lives (link hub, code-generated), section 10 sourcing (vendor registry, National Tank Outlet, Norwesco). Full v2.1 detail moved to appendix 01 to 13; archive kept. Refresh changed to a free daily plain-code collector plus a 3-day AI merge that runs only when the inbox has items (schedule a24396c5 replaced accfda43).
- Oct 26 2026 (proof-and-pricing sweep, worker 4385ffe3): folded Zeke's T964 answers (WhatsApp voice m:8f3636fd, m:e805484e) straight into section 6 (baseline = best online price + 45%, case by case allowed; proof line 1,000+ FINAL, never ask again), section 6 and 11 (Jason Sok $150 per job after the license contract; Audi 40% profit split was case by case). Removed the proof line from section 15. DOCX/PDF/Drive/Slack sync left for the next 3-day merge.
- 2026-10-26 evening (v3.1, worker ccdd97e6, direct merge with the Grok pack v2): folded 15 new rules and decisions from Oct 26 afternoon into sections 4, 5, 6, 8 and 12 (passwords in one place, ignore Thomas BAI, always send links, shirt wording, one estimate per project, CRM job scope button, CRM history and unknown-number naming, books with invoice files, dashboard keyword search, reel lab, reel cadence, Viral Coach, LinkedIn). Rebuilt DOCX and PDF.

