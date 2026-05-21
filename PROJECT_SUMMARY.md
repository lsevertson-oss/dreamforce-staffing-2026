# Dreamforce 2026 Staffing Optimization - Project Summary

**Created:** May 21, 2026  
**Status:** Discovery Phase  
**Location:** `~/.aisuite/notebook/dreamforce-staffing-2026/`

---

## What This Is

A comprehensive AI-first approach to optimizing Slack's Dreamforce 2026 staffing operations. Rather than just documenting last year's manual process, we're identifying jobs-to-be-done and determining where automation can reduce Summer Hash's (new staffing lead) manual hours.

---

## Project Structure Created

```
dreamforce-staffing-2026/
│
├── 📋 Root Documentation
│   ├── README.md              # Project overview and quick start
│   ├── PROJECT_BRIEF.md       # Detailed scope, objectives, stakeholders
│   ├── PROJECT_SUMMARY.md     # This file - visual overview
│   ├── ROADMAP.md             # Timeline, phases, milestones
│   ├── TODO.md                # Active task list and priorities
│   ├── MEMORY.md              # Key decisions and project context
│   ├── CLAUDE.md              # Instructions for Claude Code
│   └── AGENTS.md              # AI agent configurations and prompts
│
├── 📁 context/                # Background information
│   ├── audience.md            # Who this is for (Summer, stakeholders)
│   ├── business-context.md   # Why this matters, business impact
│   ├── technical-context.md  # Systems, tools, tech constraints
│   ├── constraints.md         # What we can/can't do, dependencies
│   └── terminology.md         # Glossary of terms and acronyms
│
├── 📁 research/               # Discovery and investigation
│   └── discovery-questions.md # Critical questions needing answers
│
├── 📁 deliverables/           # Final outputs
│   └── jtbd-analysis.md       # Jobs-to-be-done with automation opportunities
│
├── 📁 docs/                   # Technical documentation
│   └── current-state-process.md # How staffing works today
│
└── 📁 skills/                 # AI-assisted workflows (placeholder)
```

---

## Key Deliverables

### 1. Jobs-to-Be-Done Analysis
**File:** `deliverables/jtbd-analysis.md`  
**Status:** DRAFT - needs validation

**What it contains:**
- 30+ jobs the staffing lead must accomplish
- Organized by phase (planning → execution → post-event)
- Pain points and time estimates for each job
- Automation opportunities rated by complexity and impact
- Prioritized implementation roadmap

**Key Findings:**
- Current process: 65-97 hours of mostly manual work
- Target: 50%+ reduction through automation (35-50 hours saved)
- **Quick wins identified:** 7 easy high-impact automations
- **High-impact complex:** 5 harder automations worth building
- **Human-required:** 9 jobs that need human judgment

### 2. Discovery Questions
**File:** `research/discovery-questions.md`  
**Status:** Ready for Summer to investigate

**What it contains:**
- 20+ critical questions organized by priority
- Who to ask for each question
- Why each answer matters for design
- Interview guides for key stakeholders
- Tracking table for progress

**Critical unknowns:**
- Where is event footprint source of truth?
- What tool tracks pass allocations?
- Can we export data from Rainfocus?
- Where are sessions cataloged?
- Are staffing requirements documented?

### 3. Current State Process Map
**File:** `docs/current-state-process.md`  
**Status:** DRAFT - based on your experience

**What it contains:**
- End-to-end process flow (6 phases)
- Detailed steps with actors, systems, pain points
- System integration map showing data flows
- Time estimates per phase
- Known unknowns that need discovery

**Key pain points identified:**
1. Last-minute changes are a "horror show"
2. Unclear event footprint and source of truth
3. Manual monitoring of shift signups (very time-consuming)
4. System fragmentation (Rainfocus ↔ spreadsheets)
5. Complex pass allocation modeling

### 4. Context Documentation
**Files:** `context/*.md`

