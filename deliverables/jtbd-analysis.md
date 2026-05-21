# Jobs-to-Be-Done Analysis: Dreamforce Staffing Lead

**Purpose:** Comprehensive analysis of all jobs the staffing lead must accomplish  
**Approach:** Jobs-to-be-done framework focused on outcomes, not activities  
**Goal:** Identify automation opportunities to reduce manual hours by 50%+

**Status:** DRAFT - based on initial conversation, needs validation with Summer and stakeholders

---

## Executive Summary

The Dreamforce staffing lead role involves **[estimated] 20-30 distinct jobs** spanning 4 months from planning to post-event. Current process is heavily manual with significant pain points around:

1. **Visibility** - Hard to see current state across fragmented systems
2. **Coordination** - Manual back-and-forth between stakeholders
3. **Data management** - Copy/paste between Rainfocus and spreadsheets
4. **Last-minute changes** - No self-service, staffing lead is bottleneck

**Automation Opportunity:** Estimated 60-70% of jobs have automation potential
- **Quick wins (13):** Simple automations with immediate value
- **High-impact (8):** Complex but high time savings
- **Human-required (9):** Judgment calls that need human decision

---

## Phase 1: Pre-Event Planning (4-6 Months Before)

### Job 1.1: Understand Event Footprint

**Outcome:** Know what Slack is building at Dreamforce (booths, SICs, sessions)

**When:** 4-6 months before event (May-June for September event)

**Current Process:**
- Wait for Strategic Events to share event footprint
- Information comes via docs, emails, meetings
- Piece together what's being built
- Feel like information is gated or unclear

**Inputs Needed:**
- Event footprint document from Strategic Events
- Session list from PMM/Marika's team
- Timeline of when decisions are finalized

**Pain Points:**
- Unclear where source of truth lives
- Information trickles in slowly
- Hard to plan without complete picture
- Feels like working in the dark

**Time Required:** 2-4 hours initially + ongoing monitoring

**Automation Opportunity:** 🟡 MEDIUM
- Can't automate creation of event footprint (Strategic Events does this)
- **CAN automate:** Notification when footprint changes
- **CAN automate:** Dashboard showing what's known vs. TBD
- **CAN automate:** Summary of changes from last year

**Priority:** HIGH - needed for everything else

---

### Job 1.2: Calculate Staffing Requirements

**Outcome:** Know how many people needed for each area/shift/session

**When:** After event footprint known, ~3-4 months before event

**Current Process:**
- Review event footprint
- Apply tribal knowledge from Dustin and past experience
- Estimate needs: "probably 2 demo specialists per shift"
- Create spreadsheet with requirements
- "Made up based on what worked before"

**Inputs Needed:**
- Event footprint (booths, SICs, sessions, hours)
- Staffing formulas (from Dustin or past experience)
- Role definitions and capabilities
- Special requirements (product launches, VIP sessions)

**Pain Points:**
- No documented formulas, all tribal knowledge
- Hard to explain/justify numbers
- Easy to under or over-estimate
- Manual calculation in spreadsheet

**Time Required:** 4-8 hours initially + revisions as footprint changes

**Automation Opportunity:** 🟢 HIGH (Quick Win)
- **CAN automate:** Calculator based on formulas
- **CAN automate:** Apply rules to event footprint automatically
- **CAN automate:** Flag areas that seem under/over-staffed
- Example: "3 booths × 8 hours × 2 people per shift = 48 person-hours needed"

**Priority:** HIGH - drives pass allocation decisions

---

### Job 1.3: Determine Pass Allocation by Org

**Outcome:** Recommend how many passes each Slack org should receive

**When:** ~3 months before event, after staffing requirements known

**Current Process:**
- Look at staffing requirements
- Consider which orgs have people with needed skills
- Some roles can be non-Slack people (reduces pass need)
- Create allocation model in spreadsheet
- Present recommendations to pass allocators (James, Ria)
- Negotiate and adjust based on feedback

**Inputs Needed:**
- Staffing requirements by role
- Which roles can be filled by non-Slack people
- Org priorities and constraints
- Pass budget (total available)

