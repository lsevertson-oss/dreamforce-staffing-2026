# Constraints: Dreamforce Staffing Optimization

## Timeline Constraints

### Fixed Deadlines
- **Event Date:** September 15-17, 2026 (immovable)
- **Project Start:** May 21, 2026
- **Available Time:** ~4 months from start to event
- **Testing Window:** Must be ready by end of July for August testing

### Phase Deadlines
- **Discovery:** End of May (3 weeks from start)
- **Design:** End of June (2 months from start)
- **Implementation:** End of July (2.5 months from start)
- **Testing:** August (1 month before event)
- **Execution:** September 15-17

### Staffing Timeline (Relative to Event)
These dates are estimates based on last year:
- **6 months out:** Event footprint planning begins
- **4 months out:** Pass allocations decided (rough numbers)
- **3 months out:** Applications open
- **2 months out:** Approvals and pass assignments
- **1 month out:** Shift signups and scheduling
- **2 weeks out:** Final confirmations
- **1 week out:** Last-minute changes begin
- **Day of:** Real-time coordination

**Implication:** Tools must be ready well before they're needed. Can't build pass allocation tool in August when it's needed in June.

## Resource Constraints

### People & Time
- **Summer's availability:** Part-time (has other responsibilities)
- **Your availability:** Limited (advisor role only)
- **No dedicated dev team:** Relying on AI-assisted development
- **Stakeholder time:** Everyone is busy, need to batch requests
- **Subject matter experts:** Limited access (Dustin, James, Ria, Marika's team)

### Budget
- **Unknown total budget:** Need to clarify
- **Probably limited:** Can't buy expensive enterprise software
- **Free tools preferred:** Google Workspace, open source
- **Cloud costs:** Keep minimal (serverless, low usage)

### Technical Resources
- **No backend infrastructure:** Can't host complex applications
- **No DevOps team:** Self-service deployment only
- **Limited access:** Can't change vendor systems (Rainfocus, Staffing Force)
- **Security requirements:** Must use approved tools and authentication

## Technical Constraints

### System Access
- **Rainfocus:** Backend is hard to use, limited access
- **Staffing Force:** Employee interface only, no admin access
- **No API access:** Likely can't integrate programmatically with vendor systems
- **Export only:** Probably limited to manual CSV/Excel exports
- **Read-only data:** Can't write back to Rainfocus programmatically

### Data Constraints
- **No real-time sync:** Data from Rainfocus will be point-in-time
- **Manual updates:** Changes in tools won't auto-update Rainfocus
- **Data quality:** Exports may have inconsistent formatting
- **Incomplete data:** Some info may not be in Rainfocus
- **Access control:** Can't give everyone access to all data

### Technical Complexity
- **Keep it simple:** No time for complex architecture
- **Must be maintainable:** Summer needs to maintain after you're gone
- **Must be reliable:** Can't risk tools breaking during event
- **Must have fallback:** Manual process for every automation

### Platform Constraints
- **Google Workspace:** Primary platform (what Slack uses)
- **Browser-based preferred:** No desktop apps to install
- **Mobile-friendly needed:** Summer checks things on phone
- **SSO required:** Must use Slack/Google authentication

## Organizational Constraints

### Decision-Making Authority
- **Summer is not in charge of everything:** Many decisions made by others
- **Pass allocation:** Decided by org leaders (Ryan Gavin, Rob Seaman)
- **Event footprint:** Decided by Strategic Events
- **Session content:** Decided by session owners
- **Staffing lead role:** Coordinate and track, not command and control

### Organizational Boundaries
- **Multiple orgs:** Marketing, product, sales, executives
- **Competing priorities:** Everyone wants passes
- **Politics:** Pass allocation is sensitive
- **Distributed ownership:** Session owners manage their own staffing
- **Vendor relationships:** Strategic Events manages vendors

### Change Management
- **New process anxiety:** People may resist changes from last year
- **Trust building needed:** Summer is new, needs to earn confidence
- **Gradual adoption:** Can't force everyone to use new tools immediately
- **Communication overhead:** Need to explain changes and get buy-in

## Information Constraints

### Known Unknowns
These things are unclear and block design decisions:
- Source of truth for event footprint
- Where sessions are cataloged
- Pass allocation process and tools
- Rainfocus data export capabilities
- Staffing requirement formulas
- Timeline for when decisions are made

### Access to Information
- **Tribal knowledge:** Much is in people's heads (Dustin, you)
- **Undocumented processes:** Last year's process not written down
- **Scattered documentation:** Info in emails, Slack, random docs
- **Historical data:** May not have access to prior years' data

### Communication Gaps
- **Async required:** Can't expect real-time responses from stakeholders
- **Time zones:** Not relevant (all in US) but schedules vary
- **Meeting overhead:** Hard to get everyone in same room
- **Email overload:** People may miss important messages

## Scope Constraints

### In Scope
- Dreamforce 2026 staffing process
- Jobs-to-be-done analysis
- Automation opportunities
- Tools for Summer
- Process documentation

### Out of Scope
- Other conferences (for now)
- Session content planning
- Event footprint decisions
- Vendor management
- Changing Rainfocus/Staffing Force themselves

### Boundaries
- **Can't change:** How Rainfocus or Staffing Force work
- **Can influence:** How Slack uses these systems
- **Can automate:** Tasks Summer does manually
- **Can't require:** Others to use our tools (must provide value to get adoption)

## Quality Constraints

### Must Be Reliable
- **Zero data loss:** Can't lose pass assignments or schedules
- **Accurate calculations:** Staffing requirements must be correct
- **Audit trail:** Need to track who changed what when
- **Backup plans:** Manual process for every automated step

### Must Be Usable
- **Summer must understand it:** Not too complex or technical
- **Quick to learn:** No extensive training required
- **Self-explanatory:** Documentation built into tools
- **Error prevention:** Hard to make mistakes

### Must Be Maintainable
- **Summer can maintain:** After you're gone
- **Simple architecture:** Easy to understand and debug
- **Well documented:** Code comments, README files
- **No exotic dependencies:** Standard tools only

## Risk Tolerance

### Low Risk Tolerance For
- **Pass over-allocation:** Very bad to waste expensive passes
- **Under-staffing:** Very bad to have gaps in coverage
- **Data breaches:** Employee data is sensitive
- **System downtime:** During event would be catastrophic

### Higher Risk Tolerance For
- **Feature completeness:** 80/20 solution is fine
- **Polish:** Functional beats pretty
- **Automation coverage:** Don't need to automate everything
- **Technical elegance:** Hacky solutions OK if they work

## Success Constraints

### Definition of Success
Success is not "perfect automation" but:
- 50%+ reduction in Summer's manual hours
- Zero critical failures (over/under-staffing)
- Summer feels confident and in control
- Process documented for next year
- Tools actually get used (adoption)

### Good Enough Threshold
We're successful if:
- High-impact pain points are solved
- Summer can see current state in <1 minute
- Most shift swaps are self-service
- Documentation exists for manual backup
- Lessons learned captured

**Don't need:**
- 100% automation
- Perfect UI
- Real-time integration with all systems
- Zero manual work
- Enterprise-grade software

## Assumptions We're Making

Document assumptions so we can validate them:

1. **Summer will have access to Rainfocus backend** (probably true, but confirm)
2. **We can export data from Rainfocus** (probably manually, but confirm)
3. **Pass allocations happen before shift signups** (based on last year, but confirm)
4. **Staffing requirements can be calculated** (not purely subjective, but validate with Dustin)
5. **Google Sheets won't hit limits** (probably fine, but monitor)
6. **Stakeholders will answer discovery questions** (they're busy, but we need this info)

**Action:** Validate these assumptions during discovery phase.

## Dependencies

### Blocking Dependencies
**Can't proceed without:**
- Discovery questions answered
- Source of truth locations identified
- Rainfocus export tested
- Staffing requirements documented

### Non-Blocking Dependencies
**Nice to have but can work around:**
- API access to Rainfocus
- Direct integration with Staffing Force
- Automated notifications
- Real-time sync

### External Dependencies
**Things outside our control:**
- Strategic Events providing event footprint info
- Pass allocators using our tools
- Rainfocus working properly
- Stakeholder availability for interviews

## What We Can Control vs. Can't Control

### Can Control
- What tools we build
- How we document the process
- What we automate
- Summer's experience with our tools
- Timeline for our deliverables

### Can Influence
- How others use our tools
- Data quality in Rainfocus
- Process improvements across stakeholders
- Communication patterns

### Can't Control
- Rainfocus capabilities
- Staffing Force features
- When Strategic Events provides info
- Pass allocation decisions by orgs
- People canceling last-minute

**Strategy:** Focus energy on what we can control, design around what we can't.

---

**Last Updated:** May 21, 2026  
**Review:** Validate assumptions during discovery phase