**What it contains:**
- **Audience:** Summer Hash (primary) and all stakeholders
- **Business Context:** Why Dreamforce matters, org structure, risks
- **Technical Context:** Systems involved, integration points, constraints
- **Constraints:** Timeline, resources, what we can/can't control
- **Terminology:** Glossary of all terms, acronyms, role definitions

---

## Timeline at a Glance

```
May 2026 (NOW)          Jun 2026           Jul 2026           Aug 2026          Sep 15-17, 2026
│                       │                  │                  │                 │
│ Discovery            │ Design           │ Implementation   │ Testing         │ DREAMFORCE
│ & Mapping            │ & Validation     │                  │ & Training      │
│                       │                  │                  │                 │
└───────────────────────┴──────────────────┴──────────────────┴─────────────────┴──────────
   ↑ You are here
```

### Phase Breakdown

**Discovery (May 21 - June 3):**
- Document JTBD ✓
- Generate discovery questions ✓
- Summer investigates unknowns
- Interview stakeholders
- Validate automation opportunities

**Design (June 4-30):**
- Validate findings
- Design automation architecture
- Create dashboard mockups
- Prioritize implementation
- Get stakeholder approval

**Implementation (July 1-29):**
- Build top priority automations
- Create dashboard for Summer
- Build self-service workflows
- Process documentation

**Testing (August 1-28):**
- Summer tests all tools
- Train and validate
- Fix issues and refine
- Prepare for go-live

**Execution (September 15-17):**
- Run optimized process
- Support Summer during event
- Monitor and learn

---

## Automation Opportunities Identified

### 🟢 Quick Wins (7 total)
**Easy to build + High impact**

1. **Staffing Requirements Calculator** - Auto-calculate based on formulas
2. **Pass Allocation Model** - Model scenarios and recommendations
3. **Timeline Dashboard** - Public reference for dates and process
4. **Approval Tracking & Reminders** - Auto-remind pending approvals
5. **Shift Signup Monitor** - Dashboard with under-staffed shift alerts
6. **Confirmation Email Generation** - Auto-generate personalized emails
7. **FAQ Bot/Page** - Reduce repeated questions

**Est. Time Savings:** 20-30 hours

### 🟠 High-Impact Complex (5 total)
**Harder to build but worth it**

1. **Self-Service Cancellation & Swap** - Let people handle own changes
2. **Event Footprint Change Notification** - Alert when footprint updates
3. **Rainfocus Import Automation** - Auto-import vs. manual export
4. **Volunteer Recruitment Tracker** - Track outreach for gaps
5. **Pass Tracking Dashboard** - End-to-end pipeline view

**Est. Time Savings:** 30-40 hours

### 🔴 Keep Manual (9 total)
**Need human judgment**

- Final pass allocation decisions (political)
- Stakeholder negotiation
- Day-of emergency response
- Personal relationships
- Strategic decisions
- Session owner coordination

---

## Success Metrics

### Quantitative Goals
- ✅ 50%+ reduction in Summer's manual hours (35-50 hours saved)
- ✅ <1 minute to answer "what's the current state?"
- ✅ 70%+ of shift swaps/cancellations self-service
- ✅ Zero pass over-allocation incidents
- ✅ Zero coverage gaps during event

### Qualitative Goals
- Summer feels confident managing process
- Stakeholders find process clear and predictable
- Staff can self-service common requests
- Process documented for next year
- Learnings applicable to other conferences

---

## Key Stakeholders

### Primary
- **Summer Hash** - New staffing lead, primary user
- **You** - Previous staffing lead, advisor