**Pain Points:**
- Complex cross-referencing manually
- Hard to model different scenarios
- Allocation is political/sensitive
- Time-consuming to balance competing needs

**Time Required:** 6-10 hours for initial model + iterations

**Automation Opportunity:** 🟢 HIGH (Quick Win)
- **CAN automate:** Model that calculates recommended allocation
- **CAN automate:** "What-if" scenarios (if marketing gets X, product gets Y)
- **CAN automate:** Highlight mismatches (need 50 people, only 40 passes)
- **CANNOT automate:** Final decision (political judgment call)

**Priority:** HIGH - critical and time-consuming

---

### Job 1.4: Communicate Timeline and Expectations

**Outcome:** Everyone knows what will happen when and what they need to do

**When:** ~3 months before event, early in process

**Current Process:**
- Create timeline/calendar
- Send emails explaining process
- Post in Slack channels
- Repeat information many times
- Answer individual questions

**Inputs Needed:**
- Key dates (applications open, approvals due, shift signups, etc.)
- Process steps (apply → approve → assign → schedule)
- Who needs to do what when

**Pain Points:**
- People don't read emails
- Questions answered repeatedly
- Dates change and need to re-communicate
- No single reference people can check

**Time Required:** 4-6 hours initially + ongoing Q&A

**Automation Opportunity:** 🟢 HIGH (Quick Win)
- **CAN automate:** Public timeline dashboard everyone can reference
- **CAN automate:** Automated reminders at key milestones
- **CAN automate:** FAQ bot for common questions
- **CAN automate:** Status page ("Applications close in 5 days")

**Priority:** MEDIUM - high impact for reducing repeated questions

---

## Phase 2: Pass Allocation (2-3 Months Before)

### Job 2.1: Track Pass Applications

**Outcome:** Know who has applied for passes from each org

**When:** After applications open, ~2-3 months before event

**Current Process:**
- People apply through some system (Rainfocus? Staffing Force?)
- Track applications (spreadsheet? Rainfocus?)
- Need to know: who applied, which org, status

**Inputs Needed:**
- Application data from Rainfocus or wherever it lives
- Org mapping (who reports to whom)

**Pain Points:**
- **UNKNOWN:** Need to understand current process better
- Likely manual tracking or hard-to-use Rainfocus interface
- Need to update spreadsheets from Rainfocus data

**Time Required:** Unknown, estimate 2-4 hours/week during application period

**Automation Opportunity:** 🟡 MEDIUM
- **CAN automate:** Import application data from Rainfocus export
- **CAN automate:** Dashboard showing applications by org
- **CAN automate:** Alert when someone applies
- **CANNOT automate:** If data locked in Rainfocus with no export

**Priority:** MEDIUM - depends on discovery of current process

---

### Job 2.2: Track Leader Approvals

**Outcome:** Know which applications have been approved by managers

**When:** After applications, during approval period

**Current Process:**
- Managers approve their reports (in Rainfocus? Email?)
- Track approval status
- Follow up on pending approvals
- Chase down slow responders

**Inputs Needed:**
- Application data with approval status
- Manager contact info
- Deadline for approvals

**Pain Points:**
- **UNKNOWN:** Need to understand current approval workflow
- Probably manual tracking of who's approved vs. pending
- Chasing people for approvals is tedious

**Time Required:** Unknown, estimate 3-5 hours/week during approval period

**Automation Opportunity:** 🟢 HIGH (Quick Win)
- **CAN automate:** Dashboard showing approval status by org
- **CAN automate:** Automated reminder to managers with pending approvals
- **CAN automate:** Escalation for overdue approvals
- **CAN automate:** Summary of approved vs. available passes

**Priority:** MEDIUM - high automation potential

---

### Job 2.3: Assign Passes to Approved Applicants

**Outcome:** Each approved person gets a pass (up to org allocation limit)

**When:** After approvals, ~2 months before event

**Current Process:**
- James and Ria make pass assignments for their orgs
- Track who has been assigned a pass
- Coordinate if someone approved but no passes left
- Handle edge cases and exceptions

