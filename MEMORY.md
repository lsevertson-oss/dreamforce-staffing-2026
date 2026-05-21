# Project Memory: Key Decisions & Context

This document captures important decisions, learnings, and context as the project progresses.

## Project Origin

**Date:** May 21, 2026  
**Context:** You (previous Dreamforce staffing lead) want to teach Summer Hash (new staffing lead) using an AI-first approach. Rather than just documenting last year's manual process, the goal is to identify jobs-to-be-done and automate wherever possible to minimize manual hours.

**Key Insight:** Last year was a "horror show" of manual work, system fragmentation, and last-minute chaos. We can do much better with automation and better processes.

## Key Decisions

### Decision: AI-First Approach
**Date:** May 21, 2026  
**Decision:** Use jobs-to-be-done framework and identify automation opportunities rather than just documenting manual process  
**Rationale:** More valuable to reduce Summer's workload than to just transfer your workload to her  
**Impact:** Changes project from documentation to optimization

### Decision: Dreamforce-First, Then Generalize
**Date:** May 21, 2026  
**Decision:** Focus on Dreamforce 2026 specifically, then extract learnings for other conferences  
**Rationale:** Dreamforce is most complex, solving it will inform other events  
**Impact:** Narrow scope initially, expand later

### Decision: Build Tools That Work With Exports
**Date:** May 21, 2026  
**Decision:** Assume we may not get direct API access to Rainfocus, design tools that work with exports/spreadsheets  
**Rationale:** Rainfocus is hard to use and may have limited API, can't depend on getting access  
**Impact:** Tools need to be flexible on data input methods

## Known Constraints

### Technical Constraints
- **Rainfocus backend is hard to use** - Likely limited API, may only have export capability
- **Multiple disconnected systems** - Rainfocus, Staffing Force, spreadsheets, Google Calendar
- **No control over vendor systems** - Can't change how Rainfocus or Staffing Force work
- **Limited development resources** - Relying on AI-assisted automation, not a dev team

### Organizational Constraints
- **Distributed decision making** - Multiple org leaders allocate passes
- **Session owners manage their own staffing** - Not centrally managed
- **Strategic Events controls event footprint** - Staffing lead doesn't decide what's built
- **Timeline is tight** - Event in September, starting in May

### Resource Constraints
- **Summer has other responsibilities** - Not 100% dedicated to Dreamforce
- **Your limited availability** - Can advise but not do all the work
- **Unknown budget** - May have constraints on tooling purchases

## Known Unknowns (Need Discovery)

### Critical Questions Needing Answers

1. **Event Footprint Source of Truth**
   - Where does Strategic Events document what Slack is building?
   - Who receives this info and when?
   - Status: Unknown, need to ask Strategic Events or Alyssa

2. **Sessions & Meetings Catalog**
   - Where does Marika's team track sessions (SICs, spoken sessions)?
   - Is Rainfocus the source of truth?
   - Who on PMM team owns this list?
   - Status: Unknown, need to ask Marika's team

3. **Pass Allocation Process**
   - Who decides how many passes each org gets?
   - What tool is used to track this?
   - When are allocations decided?
   - Status: Unknown, need to ask James Turner and Ria Mancoosh

4. **Multi-Stage Tracking**
   - Is apply → approve → assign → schedule all in Rainfocus?
   - Or partly in spreadsheets/email?
   - Status: Unknown, Summer needs to investigate

5. **Staffing Requirements**
   - Are there documented formulas (e.g., "2 demo specialists per booth shift")?
   - Or all tribal knowledge?
   - Status: Tribal knowledge, need to interview Dustin Burnett

### Lower Priority Questions

- Can we export data from Rainfocus programmatically?
- What causes most last-minute shift changes?
- What roles can be filled by non-Slack people?
- How far in advance are session details finalized?

## Key Learnings

### From Last Year's Experience

**Pain Point: Unclear Event Footprint**
- Hard to understand what Slack is building at the event
- Information felt gated or came late
- Made it hard to plan staffing needs

**Pain Point: Manual Pass Allocation**
- Cross-referencing pass allocations with staffing needs was time-consuming
- Multiple checks: apply, leader approval, pass assignment, shift signup
- Hard to track who was where in the pipeline

