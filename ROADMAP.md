# Roadmap: Dreamforce 2026 Staffing Optimization

**Event Date:** September 15-17, 2026  
**Project Start:** May 21, 2026

## Timeline Overview

```
May 2026          Jun 2026          Jul 2026          Aug 2026          Sep 2026
│                 │                 │                 │                 │
│ Discovery       │ Design          │ Implementation  │ Testing         │ Execution
│ & Mapping       │ & Validation    │                 │ & Training      │
│                 │                 │                 │                 │
└─────────────────┴─────────────────┴─────────────────┴─────────────────┴──────────
```

## Phase 1: Discovery & Mapping (May 2026) - CURRENT

**Goal:** Understand current process and identify automation opportunities

### Week 1: May 21-27
- [x] Project kickoff and structure creation
- [ ] Document current staffing process from your experience
- [ ] Map jobs-to-be-done for staffing lead role
- [ ] Generate discovery questions for Summer
- [ ] Create initial JTBD analysis document

### Week 2: May 28 - June 3
- [ ] Summer investigates source of truth questions
- [ ] Interview Dustin Burnett about staffing requirements
- [ ] Interview James Turner about pass allocation process
- [ ] Interview Ria Mancoosh about Rob Seaman's org process
- [ ] Document findings in `/research/`

### Deliverables
- [ ] Complete JTBD analysis with automation opportunities
- [ ] Discovery questions answered
- [ ] Current state process map
- [ ] Pain points prioritized by impact

## Phase 2: Validation & Design (June 2026)

**Goal:** Validate findings and design optimized workflows

### Week 1: June 4-10
- [ ] Validate source of truth locations with Strategic Events
- [ ] Confirm data access/export capabilities from Rainfocus
- [ ] Document staffing requirement formulas with Dustin
- [ ] Map current data flows between systems

### Week 2: June 11-17
- [ ] Design automation architecture
- [ ] Prioritize automation opportunities (ROI vs. effort)
- [ ] Design dashboard mockups for Summer
- [ ] Design self-service workflows