**Inputs Needed:**
- Approved applications
- Pass allocations by org
- Assignment decisions from James and Ria

**Pain Points:**
- **UNKNOWN:** What tool is used for assignments?
- Coordination between James and Ria
- Over-allocation risk (more approvals than passes)
- Under-allocation waste (passes unused)

**Time Required:** Unknown, estimate 4-8 hours for coordination

**Automation Opportunity:** 🟡 MEDIUM
- **CAN automate:** Dashboard showing approved vs. allocated vs. assigned
- **CAN automate:** Flag over/under-allocation early
- **CAN automate:** Suggested assignments based on staffing needs
- **CANNOT automate:** Final decision (James/Ria make the call)

**Priority:** HIGH - critical to get right

---

## Phase 3: Shift Scheduling (1-2 Months Before)

### Job 3.1: Set Up Shift Schedule in System

**Outcome:** Shifts are defined and available for signups

**When:** ~1-2 months before event, after passes assigned

**Current Process:**
- Create shifts in Staffing Force / Rainfocus
- Define: date, time, location, role, number of people needed
- Probably manual data entry for each shift

**Inputs Needed:**
- Staffing requirements (from Job 1.2)
- Event schedule (hours, booth locations)
- Shift duration (2 hours? 4 hours?)

**Pain Points:**
- Manual data entry of many shifts
- Easy to make mistakes (typos, wrong times)
- Hard to edit if event schedule changes

**Time Required:** 3-6 hours for initial setup

**Automation Opportunity:** 🟢 HIGH
- **CAN automate:** Generate shifts from staffing requirements
- **CAN automate:** Bulk import to Rainfocus (if API exists)
- **CAN automate:** Validation (no overlaps, all times covered)
- **CANNOT automate:** If Rainfocus doesn't allow bulk import

**Priority:** MEDIUM - one-time task but error-prone

---

### Job 3.2: Communicate Shift Signup Instructions

**Outcome:** Pass holders know how and when to sign up for shifts

**When:** When shift signups open

**Current Process:**
- Email everyone with passes
- Explain how to use Staffing Force
- Set deadlines
- Answer questions about how to sign up

**Inputs Needed:**
- List of pass holders
- Staffing Force instructions
- Signup deadline

**Pain Points:**
- People don't read instructions
- Lots of individual questions
- Confusion about how system works

**Time Required:** 2-4 hours + Q&A

**Automation Opportunity:** 🟢 HIGH (Quick Win)
- **CAN automate:** Automated email with instructions
- **CAN automate:** FAQ page or chatbot
- **CAN automate:** Video walkthrough of Staffing Force
- **CAN automate:** Reminder emails as deadline approaches

**Priority:** LOW - not time-consuming but nice to automate

---

### Job 3.3: Monitor Shift Signup Progress

**Outcome:** Know which shifts are under-staffed and need more volunteers

**When:** During signup period, ongoing monitoring

**Current Process:**
- Log into Rainfocus/Staffing Force
- Check each shift manually
- Identify gaps (shifts with too few signups)
- Track in spreadsheet
- Reach out to recruit more volunteers

**Inputs Needed:**
- Shift data with signup counts
- Staffing requirements (target per shift)

**Pain Points:**
- Manual checking of each shift
- Hard to get overview across all shifts
- Reactive (only notice gaps when you check)
- Time-consuming to monitor frequently

**Time Required:** 1-2 hours per day during signup period

**Automation Opportunity:** 🟢 HIGH (Quick Win)
- **CAN automate:** Dashboard showing signup status per shift
- **CAN automate:** Highlight under-staffed shifts in red
- **CAN automate:** Daily summary email of status
- **CAN automate:** Alert when shift falls below threshold

**Priority:** HIGH - very time-consuming currently

---

### Job 3.4: Recruit Volunteers for Under-Staffed Shifts

**Outcome:** All shifts reach minimum staffing requirement

**When:** During and after signup period

**Current Process:**
- Identify people with passes who haven't signed up
- Reach out individually via Slack/email
- Ask if they can cover specific shifts
- Follow up on non-responses
- Coordinate and track commitments

