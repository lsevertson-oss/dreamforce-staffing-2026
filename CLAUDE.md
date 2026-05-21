# Claude Code Instructions: Dreamforce Staffing Optimization

## Project Context

This is an AI-first approach to optimizing Slack's Dreamforce 2026 staffing process. The goal is to identify jobs-to-be-done, find automation opportunities, and minimize manual hours required by Summer Hash (new staffing lead).

## Key Principles

1. **Jobs-to-be-done mindset** - Focus on what needs to be accomplished, not just documenting last year's process
2. **Automation-first** - Look for opportunities to reduce manual work through AI, scripts, or integrations
3. **Practical over perfect** - Deliver high-ROI improvements fast rather than perfect solutions slowly
4. **Self-service wherever possible** - Enable people to help themselves (shift swaps, cancellations)
5. **Visibility and clarity** - Summer should always know current state and what to do next

## Working with This Project

### When analyzing staffing workflows:
- Always ask "could this be automated?"
- Look for rule-based decisions that don't need human judgment
- Identify data that could be pulled automatically vs. manually entered
- Consider what could be self-service vs. requires staffing lead approval

### When creating documentation:
- Write for Summer Hash (new to this role) as primary audience
- Include context and "why" not just "how"
- Call out decisions points and who needs to make them
- Note dependencies and timing clearly

### When designing automation:
- Prioritize by ROI (time saved vs. effort to build)
- Consider data access constraints (Rainfocus may be locked down)
- Build tools that work with exports/spreadsheets as fallback
- Always have manual backup process documented

### When making recommendations:
- Show tradeoffs clearly (complexity vs. benefit)
- Identify what needs discovery/validation first
- Explain assumptions and how to validate them
- Consider reusability for other conferences

## Key Stakeholders

- **Summer Hash** - Primary user, new staffing lead
- **Dustin Burnett** - Event expert, knows staffing requirements
- **Marika's team** - Manages sessions and scheduling
- **James Turner** - Pass allocation (Ryan Gavin's org)
- **Ria Mancoosh** - Pass allocation (Rob Seaman's org)
- **Strategic Events** - Event footprint planning

## Systems Involved

- **Rainfocus** - Backend system (hard to use, may have limited data access)
- **Staffing Force** - Employee-facing staffing signup system
- **Spreadsheets** - Current workaround because Rainfocus is difficult
- **Google Calendar** - Session and shift tracking
- **Slack** - Communication and last-minute changes

## Common Tasks

### Research and Discovery
```bash
# When searching for prior context
grep -r "keyword" research/
grep -r "keyword" docs/
```

### Process Mapping
- Focus on data flows: where does information come from and where does it go?
- Identify decision points: who decides and based on what criteria?
- Note timing: when does this need to happen relative to event date?

### Automation Opportunities
Ask these questions:
1. Is this rule-based or requires human judgment?
2. Is the input data available programmatically?
3. How much time does this take manually?
4. What's the failure mode if automation breaks?
5. Can we build a 80/20 version quickly?

### Creating Deliverables
- Use markdown for all documentation
- Save to appropriate subfolder (context/, docs/, deliverables/, research/)
- Include last updated date and document owner
- Link related documents

## File Organization

```
/dreamforce-staffing-2026
  /context          - Background info (audience, constraints, terminology)
  /skills           - AI-assisted workflows
  /docs             - Technical documentation
  /research         - Discovery and investigation
  /deliverables     - Final outputs (JTBD analysis, recommendations)
  /tools            - Scripts, automations, prototypes
```

## Current Phase: Discovery & Mapping

Right now we are in discovery. Focus on:
1. Documenting current process based on prior experience
2. Mapping all jobs-to-be-done for staffing lead role
3. Identifying pain points and their root causes
4. Generating questions that need answers from stakeholders
5. Spotting automation opportunities

## Important Open Questions

These need answers before we can design solutions:
- Where is source of truth for event footprint (what Slack is building)?
- Where are sessions/meetings cataloged (Rainfocus? Elsewhere?)?
- What tool tracks pass allocations and approvals?
- Can we export data from Rainfocus programmatically?
- Are staffing requirements documented or just tribal knowledge?

## Commands and Workflows

### Start new research
```markdown
Create a new file in /research with:
- Date and researcher
- Questions being investigated
- Findings as they come in
- Open questions remaining
- Next steps
```

### Document a job-to-be-done
```markdown
Format:
**Job:** [What needs to be accomplished]
**When:** [Timing relative to event]
**Who:** [Current owner]
**Current Process:** [How it's done today]
**Pain Points:** [What's hard/time-consuming]
**Automation Opportunity:** [What could be automated]
**Priority:** [High/Medium/Low based on ROI]
```

### Propose an automation
```markdown
Format:
**Problem:** [What manual work this eliminates]
**Solution:** [What the automation does]
**Input:** [What data/info it needs]
**Output:** [What it produces]
**Complexity:** [Easy/Medium/Hard to build]
**Impact:** [Hours saved per event]
**Dependencies:** [What needs to be in place first]
**Fallback:** [Manual process if automation fails]
```

## Working with Summer

- She's new to this role, so explain context and reasoning
- She has limited time, so prioritize her questions
- She needs confidence in the new process, so show how it's better than manual
- She's the one who will live with these tools, so get her input on design

## Success Metrics

Good outcomes for this project:
- Summer spends 50%+ less time on manual tasks
- Summer can answer "what's the current state?" in under 1 minute
- 70%+ of shift swaps/cancellations happen without Summer's involvement
- Zero over-allocation or double-booking incidents
- Process documented well enough to reuse for other conferences

## Anti-patterns to Avoid

- Don't just document last year's process without questioning if it's optimal
- Don't design complex solutions when simple ones work
- Don't assume we can change how Rainfocus or Staffing Force work (we likely can't)
- Don't create automation without manual backup plan
- Don't prioritize low-ROI automation over high-impact improvements

## When You're Stuck

1. Check /research for answers to open questions
2. Note the blocker in TODO.md with what info is needed
3. Design around the constraint or note it as a dependency
4. Propose 2-3 options with different assumptions

## Timeline Awareness

- Event is September 15-17, 2026
- We're in May 2026 (4 months out)
- Discovery needs to complete by end of May
- Tools need to be ready by end of July for August testing
- This is aggressive, prioritize ruthlessly

---

**Last Updated:** May 21, 2026  
**Phase:** Discovery & Mapping