### Week 3: June 18-24
- [ ] Review designs with Summer
- [ ] Review with key stakeholders (Dustin, Marika's team)
- [ ] Refine based on feedback
- [ ] Finalize implementation plan

### Week 4: June 25 - July 1
- [ ] Create detailed technical specs
- [ ] Identify tooling needs (scripts, integrations, dashboards)
- [ ] Set up development environment
- [ ] Begin high-priority automation prototypes

### Deliverables
- [ ] Validated source of truth documentation
- [ ] Automation architecture document
- [ ] Dashboard designs approved by Summer
- [ ] Prioritized implementation backlog

## Phase 3: Implementation (July 2026)

**Goal:** Build automation tools and process improvements

### Week 1: July 2-8
- [ ] Build pass allocation model/calculator
- [ ] Create staffing requirements calculator
- [ ] Set up data import from Rainfocus (if possible)
- [ ] Build first version of Summer's dashboard

### Week 2: July 9-15
- [ ] Build self-service shift swap workflow
- [ ] Create automated notification system
- [ ] Build reporting/analytics views
- [ ] Create process documentation for Summer

### Week 3: July 16-22
- [ ] Build integration between systems (if feasible)
- [ ] Create early warning system for under-staffed shifts
- [ ] Build checklist/timeline tracker for Summer
- [ ] Develop training materials

### Week 4: July 23-29
- [ ] Polish and refine all tools
- [ ] Create backup/manual processes for each automation
- [ ] Document troubleshooting guides
- [ ] Prepare for testing phase

### Deliverables
- [ ] Working dashboard for Summer
- [ ] Automated tools deployed and tested
- [ ] Process documentation complete
- [ ] Training materials ready

## Phase 4: Testing & Training (August 2026)

**Goal:** Validate tools work and Summer is confident using them

### Week 1: August 1-7
- [ ] Summer testing: pass allocation modeling
- [ ] Summer testing: staffing requirements calculation
- [ ] Summer testing: dashboard navigation
- [ ] Gather feedback and identify bugs

### Week 2: August 8-14
- [ ] Fix bugs and issues from Week 1 testing
- [ ] Summer testing: self-service workflows
- [ ] Summer testing: reporting and analytics
- [ ] Train backup person (if applicable)

### Week 3: August 15-21
- [ ] End-to-end process walkthrough with Summer
- [ ] Test with real data (if available yet)
- [ ] Stress test: what if scenarios (mass cancellations, etc.)
- [ ] Refine based on learnings

### Week 4: August 22-28
- [ ] Final polish and refinements
- [ ] Create quick reference guides
- [ ] Set up monitoring/alerting for tools
- [ ] Go/no-go decision for using new process

### Deliverables
- [ ] All tools tested and validated by Summer
- [ ] Summer trained and confident
- [ ] Quick reference guides created
- [ ] Contingency plans documented

## Phase 5: Execution (September 2026)

**Goal:** Successfully staff Dreamforce 2026 with new process

### Week 1: September 1-7 (Pre-Event)
- [ ] Summer uses tools for final assignments
- [ ] Monitor for issues, provide support
- [ ] Handle last-minute changes with new workflows
- [ ] Final staffing confirmed

### Week 2: September 8-14 (Pre-Event)
- [ ] Real-time support as Summer manages final week changes
- [ ] Test self-service capabilities with staff
- [ ] Prepare for day-of support

### Event Week: September 15-17
- [ ] Monitor dashboard and tools during event
- [ ] Support Summer with any issues
- [ ] Track self-service adoption and success
- [ ] Document any problems for improvement

### Post-Event: September 18-30
- [ ] Debrief with Summer: what worked, what didn't
- [ ] Analyze metrics: time saved, accuracy, self-service adoption
- [ ] Document lessons learned
- [ ] Update tools and process based on learnings
- [ ] Create final report and recommendations

### Deliverables
- [ ] Successful Dreamforce 2026 staffing execution
- [ ] Metrics report showing improvements
- [ ] Lessons learned document
- [ ] Updated process for future events

## Key Milestones

| Date | Milestone | Owner |
|------|-----------|-------|
| May 27 | Discovery questions delivered to Summer | You |
| June 3 | All discovery answers received | Summer |
| June 24 | Automation designs approved | Summer |
| July 29 | All tools built and ready for testing | You + Claude |
| August 28 | Summer trained and confident | Summer |
| September 15-17 | Dreamforce 2026 execution | Summer |
| September 30 | Post-event report complete | You + Summer |

## Dependencies & Critical Path

### Critical Dependencies
1. **Source of truth clarification** (blocking design phase)
2. **Rainfocus data access** (blocking some automations)
3. **Pass allocation timeline** (blocking modeling work)
4. **Stakeholder availability** (blocking validation)

### Critical Path
```
Discovery → Design → Pass Calculator → Dashboard → Testing → Execution
```

### Parallel Workstreams (Can happen concurrently)
- Self-service workflows
- Reporting/analytics
- Documentation
- Training materials

## Risk Factors

| Timeline Risk | Impact | Mitigation |
|--------------|--------|------------|
| Discovery delays into June | Medium | Have Summer focus on critical questions first |
| Rainfocus access blocked | High | Build tools that work with manual exports |
| Implementation takes longer | Medium | Prioritize must-have automations |
| August testing reveals major issues | High | Allow buffer time, have manual backup |
| Key stakeholder unavailable | Medium | Identify backup contacts early |

## Checkpoints

### End of May Checkpoint
- **Questions:** Is discovery complete? Do we have enough info to design?
- **Decision:** Proceed to design or extend discovery

### End of June Checkpoint
- **Questions:** Are designs validated? Is implementation plan realistic?
- **Decision:** Proceed to implementation or revise designs

### End of July Checkpoint
- **Questions:** Are tools working? Is Summer ready to test?
- **Decision:** Proceed to testing or extend development

### Mid-August Checkpoint
- **Questions:** Does Summer feel confident? Are tools reliable?
- **Decision:** Go/no-go on using new process for Dreamforce

## Success Indicators

By end of each phase, we should see:

- **May:** Clear understanding of problems and opportunities
- **June:** Validated designs that Summer is excited about
- **July:** Working tools that demonstrate value
- **August:** Summer confidently navigating new process
- **September:** Measurably better outcomes than last year

---

**Last Updated:** May 21, 2026  
**Next Review:** May 27, 2026 (End of Week 1)
