# TODO: Dreamforce Staffing Optimization

**Last Updated:** May 21, 2026  
**Phase:** Discovery & Mapping

## Now (This Week: May 21-27)

### High Priority
- [ ] Complete JTBD analysis document (jobs-to-be-done mapping)
  - Document every job the staffing lead does
  - Map timing relative to event
  - Identify pain points and time requirements
  - Spot automation opportunities
  - **Owner:** Claude + You
  - **Deliverable:** `/deliverables/jtbd-analysis.md`

- [ ] Generate discovery questions for Summer
  - Questions about source of truth locations
  - Questions about data access
  - Questions about current tools and processes
  - **Owner:** Claude + You
  - **Deliverable:** `/research/discovery-questions.md`

- [ ] Document current state process map
  - End-to-end flow from planning to execution
  - Show all systems and handoffs
  - Highlight pain points
  - **Owner:** You (with Claude's help)
  - **Deliverable:** `/docs/current-state-process.md`

### Medium Priority
- [ ] Create stakeholder interview guide
  - Questions for Dustin Burnett (staffing requirements)
  - Questions for James Turner (pass allocation)
  - Questions for Ria Mancoosh (pass allocation)
  - Questions for Marika's team (sessions/scheduling)
  - **Owner:** Claude
  - **Deliverable:** `/research/interview-guides.md`

- [ ] Brainstorm automation opportunities
  - Initial list based on current knowledge
  - Prioritized by estimated ROI
  - **Owner:** Claude + You
  - **Deliverable:** `/deliverables/automation-opportunities.md`

### Low Priority
- [ ] Research similar tools/solutions
  - See if other companies have solved this
  - Check if any products exist for conference staffing
  - **Owner:** Claude
  - **Deliverable:** `/research/market-scan.md`

## Next (Week of May 28 - June 3)

### Summer's Discovery Tasks
- [ ] Investigate source of truth for event footprint
  - Ask Strategic Events or Alyssa
  - Document where info lives and when it's available
  
- [ ] Confirm where sessions are cataloged
  - Talk to Marika's team
  - Understand if Rainfocus is source of truth
  
- [ ] Understand pass allocation process
  - Interview James Turner (Ryan Gavin's org)
  - Interview Ria Mancoosh (Rob Seaman's org)
  - Document the tool(s) they use
  
- [ ] Test data export from Rainfocus
  - See what data can be exported
  - Check format and completeness
  - Note any limitations

### Analysis Tasks
- [ ] Synthesize discovery findings
  - Compile answers from Summer's investigation
  - Update MEMORY.md with confirmed facts
  - Identify remaining gaps
  
- [ ] Prioritize automation opportunities
  - Based on actual data access and constraints
  - Create implementation roadmap
  
- [ ] Interview Dustin Burnett
  - Document staffing requirement formulas
  - Understand what roles exist
  - Learn which roles can be non-Slack people

## Later (June+)

### Design Phase
- [ ] Create dashboard mockups for Summer
- [ ] Design self-service workflows
- [ ] Design automation architecture
- [ ] Get stakeholder feedback on designs

### Implementation Phase
- [ ] Build pass allocation calculator
- [ ] Build staffing requirements calculator
- [ ] Create Summer's dashboard
- [ ] Build self-service shift swap workflow
- [ ] Create process documentation

### Testing Phase
- [ ] Summer tests all tools
- [ ] Train Summer on new process
- [ ] Test with real data
- [ ] Create quick reference guides

## Blocked (Waiting On)

- [ ] Pass allocation process details
  - **Blocked by:** Need Summer to interview James & Ria
  - **Needed for:** Pass allocation automation design
  
- [ ] Rainfocus data access
  - **Blocked by:** Need to test what's exportable
  - **Needed for:** Integration architecture
  
- [ ] Staffing requirement formulas
  - **Blocked by:** Need Dustin interview
  - **Needed for:** Staffing calculator design
  
- [ ] Event footprint source of truth
  - **Blocked by:** Need Summer to investigate
  - **Needed for:** Timeline and planning automation

## Questions to Resolve

- [ ] What's our budget for tools/integrations?
- [ ] Who is the backup if Summer is unavailable?
- [ ] Should session owner staffing be in scope?
- [ ] How much integration with Rainfocus is realistic?
- [ ] What decisions require human judgment vs. can be automated?

## Ideas / Future Enhancements

- [ ] Predictive analytics for likely cancellations
- [ ] Automated shift swap matching
- [ ] Real-time dashboard during event
- [ ] Mobile app for day-of coordination
- [ ] Integration with Slack for notifications
- [ ] Generalize process for all Slack conferences
- [ ] Historical data analysis to improve staffing formulas

## Completed

*Tasks will be moved here as they're completed*

---

## Quick Add Template

When adding a task, use this format:

```markdown
- [ ] Task description
  - **Owner:** Who's responsible
  - **Deliverable:** What gets created
  - **Blocked by:** Any blockers
  - **Priority:** High/Medium/Low
```

## Priority Definitions

- **High:** Blocking other work or time-sensitive
- **Medium:** Important but not blocking
- **Low:** Nice to have, can wait
