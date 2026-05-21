# Discovery Questions for Dreamforce Staffing

**Purpose:** These questions need answers before we can design effective automation  
**Owner:** Summer Hash to investigate  
**Timeline:** Need answers by end of May 2026 (first week of June latest)

---

## Priority 1: Critical (Blocking Design)

These questions block our ability to design solutions. Must be answered first.

### Event Footprint Source of Truth

**Question:** Where does Strategic Events document what Slack is building at Dreamforce (booths, SICs, sessions, meeting spaces)?

**Ask:** Strategic Events team or Alyssa Sachs  
**Why it matters:** Need to know where to get staffing requirements from  
**Validation:** Get access to the document, confirm it's kept current  
**Priority:** URGENT - blocks understanding of staffing needs

**Follow-up questions:**
- When is this information finalized?
- Who receives updates when it changes?
- Is there a timeline/schedule for decisions?

---

**Question:** Where are sessions (SICs and spoken sessions) cataloged?

**Ask:** Marika's team, PMM leads  
**Why it matters:** Need to know staffing requirements for sessions  
**Validation:** Get access, see if it's in Rainfocus or elsewhere  
**Priority:** URGENT - major component of staffing

**Follow-up questions:**
- Is Rainfocus the source of truth or just one copy?
- Who updates this list and how often?
- When are sessions finalized?
- Who on PMM team owns this?

---

### Pass Allocation Process

**Question:** What tool/system is used to allocate passes to people?

**Ask:** James Turner (Ryan Gavin's org), Ria Mancoosh (Rob Seaman's org)  
**Why it matters:** Need to know if we can access or integrate with this system  
**Validation:** See the tool yourself, understand its capabilities  
**Priority:** URGENT - central to entire process

**Follow-up questions:**
- Is it Rainfocus backend?
- Is it a spreadsheet?
- Is it something else?
- Can you export data from it?
- Who has access?

---

**Question:** How are pass allocations per org decided?

**Ask:** James Turner, Ria Mancoosh, Alyssa Sachs  
**Why it matters:** Need to know if this is rule-based or pure judgment  
**Validation:** Understand the process they use to make decisions  
**Priority:** URGENT - determines if we can build allocation models

**Follow-up questions:**
- Is it based on staffing needs?
- Is it based on headcount per org?
- Is it political negotiation?
- When are allocations finalized?
- Can this be modeled/calculated?

---

### Rainfocus Data Access

**Question:** Can we export data from Rainfocus? What data? How?

**Ask:** Marika's team (they use Rainfocus backend)  
**Why it matters:** Determines what automation is possible  
**Validation:** Actually try exporting, see what you get  
**Priority:** URGENT - determines technical approach

**Follow-up questions:**
- Is there an export button? What format (CSV, Excel)?
- What tables/data can be exported?
- How often can exports be generated?
- Is data export real-time or delayed?
- Who has permission to export?

---

**Question:** Is there a Rainfocus API or programmatic access?

**Ask:** Marika's team, Strategic Events, Salesforce conference tech team  
**Why it matters:** Would enable real-time automation  
**Validation:** Get API documentation if it exists  
**Priority:** HIGH - nice to have but not required

**Follow-up questions:**
- Is it a public API or requires special access?
- What operations are supported (read, write, both)?
- Are there rate limits or restrictions?
- Who can we talk to about API access?

---

### Multi-Stage Tracking

**Question:** Where is the apply → approve → assign → schedule pipeline tracked?

**Ask:** James Turner, Ria Mancoosh  
**Why it matters:** Need to understand current workflow to improve it  
**Validation:** See the actual system/spreadsheet they use  
**Priority:** URGENT - need to track this data

**Follow-up questions:**
- Is any of it in Rainfocus?
- Is it in spreadsheets?
- Is it in email?
- Is it in multiple places (which ones)?
- How do you know current status for each person?

---

## Priority 2: Important (Informs Design)

These questions significantly impact design but we can make assumptions if needed.

### Staffing Requirements

**Question:** Are staffing requirements documented anywhere or is it all tribal knowledge?

**Ask:** Dustin Burnett  
**Why it matters:** Need to know if we can codify requirements into calculator  
**Validation:** Review documentation or document it from interview  
**Priority:** HIGH - required for automation

