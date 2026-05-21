# Project Brief: Dreamforce 2026 Staffing Optimization

## Executive Summary

Transform Dreamforce staffing from a manual, spreadsheet-driven process into an AI-optimized workflow that reduces manual hours, improves visibility, and enables self-service for common requests.

## Background

### Current State Problems

Last year's Dreamforce staffing involved significant manual effort and pain points:

1. **Unclear event footprint** - Difficulty understanding what Slack is building (booths, sessions, meetings)
2. **Unknown staffing requirements** - Manually determining needs for each area and which roles can fill them
3. **Pass allocation complexity** - Multiple orgs (Ryan Gavin's marketing, Rob Seaman's areas) with unclear allocation process
4. **Multi-stage tracking nightmare** - Four stages (apply → leader approve → pass assignment → shift signup) tracked across multiple systems
5. **System fragmentation** - Rainfocus, Staffing Force, spreadsheets, Google Calendar with no single source of truth
6. **Last-minute chaos** - "Horror show" of cancellations and substitutions with no self-service capability
7. **Hard-to-use tools** - Rainfocus backend is difficult to use, causing people to maintain parallel spreadsheets

### What Makes This Complex

- **Cross-org coordination** - Multiple Slack orgs need passes (marketing, product, sales support, etc.)
- **Role flexibility** - Some staffing needs can be filled by non-Slack-specific people
- **Multiple work streams** - Booth shifts (via Staffing Force), sessions (via session owners), executive/producer roles
- **Vendor relationships** - Strategic Events works with external vendors on event footprint
- **Parallel systems** - Rainfocus is official system but hard to use, so people create shadow spreadsheets

## Project Objectives

### Primary Goals

1. **Map jobs-to-be-done** - Identify every task the staffing lead performs and when
2. **Identify automation opportunities** - Determine which tasks can be AI-assisted or fully automated
3. **Improve visibility** - Create dashboard showing current state and what needs to be done next
4. **Enable self-service** - Let people handle common requests (shift swaps, cancellations) without staffing lead intervention
5. **Establish source of truth** - Clarify where information lives and create integration if needed

### Success Metrics

- **Time saved** - Reduce staffing lead hours by 50%+ through automation
- **Visibility** - Summer can answer "what's the current state?" in < 1 minute
- **Self-service adoption** - 70%+ of shift swaps/cancellations handled without staffing lead
- **Accuracy** - Zero pass over-allocation or double-booking incidents
- **Reusability** - Process can be adapted for other Slack conferences

## Scope

### In Scope

- Jobs-to-be-done analysis for Dreamforce 2026 staffing
- Process mapping and timeline dashboard
- Identification of automation opportunities
- Discovery of source-of-truth systems and data flows
- Recommendations for tools/integrations to build
- Handoff documentation for Summer Hash
- Learnings applicable to other conferences

### Out of Scope (For Now)

- Building custom integrations with Rainfocus/Staffing Force (may come later)
- Managing other conferences' staffing (focus on Dreamforce first)
- Session content planning (that's session owners' responsibility)
- Event footprint decisions (that's Strategic Events' responsibility)
- Vendor selection or management

### Open Questions (Discovery Needed)

These questions need answers before we can fully optimize:

1. **Event Footprint Source of Truth**
   - Where does Strategic Events document what Slack is building?
   - Who receives this information and when?
   - Is there a timeline for when decisions are finalized?

2. **Pass Allocation Process**
   - Who decides how many passes each org gets?
   - When is this decided?
   - What tool is used to track allocations? (Rainfocus backend?)
   - Is there a formal request/approval process?

3. **Sessions & Meetings Tracking**
   - Where does Marika's team catalog sessions (SICs, spoken sessions)?
   - Is Rainfocus the source of truth or is there another system?
   - Who on PMM team owns the session list?

4. **Multi-Stage Process Tracking**
   - Is the apply → approve → assign → schedule flow all in Rainfocus?
   - Or are parts tracked in spreadsheets/email?
   - Can we get data export access from Rainfocus?

5. **Staffing Requirements**
   - Are there documented formulas (e.g., "2 demo specialists per booth shift")?
   - Or is this all tribal knowledge from Dustin and prior experience?
   - What roles exist and which can be filled by non-Slack people?

## Stakeholders

### Primary

- **Summer Hash** - New staffing lead, primary user of new process
- **You (Previous Staffing Lead)** - Domain expertise, process knowledge