### Key Contributors
- **Dustin Burnett** - Event floor lead, staffing expert
- **James Turner** - Pass allocation (Ryan Gavin's org)
- **Ria Mancoosh** - Pass allocation (Rob Seaman's org)
- **Marika's Team** - Sessions/scheduling, Rainfocus users

### Informed
- **Alyssa Sachs** - Slack CMO
- **Strategic Events** - Event footprint planning
- **Session Owners** - Individual session management

---

## Critical Path & Blockers

### Blocking Discovery Questions (Must Answer First)
1. Where is event footprint source of truth?
2. What tool tracks pass allocations?
3. Can we export data from Rainfocus?
4. Where are sessions cataloged?

**Action:** Summer to investigate by end of May

### Dependencies
- Rainfocus data access determines automation approach
- Staffing requirements (from Dustin) needed for calculator
- Pass allocation process understanding needed for modeling
- Timeline/deadlines needed for dashboard

### Risks
- **High Risk:** Can't get Rainfocus API access
  - **Mitigation:** Build tools that work with exports
- **Medium Risk:** Timeline too aggressive
  - **Mitigation:** Prioritize ruthlessly, focus on quick wins
- **Medium Risk:** Stakeholders unresponsive
  - **Mitigation:** Identify backups, escalate if needed

---

## Immediate Next Steps

### This Week (May 21-27)

**For You:**
- [ ] Review all generated documents
- [ ] Validate JTBD analysis accuracy
- [ ] Add any missing context or corrections
- [ ] Prioritize which jobs Summer finds most painful

**For Summer:**
- [ ] Review project documentation
- [ ] Read discovery-questions.md
- [ ] Schedule interviews with stakeholders
- [ ] Begin investigating source of truth locations

**For Claude:**
- [ ] Incorporate your feedback
- [ ] Refine JTBD analysis based on your corrections
- [ ] Fill in any gaps you identify

### Next Week (May 28 - June 3)

**Summer's Tasks:**
- Conduct stakeholder interviews
- Test Rainfocus export capability
- Document findings
- Answer critical discovery questions

**Your Tasks:**
- Interview Dustin about staffing requirements
- Validate process map
- Provide any missing context from 2025

---

## How to Use This Project

### For Summer
1. Start with `README.md` for overview
2. Review `PROJECT_BRIEF.md` for full context
3. Check `TODO.md` for your immediate tasks
4. Use `research/discovery-questions.md` as interview guide
5. Reference `context/` when you need background
6. Check `ROADMAP.md` to see timeline

### For You (Previous Staffing Lead)
1. Validate `deliverables/jtbd-analysis.md` - did we get it right?
2. Correct `docs/current-state-process.md` with missing details
3. Fill in unknowns based on your 2025 experience
4. Prioritize automations based on what was most painful
5. Add to `MEMORY.md` any important context we missed

### For Claude Code
1. Read `CLAUDE.md` for project-specific instructions
2. Use `AGENTS.md` for specialized agent prompts
3. Check `MEMORY.md` for key decisions and context
4. Update `TODO.md` as work progresses
5. Reference `context/` for constraints and background

---

## Project Principles

1. **Jobs-to-be-done mindset** - Focus on outcomes, not activities
2. **Automation-first** - Look for opportunities to reduce manual work
3. **Practical over perfect** - 80/20 solutions that work
4. **Self-service wherever possible** - Enable people to help themselves
5. **Visibility and clarity** - Summer should always know current state
6. **Document everything** - Next year's staffing lead should have great docs

---

## Questions or Feedback?

**Document Owner:** You (Previous Staffing Lead)  
**Project Status:** Discovery Phase  
**Last Updated:** May 21, 2026

**Next Review:** May 27, 2026 (end of Week 1)

---

## Quick Reference

| Document | Purpose |
|----------|---------|
| README.md | Start here - project overview |
| PROJECT_BRIEF.md | Full scope, objectives, stakeholders |
| THIS FILE | Visual summary and status |
| ROADMAP.md | Timeline and milestones |
| TODO.md | What needs to be done |
| MEMORY.md | Key decisions and context |
| jtbd-analysis.md | Jobs and automation opportunities |
| discovery-questions.md | Questions to investigate |
| current-state-process.md | How it works today |
| context/* | Background information |

**Location:** `~/.aisuite/notebook/dreamforce-staffing-2026/`