**Inputs Needed:**
- Under-staffed shift list
- Pass holder list
- Who has already signed up (so don't ask twice)

**Pain Points:**
- Manual outreach one-by-one
- Tracking who you've asked and what they said
- Follow-ups on non-responses
- Coordination is tedious and time-consuming

**Time Required:** 5-10 hours for recruiting

**Automation Opportunity:** 🟡 MEDIUM
- **CAN automate:** List of people to contact for each shift
- **CAN automate:** Email template generation
- **CAN automate:** Track outreach status (asked, responded, committed)
- **CANNOT automate:** Actual ask (personal touch matters)

**Priority:** MEDIUM - time-consuming but needs human touch

---

### Job 3.5: Coordinate Session Staffing (Parallel Track)

**Outcome:** All sessions have presenters, demo specialists, support

**When:** Parallel to booth shift scheduling

**Current Process:**
- Session owners manage their own session staffing
- Not centrally coordinated by staffing lead
- Demo specialists shared across sessions and booth
- Need to avoid conflicts (demo specialist in two places at once)

**Inputs Needed:**
- Session schedule
- Demo specialist assignments
- Session owner contacts

**Pain Points:**
- Limited visibility into session staffing
- Demo specialists double-booked
- Hard to coordinate across session owners
- Not clear if this is in scope for staffing lead

**Time Required:** Unknown, possibly not staffing lead's job

**Automation Opportunity:** 🔴 LOW
- This may be out of scope (session owners manage it)
- **MAYBE:** Dashboard showing demo specialist availability
- **MAYBE:** Conflict detection across sessions and booth

**Priority:** LOW / OUT OF SCOPE - need to clarify

---

## Phase 4: Pre-Event Finalization (1-2 Weeks Before)

### Job 4.1: Confirm Final Assignments

**Outcome:** Everyone knows their shifts and shows up prepared

**When:** 1-2 weeks before event

**Current Process:**
- Send confirmation emails to all staff
- Include: shift times, locations, what to bring, who to contact
- Answer last-minute questions
- Update calendar invites

**Inputs Needed:**
- Final shift assignments from Rainfocus
- Event logistics (booth locations, check-in info)

**Pain Points:**
- Manual email composition
- Information changes and needs resending
- People lose emails and ask again

**Time Required:** 3-5 hours

**Automation Opportunity:** 🟢 HIGH (Quick Win)
- **CAN automate:** Email generation from shift data
- **CAN automate:** Calendar invite creation
- **CAN automate:** Personalized itinerary for each person
- **CAN automate:** FAQ link in every email

**Priority:** MEDIUM - one-time but useful

---

### Job 4.2: Handle Last-Minute Cancellations (Week Before)

**Outcome:** Shifts remain fully staffed despite cancellations

**When:** 1-2 weeks before event, accelerating as event approaches

**Current Process:**
- Person DMs or messages in channel: "I can't make my shift"
- Staffing lead tries to find replacement
- Asks in channel or DMs individuals
- Updates Rainfocus manually when replacement found
- Person can't update Rainfocus themselves

**Inputs Needed:**
- Cancellation notification
- Shift details
- Available replacements

**Pain Points:**
- Manual coordination, staffing lead is bottleneck
- Frantic searching for replacements
- Updates to Rainfocus are manual and slow
- People can't self-service

**Time Required:** 2-5 hours in final week

**Automation Opportunity:** 🟠 HIGH (Complex)
- **CAN automate:** Self-service cancellation form
- **CAN automate:** Broadcast to available replacements
- **CAN automate:** Allow people to claim open shifts
- **CAN automate:** Update tracking (if not Rainfocus)
- **CANNOT automate:** Updating Rainfocus if no API

**Priority:** HIGH - causes "horror show" currently

---

### Job 4.3: Handle Last-Minute Shift Swaps

**Outcome:** Two people successfully swap shifts

**When:** 1-2 weeks before event

**Current Process:**
- Person A says "can someone swap with me?"
- Staffing lead helps find Person B
- Confirm both are qualified for each other's shifts
- Update Rainfocus with swap
- Manual coordination and updates

**Inputs Needed:**
- Swap request from Person A
- Shift details for both shifts
- Qualifications/roles

**Pain Points:**
- Same as cancellations: manual, slow, bottleneck
- People can't coordinate swaps themselves
- Rainfocus updates are manual

**Time Required:** 1-3 hours in final week

**Automation Opportunity:** 🟠 HIGH (Complex)
- **CAN automate:** Shift swap request system
- **CAN automate:** Match people willing to swap
- **CAN automate:** Validation (both qualified)
- **CAN automate:** Update tracking
- **CANNOT automate:** Rainfocus update if no API

**Priority:** HIGH - high-impact time saver

---

## Phase 5: Day-Of Event (During Dreamforce)

### Job 5.1: Monitor Real-Time Coverage

**Outcome:** Know if shifts are staffed or have gaps

**When:** During event (September 15-17)

**Current Process:**
- Check in with Dustin on the floor
- Respond to messages about no-shows
- Visible presence at booth to monitor

**Inputs Needed:**
- Expected schedule
- Actual attendance
- Communication from floor lead

**Pain Points:**
- Hard to know status remotely
- Reactive (only know there's a problem when someone reports it)

**Time Required:** Ongoing during event

**Automation Opportunity:** 🟡 MEDIUM
- **CAN automate:** Real-time dashboard of who's checked in
- **COULD automate:** Check-in system (QR code or app)
- Limited ROI - event is only 3 days and staffing lead likely on-site

**Priority:** LOW - not worth building for 3-day event

---

### Job 5.2: Handle Day-Of Emergencies

**Outcome:** Fill gaps when people don't show up

**When:** During event

**Current Process:**
- Get alert about no-show
- Find anyone available to fill in
- Text/Slack/in-person recruitment
- Update tracking

**Inputs Needed:**
- No-show notification
- List of people on-site and available
- Shift requirements

**Pain Points:**
- High-stress, time-sensitive
- Limited pool of available people
- On-site coordination challenges

**Time Required:** Variable, hopefully rare

**Automation Opportunity:** 🔴 LOW
- Hard to automate emergency response
- **MAYBE:** List of on-site people available for emergency coverage
- Human judgment and relationships matter most

**Priority:** LOW - can't really automate this

---

### Job 5.3: Support Dustin and Floor Team

**Outcome:** Floor operations run smoothly

**When:** During event

**Current Process:**
- Be available for questions and issues
- Coordinate with Dustin
- Problem-solve in real-time

**Inputs Needed:**
- Communication channels
- Situational awareness

**Pain Points:**
- Need to be responsive and available

**Time Required:** Full-time during event

**Automation Opportunity:** 🔴 NONE
- This is core human coordination work

**Priority:** N/A - not automatable

---

## Phase 6: Post-Event (After Dreamforce)

### Job 6.1: Capture Lessons Learned

**Outcome:** Document what worked and what didn't for next year

**When:** 1-2 weeks after event

**Current Process:**
- Debrief with key stakeholders
- Write up learnings
- Store for next year

**Inputs Needed:**
- Feedback from Dustin, session owners, staff
- Data on what happened (cancellations, no-shows, etc.)
- Personal observations

**Pain Points:**
- Easy to skip when busy
- Learnings get lost
- Not structured or actionable

**Time Required:** 2-4 hours

**Automation Opportunity:** 🟡 MEDIUM
- **CAN automate:** Survey to gather feedback
- **CAN automate:** Data summary (how many changes, gaps, etc.)
- **CAN automate:** Template for lessons learned doc
- **CANNOT automate:** Analysis and synthesis

**Priority:** MEDIUM - important for future but not urgent

---

### Job 6.2: Thank Volunteers and Stakeholders

**Outcome:** People feel appreciated and will help again next year

**When:** Shortly after event

**Current Process:**
- Send thank you emails
- Public recognition in Slack channels
- Personal notes to key contributors

**Inputs Needed:**
- List of everyone who helped
- What they did

**Pain Points:**
- Time-consuming to personalize
- Easy to accidentally skip someone

**Time Required:** 2-3 hours

**Automation Opportunity:** 🟢 MEDIUM (Quick Win)
- **CAN automate:** Thank you email generation from shift data
- **CAN automate:** Public recognition post with names
- **SHOULD have:** Human personalization for key people

**Priority:** LOW - nice to have but not critical

---

### Job 6.3: Update Process Documentation

**Outcome:** Next year's staffing lead has good docs

**When:** 1 month after event

**Current Process:**
- Update any docs that exist
- Write up new processes
- Often skipped due to time

**Inputs Needed:**
- Lessons learned
- Process changes made this year

**Pain Points:**
- Hard to remember details after time passes
- Documentation debt accumulates

**Time Required:** 4-8 hours

**Automation Opportunity:** 🔴 LOW
- This project is doing this job!
- **CAN automate:** Template and structure
- **CANNOT automate:** Writing itself

**Priority:** HIGH - this project addresses this need

---

## Summary: Automation Opportunities

### 🟢 Quick Wins (Easy + High Impact)

1. **Staffing Requirements Calculator** - Apply formulas to event footprint automatically
2. **Pass Allocation Model** - Calculate recommended allocations and run scenarios
3. **Timeline Dashboard** - Public reference for key dates and process
4. **Approval Tracking & Reminders** - Auto-remind managers with pending approvals
5. **Shift Signup Monitor** - Dashboard showing under-staffed shifts with alerts
6. **Confirmation Email Generation** - Auto-generate personalized shift confirmations
7. **FAQ Bot / Page** - Reduce repeated questions

**Estimated Time Savings:** 20-30 hours

### 🟠 High-Impact (Complex but Worth It)

1. **Self-Service Cancellation & Swap** - Let people handle their own changes
2. **Event Footprint Change Notification** - Alert when footprint updates
3. **Rainfocus Import Automation** - Auto-import data instead of manual export
4. **Volunteer Recruitment Tracker** - Track outreach for under-staffed shifts
5. **Pass Tracking Dashboard** - End-to-end view of apply → approve → assign → schedule

**Estimated Time Savings:** 30-40 hours

### 🔴 Human-Required (Keep Manual)

1. Final pass allocation decisions (political judgment)
2. Negotiation with org leaders
3. Day-of emergency response
4. Personal relationship building
5. Strategic decisions about event approach
6. Session owner coordination (may be out of scope)

**Cannot automate:** Judgment, politics, relationships, emergencies

---

## Prioritized Implementation Roadmap

### Phase 1: Must-Have (Build First)
1. Staffing Requirements Calculator
2. Pass Allocation Model
3. Shift Signup Monitor Dashboard
4. Rainfocus Import Automation

**Why:** These save the most time and are needed early in timeline

### Phase 2: Should-Have (Build If Time)
1. Self-Service Cancellation/Swap System
2. Timeline Dashboard
3. Approval Tracking & Reminders
4. Confirmation Email Generation

**Why:** High impact but can work around them if needed

### Phase 3: Nice-to-Have (Build If Extra Time)
1. FAQ Page/Bot
2. Event Footprint Change Notifications
3. Volunteer Recruitment Tracker
4. Thank You Email Generation
5. Lessons Learned Templates

**Why:** Helpful but not critical, lower time savings

---

## Success Metrics

### Quantitative
- **Manual hours saved:** Target 50%+ reduction (est. 40-60 hours saved)
- **Time to current state:** <1 minute (vs. ~15 minutes currently)
- **Self-service rate:** 70%+ of shift changes without staffing lead
- **Accuracy:** Zero over-allocation, zero coverage gaps

### Qualitative
- Summer feels confident and in control
- Stakeholders find process clear and predictable
- Staff can self-service common requests
- Process documented for next year

---

**Next Steps:**
1. Validate this analysis with Summer and you
2. Prioritize jobs based on actual time spent (fill in unknowns)
3. Confirm automation feasibility after discovery phase
4. Build top priority automations first

**Last Updated:** May 21, 2026  
**Status:** DRAFT pending validation