### Key Contributors

- **Dustin Burnett** - Event floor lead, knows staffing requirements from past events
- **Marika's team** - Manages sessions and scheduling, uses Rainfocus
- **James Turner** - Manages pass allocation for Ryan Gavin's org
- **Ria Mancoosh** - Manages pass allocation for Rob Seaman's org

### Informed

- **Alyssa Sachs** - Slack CMO, "Slack at Dreamforce" lead
- **Strategic Events team** - Provides event footprint information
- **Session owners** - Manage their own session staffing
- **All Dreamforce attendees** - Will benefit from better self-service

## Approach

### Phase 1: Discovery & Mapping (Current)

1. Document current process based on your experience
2. Identify all jobs-to-be-done for staffing lead role
3. Map data flows and system dependencies
4. Generate discovery questions for Summer to investigate
5. Identify automation opportunities

### Phase 2: Validation (After Discovery)

1. Summer confirms source of truth locations
2. Verify data access and export capabilities
3. Validate staffing requirement formulas with Dustin
4. Confirm stakeholder roles and responsibilities

### Phase 3: Design (June 2026 Target)

1. Design automation workflow for high-ROI opportunities
2. Create dashboard/visibility tools
3. Design self-service capabilities
4. Document optimized process

### Phase 4: Implementation (July-August 2026)

1. Build automation tools (scripts, integrations, dashboards)
2. Create process documentation and training materials
3. Test with Summer and key stakeholders
4. Refine based on feedback

### Phase 5: Execution (September 2026)

1. Run optimized process for Dreamforce 2026
2. Monitor and support Summer throughout event
3. Capture learnings and improvements
4. Document for future events

## Constraints

### Technical

- **Rainfocus limitations** - Backend is hard to use, may have limited API/export
- **System fragmentation** - Multiple disconnected tools (Rainfocus, Staffing Force, spreadsheets)
- **No direct control** - We can't change how Rainfocus or Staffing Force work
- **Data access** - May have limited ability to export data programmatically

### Organizational

- **Multiple decision makers** - Pass allocation decided by org leaders
- **Distributed ownership** - Session owners manage their own staffing
- **Vendor dependencies** - Strategic Events works with external vendors
- **Timeline pressure** - Event is September, planning starts now

### Resources

- **Summer's time** - She has other responsibilities beyond Dreamforce
- **Your availability** - Limited time to advise and support
- **No dedicated dev team** - Relying on AI-assisted automation, not full custom development
- **Budget unknown** - May have constraints on tooling purchases

## Risks & Mitigations

| Risk | Impact | Likelihood | Mitigation |
|------|--------|-----------|------------|
| Rainfocus data access blocked | High | Medium | Document manual workarounds, build tools that work with exports |
| Key stakeholders unresponsive | High | Low | Identify backup contacts, escalate to Alyssa if needed |
| Source of truth doesn't exist | High | Medium | Create one in collaboration with Strategic Events |
| Timeline too aggressive | Medium | Medium | Focus on highest ROI automations first, manual backup plans |
| Automation complexity underestimated | Medium | Medium | Start with simple wins, iterate based on Summer's feedback |

## Success Criteria

### Must Have

- [ ] Complete jobs-to-be-done analysis with automation opportunities identified
- [ ] Dashboard showing Summer what needs to be done and when
- [ ] Discovery questions answered (source of truth locations, data access)
- [ ] Process documentation for Dreamforce 2026 staffing
- [ ] At least 3 high-impact automations implemented

### Should Have

- [ ] Self-service capability for shift swaps/cancellations
- [ ] Automated pass allocation recommendations based on staffing needs
- [ ] Integration between Rainfocus and tracking spreadsheets
- [ ] Early warning system for under-staffed shifts

### Nice to Have

- [ ] Predictive analytics for likely cancellations
- [ ] Automated shift swap matching
- [ ] Real-time dashboard during event
- [ ] Process generalized for other conferences

## Next Steps

1. **Review discovery questions** in `/research/discovery-questions.md`
2. **Summer investigates** source of truth locations and data access
3. **Complete JTBD analysis** in `/deliverables/jtbd-analysis.md`
4. **Prioritize automations** based on ROI and feasibility
5. **Schedule sync with Dustin** to validate staffing requirements

---

**Document Owner:** You (Previous Staffing Lead)  
**Last Updated:** May 21, 2026  
**Status:** Discovery Phase