**Follow-up questions:**
- How do you determine how many people per shift?
- Are there formulas (e.g., "2 demo specialists per 4-hour shift")?
- Does it vary by booth/SIC/session?
- What skills/roles are needed for what areas?
- Which roles can be filled by non-Slack people?

---

**Question:** What roles exist and what are the requirements for each?

**Ask:** Dustin Burnett, Marika's team  
**Why it matters:** Need role taxonomy for staffing calculator  
**Validation:** Get definitive list with descriptions  
**Priority:** HIGH - required for accurate staffing

**Follow-up questions:**
- What's the difference between booth volunteer vs. demo specialist?
- What roles require special training or skills?
- What roles can only be Slack employees vs. contractors?
- Are there minimum shift lengths per role?

---

### Timeline & Deadlines

**Question:** When do key decisions happen relative to event date?

**Ask:** You, James, Ria, Marika's team  
**Why it matters:** Need to know when Summer needs to do what  
**Validation:** Create timeline based on last year + this year's plan  
**Priority:** HIGH - determines dashboard and reminder timing

Key milestones to clarify:
- When are pass allocations decided?
- When do applications open?
- When do approvals close?
- When are pass assignments finalized?
- When do shift signups open?
- When do shift signups close?
- When do sessions get finalized?

---

### Last-Minute Changes

**Question:** What causes most last-minute shift changes?

**Ask:** You, Dustin  
**Why it matters:** Understanding root cause helps design better solution  
**Validation:** Review last year's data if available  
**Priority:** MEDIUM - informs self-service design

**Follow-up questions:**
- How many changes typically happen?
- Are they mostly cancellations or swaps?
- What are common reasons (sick, client meeting, conflict)?
- How much advance notice do people give?
- How are changes currently communicated?

---

**Question:** What's the current process when someone can't make their shift?

**Ask:** You, Dustin  
**Why it matters:** Need to understand current workflow to improve it  
**Validation:** Document the step-by-step process  
**Priority:** MEDIUM - required for self-service design

**Follow-up questions:**
- Do they contact staffing lead directly?
- Do they try to find their own replacement?
- How is the change recorded?
- How is Rainfocus updated?
- Who has authority to approve swaps?

---

## Priority 3: Nice-to-Know (Optimization)

These questions help optimize but aren't blocking.

### Historical Data

**Question:** Do we have data from past Dreamforces (2024, 2025)?

**Ask:** You, Strategic Events, Marika's team  
**Why it matters:** Historical data could inform predictive models  
**Validation:** See if data exists and is accessible  
**Priority:** LOW - nice for analytics but not required

**Follow-up questions:**
- What data do we have (attendance, no-shows, changes)?
- Is it in Rainfocus or archived elsewhere?
- Can we access it?
- Is it clean and usable?

---

### Integration Opportunities

**Question:** What other tools does Summer use day-to-day?

**Ask:** Summer Hash  
**Why it matters:** Could integrate with her existing workflow  
**Validation:** List of tools and usage patterns  
**Priority:** LOW - nice to have integrations

**Follow-up questions:**
- Email client (Gmail)?
- Calendar (Google Calendar)?
- Task management (Asana, Trello)?
- Communication (Slack channels)?
- Preferred dashboard style?

---

### Communication Patterns

**Question:** How did communication about staffing happen last year?

**Ask:** You  
**Why it matters:** Informs notification and communication design  
**Validation:** Your experience  
**Priority:** LOW - can observe and adjust

**Follow-up questions:**
- What Slack channels were used?
- How many DMs did you get?
- Were there email blasts?
- What worked well vs. poorly?

---

### Success Metrics

**Question:** How will we measure if the new process is better?

**Ask:** Summer, You  
**Why it matters:** Need to define success  
**Validation:** Agreement on metrics  
**Priority:** LOW - can define but good to align

Proposed metrics:
- Hours saved per week for Summer
- Number of last-minute panics
- Time to answer "what's the current state?"
- Percentage of self-service shift changes
- Zero coverage gaps
- Zero over-allocations

---

## Interview Guides by Stakeholder

### Interview: James Turner (Pass Allocation - Ryan Gavin's Org)

**Time needed:** 30 minutes  
**Best format:** Video call or in-person