**Pain Point: System Fragmentation**
- Official system (Rainfocus) is hard to use
- People create parallel spreadsheets as workaround
- No single source of truth
- Lots of manual reconciliation

**Pain Point: Last-Minute Changes are Chaos**
- People DM or message in channels about cancellations
- Hard for them to find coverage
- They can't make changes themselves in Rainfocus
- Staffing lead has to manually coordinate everything

**Pain Point: Unclear Staffing Requirements**
- Requirements seem "made up" based on past experience
- Tribal knowledge from Dustin and prior events
- Not documented as formulas or rules

### What Worked Well Last Year

- *To be filled in as you recall*

## Stakeholder Map

### Primary Stakeholders

**Summer Hash** (New Staffing Lead)
- Primary user of new process and tools
- Needs: Clarity, visibility, reduced manual work, confidence
- Constraints: Limited time, new to role

**You** (Previous Staffing Lead)
- Domain expert and advisor
- Provides: Process knowledge, context, validation
- Constraints: Limited ongoing availability

### Key Contributors

**Dustin Burnett** (Event Floor Lead)
- Knows staffing requirements from past events
- Expertise: What works on the ground, staffing formulas
- Need from him: Documented staffing requirements

**Marika's Team** (Sessions & Scheduling)
- Manages sessions and scheduling
- Uses Rainfocus backend
- Need from them: Source of truth for sessions, data access

**James Turner** (Pass Allocation - Ryan Gavin's Org)
- Allocates passes for marketing org
- May use Rainfocus backend
- Need from him: Process documentation, tool access

**Ria Mancoosh** (Pass Allocation - Rob Seaman's Org)
- Allocates passes for product/other orgs
- Parallel process to James
- Need from her: Process documentation, tool access

### Informed Stakeholders

**Alyssa Sachs** (Slack CMO)
- Leads "Slack at Dreamforce"
- Receives event footprint info from Strategic Events
- May need to escalate to her if blockers arise

**Strategic Events Team**
- Plans overall event footprint
- Works with external vendors
- Source of truth for what's being built

**Session Owners**
- Manage their own session staffing
- Not centrally coordinated
- May benefit from self-service tools

## Design Principles

These principles should guide all decisions in this project:

1. **Automate the automatable** - If it's rule-based, don't make a human do it
2. **Self-service over coordination** - Let people solve their own problems when possible
3. **Visibility over surprises** - Summer should always know current state
4. **Simple over clever** - 80/20 solutions that work beat perfect solutions that don't
5. **Backup plans always** - Manual fallback for every automation
6. **Reusable over one-off** - Design for other conferences too
7. **Summer's time is precious** - Ruthlessly prioritize her convenience

## Risks & Mitigations

### Risk: Can't Get Rainfocus API Access
**Impact:** High - Limits automation possibilities  
**Mitigation:** Design tools that work with exports/spreadsheets  
**Status:** Assumed constraint, designing around it

### Risk: Source of Truth Doesn't Exist
**Impact:** High - Hard to automate without clear data source  
**Mitigation:** Work with Strategic Events to create one  
**Status:** Need to investigate

### Risk: Timeline Too Aggressive
**Impact:** Medium - May not finish all planned automation  
**Mitigation:** Prioritize highest ROI items first, manual backup for rest  
**Status:** Monitoring

### Risk: Stakeholders Unresponsive
**Impact:** High - Blocks discovery and validation  
**Mitigation:** Identify backup contacts, escalate to Alyssa if needed  
**Status:** Not occurred yet

## Success Metrics

How we'll know this project succeeded:

### Quantitative
- 50%+ reduction in hours Summer spends on manual tasks
- 70%+ of shift swaps/cancellations handled without staffing lead
- <1 minute for Summer to answer "what's the current state?"
- Zero pass over-allocation incidents
- Zero double-booking incidents

### Qualitative
- Summer feels confident in the process
- Process is documented well enough for next year
- Learnings are applicable to other conferences
- Last-minute changes are manageable, not chaos

## Open Questions for Discussion

- Should we try to build integrations or just accept manual imports?
- How much should we try to centralize vs. keep distributed?
- What's the right balance of automation vs. human oversight?
- Should session owner staffing be in scope or truly separate?

---

**Last Updated:** May 21, 2026  
**Next Review:** End of May after discovery complete
