# Bots of Customer Success  (docx S5 candidate menu)

These are the **Major sub-functions** of Customer Success from the spec. Each is a bot — a
child decision system that can be instantiated to do the actual work.

## Install flow (matches the Orientation Protocol)
1. **Orient** — the agent runs the Kojiki Orientation Protocol (name / industry /
   jurisdiction / siblings).
2. **Research** — the agent researches the field and decides which sub-functions this
   specific org needs.
3. **Install** — instantiate only the chosen bots:
   ```bash
   cd bots
   python3 install_bots.py brand growth performance-marketing
   ```
   (use the slugs listed below; omit args to install all). Each installed bot becomes a
   full decision system under `bots/<slug>/` with README + AGENT.md + schemas + a stub
   decision record, and registers under this department's group_id for handoffs.

Total candidates: 8.

- `onboarding` — **Onboarding**  ·  titles: Chief Customer Officer, VP Customer Success, Customer Success Director, Customer Success Manager, Account Manager, Support Director, Implementation Manager, CX Manager
- `customer-success` — **Customer Success**  ·  titles: Chief Customer Officer, VP Customer Success, Customer Success Director, Customer Success Manager, Account Manager, Support Director, Implementation Manager, CX Manager
- `account-management` — **Account Management**  ·  titles: Chief Customer Officer, VP Customer Success, Customer Success Director, Customer Success Manager, Account Manager, Support Director, Implementation Manager, CX Manager
- `support` — **Support**  ·  titles: Chief Customer Officer, VP Customer Success, Customer Success Director, Customer Success Manager, Account Manager, Support Director, Implementation Manager, CX Manager
- `implementation` — **Implementation**  ·  titles: Chief Customer Officer, VP Customer Success, Customer Success Director, Customer Success Manager, Account Manager, Support Director, Implementation Manager, CX Manager
- `professional-services` — **Professional Services**  ·  titles: Chief Customer Officer, VP Customer Success, Customer Success Director, Customer Success Manager, Account Manager, Support Director, Implementation Manager, CX Manager
- `customer-experience` — **Customer Experience**  ·  titles: Chief Customer Officer, VP Customer Success, Customer Success Director, Customer Success Manager, Account Manager, Support Director, Implementation Manager, CX Manager
- `voice-of-customer` — **Voice of Customer**  ·  titles: Chief Customer Officer, VP Customer Success, Customer Success Director, Customer Success Manager, Account Manager, Support Director, Implementation Manager, CX Manager