**Questions:**
1. Walk me through your process for allocating passes last year
2. What tool/system do you use? (Rainfocus? Spreadsheet? Other?)
3. How do you decide who gets passes?
4. When do you make allocation decisions?
5. How do you track: applications, approvals, assignments?
6. What was hardest about the process?
7. What would make your job easier this year?
8. Can I see the tool you use (screen share)?

**Deliverable:** Document the process, get access to tools if possible

---

### Interview: Ria Mancoosh (Pass Allocation - Rob Seaman's Org)

**Time needed:** 30 minutes  
**Best format:** Video call or in-person

**Questions:**
1. Walk me through your process for allocating passes last year
2. What tool/system do you use?
3. Is your process similar to James Turner's or different?
4. How do you decide who gets passes?
5. When do you make allocation decisions?
6. How do you coordinate with James (if at all)?
7. What was hardest about the process?
8. What would make your job easier this year?

**Deliverable:** Document the process, identify differences from James's process

---

### Interview: Dustin Burnett (Event Floor Lead)

**Time needed:** 45 minutes  
**Best format:** Video call or in-person

**Questions:**
1. Walk me through staffing requirements for different areas
2. How do you determine how many people per shift?
3. Are there formulas or rules of thumb you use?
4. What roles exist (booth volunteer, demo specialist, etc.)?
5. What skills/training does each role need?
6. Which roles can be non-Slack people?
7. How do requirements differ between: campground booth, SICs, sessions?
8. What causes under-staffing in practice?
9. How do you handle last-minute changes during the event?
10. What would make staffing coordination easier?

**Deliverable:** Documented staffing requirement formulas and role taxonomy

---

### Interview: Marika's Team (Sessions & Scheduling)

**Time needed:** 30 minutes  
**Best format:** Video call or in-person

**Questions:**
1. Where do you track sessions (SICs, spoken sessions)?
2. Is Rainfocus the source of truth?
3. How do you use Rainfocus backend?
4. Can you export data? Show me how?
5. What data is available for export?
6. Is there a Rainfocus API?
7. How do you coordinate demo specialists for sessions?
8. How do you handle scheduling conflicts?
9. What's hardest about sessions/scheduling?
10. What would make your job easier?

**Deliverable:** Understand Rainfocus access, get export capability tested

---

### Self-Investigation: Summer

**These tasks Summer should do herself:**

1. **Test Rainfocus export**
   - Log into Rainfocus backend
   - Find export functionality
   - Export sample data (if any exists yet)
   - Document: what data, what format, how long it takes

2. **Map your current workspace**
   - List tools you use day-to-day
   - Note what you use them for
   - Identify pain points with current tools
   - Think about ideal workflow

3. **Review last year's artifacts** (from you)
   - Any spreadsheets, docs, or notes from 2025
   - Identify what you'll inherit vs. start fresh

---

## Tracking Discovery Progress

| Question | Priority | Owner | Status | Answer | Date |
|----------|----------|-------|--------|--------|------|
| Event footprint source of truth | P1 | Summer | ⬜ Not Started | | |
| Sessions catalog location | P1 | Summer | ⬜ Not Started | | |
| Pass allocation tool | P1 | Summer | ⬜ Not Started | | |
| Pass allocation process | P1 | Summer | ⬜ Not Started | | |
| Rainfocus export capability | P1 | Summer | ⬜ Not Started | | |
| Rainfocus API access | P2 | Summer | ⬜ Not Started | | |
| Multi-stage tracking | P1 | Summer | ⬜ Not Started | | |
| Staffing requirements docs | P2 | Summer | ⬜ Not Started | | |
| Role taxonomy | P2 | Summer | ⬜ Not Started | | |
| Timeline/deadlines | P2 | Summer | ⬜ Not Started | | |
| Last-minute change causes | P3 | Summer | ⬜ Not Started | | |
| Current change process | P3 | You | ⬜ Not Started | | |
| Historical data | P3 | Summer | ⬜ Not Started | | |

**Status key:**
- ⬜ Not Started
- 🔄 In Progress
- ✅ Complete
- ⚠️ Blocked

---

**Next Steps:**
1. Summer reviews this document
2. Schedule interviews with stakeholders
3. Conduct investigations
4. Update tracking table as answers come in
5. Synthesize findings in `/research/discovery-findings.md`

**Last Updated:** May 21, 2026
