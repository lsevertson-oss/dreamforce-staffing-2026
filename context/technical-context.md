# Technical Context: Systems & Tools

## Current Systems Landscape

### 1. Rainfocus (Backend System)

**What it is:** Event management platform used by Salesforce for conference management

**What it does:**
- Manages conference registrations
- Tracks sessions and attendees
- Handles staffing assignments (backend)
- Source of truth (supposedly) for official data

**Who uses it:**
- Conference organizers
- Session managers (like Marika's team)
- Staffing leads (including Summer)
- Pass allocators (James, Ria)

**Known Limitations:**
- Very hard to use ("really hard to use" - direct quote)
- Poor UX, complex navigation
- Limited/unclear export capabilities
- May not have public API
- Difficult to get data out for analysis

**Integration Status:**
- No known API access currently
- Likely requires manual export (CSV/Excel)
- Updates may require manual data entry
- Real-time sync probably not possible

**Critical Unknown:**
- Can we export data programmatically?
- What data is available via export?
- How often can exports be generated?
- Who has access to export functionality?

### 2. Staffing Force (Employee Interface)

**What it is:** Employee-facing interface for volunteering for event staffing

**What it does:**
- Employees apply for passes
- Employees sign up for shifts
- Shows available shifts and roles
- Handles volunteer coordination

**Relationship to Rainfocus:**
- Appears to be a front-end layer on top of Rainfocus
- "Rainfocus behind the scenes" surfaced as Staffing Force
- Data flows between them (exact mechanism unclear)

**Who uses it:**
- Slack employees volunteering to staff
- Booth volunteers
- Session staffers

**Known Limitations:**
- Limited to volunteer roles (booth shifts mainly)
- Does NOT cover sessions (session owners manage separately)
- Does NOT cover executives or producers
- No self-service for shift swaps or cancellations

**Integration Status:**
- Tied to Rainfocus backend
- Probably no independent API
- Changes must go through Rainfocus

### 3. Spreadsheets (Current Workaround)

**What they are:** Google Sheets/Excel used as shadow systems

**Why they exist:**
- Rainfocus is too hard to use
- Need to do analysis and calculations
- Need to share data with stakeholders
- Need to track things Rainfocus doesn't handle well

**What they track:**
- Pass allocations by org
- Who has applied vs. approved vs. assigned
- Staffing requirements and calculations
- Session assignments (managed by session owners)
- Last-minute changes and notes

**Problems:**
- No single source of truth (multiple spreadsheets)
- Manual data entry from Rainfocus exports
- Version control and sync issues
- Error-prone (copy/paste mistakes)
- Hard to keep current

**Opportunity:**
- Could be basis for automation
- If we can't fix Rainfocus, we can make spreadsheets smarter

### 4. Google Calendar

**What it's used for:**
- Session scheduling
- Shift scheduling
- Personal reminders for staff
- Shared calendars for visibility

**Limitations:**
- Not integrated with Rainfocus or Staffing Force
- Manual data entry
- Hard to get aggregate view
- Doesn't handle conflicts automatically

**Integration Opportunities:**
- Could auto-generate from Rainfocus exports
- Could sync with dashboard
- Could send automated reminders

### 5. Slack (Communication)

**Current Usage:**
- Last-minute change requests ("I can't make my shift")
- Questions about assignments
- Coordination between staffing lead and staff
- Channel-based communication

**Problems:**
- Messages get lost
- No structured workflow
- Manual coordination required
- Staffing lead becomes bottleneck

**Automation Opportunities:**
- Bot for self-service requests
- Automated notifications
- Structured workflows (shift swap requests)
- Dashboard links in channels

### 6. Email

**Current Usage:**
- Pass application notifications
- Approval workflows (?)
- Announcements to staff
- Individual communications

**Problems:**
- Gets buried in inbox
- No tracking or workflow
- Hard to know current state

## Data Flow (Current State)

```
Strategic Events
    ↓ (event footprint)
Staffing Lead
    ↓ (staffing needs)
Pass Allocators (James, Ria)
    ↓ (allocations by org)
Employees
    ↓ (applications)
Leaders
    ↓ (approvals)
Pass Allocators
    ↓ (pass assignments)
Rainfocus ←→ Spreadsheets (manual sync)
    ↓
Staffing Force
    ↓ (shift signups)
Employees

[Parallel track:]
Session Owners
    ↓ (session staffing)
Google Calendar / Spreadsheets
    ↓
Rainfocus (maybe?)
```

**Key Observations:**
- Multiple manual handoffs
- Unclear where Rainfocus is updated vs. read from
- Parallel tracks (booth vs. session staffing)
- Spreadsheets used to bridge gaps

## Technical Constraints

### Data Access
- **Rainfocus API:** Unknown, possibly doesn't exist
- **Rainfocus Export:** Probably available but manual
- **Staffing Force API:** Unlikely to have direct access
- **Spreadsheets:** Full access (we own them)
- **Google Calendar:** Full API access

### Integration Complexity
- **High:** Direct integration with Rainfocus/Staffing Force
- **Medium:** Automated import/export workflows
- **Low:** Tools that work with spreadsheet exports

### Technical Skills
- **Available:** AI-assisted scripting (Python, JavaScript)
- **Available:** Spreadsheet automation (Google Sheets API)
- **Available:** Simple web dashboards
- **Not Available:** Backend access to vendor systems
- **Not Available:** Dedicated dev team

### Hosting & Deployment
- **Available:** Google Workspace (Sheets, Docs)
- **Available:** Cloud functions (Google Cloud, AWS Lambda)
- **Available:** Static site hosting
- **Unknown:** Internal Slack hosting options

### Security & Privacy
- **Concern:** Employee data (names, roles, etc.)
- **Concern:** Pass allocation decisions (org politics)
- **Concern:** Access control for tools
- **Requirement:** SSO/authentication for any tools built
- **Requirement:** Audit trail for changes

## Potential Technical Solutions

### Option 1: Enhanced Spreadsheet System
**Approach:** Make spreadsheets smarter with automation
- Google Sheets with Apps Script
- Automated import from Rainfocus exports
- Calculated fields for staffing needs
- Dashboard views
- Integration with Slack for notifications

**Pros:**
- No dependency on Rainfocus API
- Familiar tools (Google Sheets)
- Fast to build
- Easy to maintain

**Cons:**
- Still requires manual export from Rainfocus
- Not true real-time
- Could get complex with too many formulas

### Option 2: Custom Dashboard + Backend
**Approach:** Build web app with database backend
- Import data from Rainfocus exports
- Custom database (PostgreSQL, Firebase)
- React/Next.js dashboard
- API for integrations

**Pros:**
- Full control over features
- Better UX than spreadsheets
- Can add complex workflows
- Real database

**Cons:**
- Higher complexity
- Hosting and maintenance required
- Still depends on Rainfocus exports
- More time to build

### Option 3: Hybrid Approach (Recommended)
**Approach:** Smart spreadsheets + targeted automation
- Google Sheets as data layer
- Apps Script for automation
- Simple web dashboard for Summer (iframe Sheets)
- Slack bot for self-service
- Python scripts for complex calculations

**Pros:**
- Low complexity, fast to build
- Familiar tools where appropriate
- Automation where it adds value
- Can evolve over time

**Cons:**
- Multiple pieces to coordinate
- Not as polished as single app
- Some manual steps remain

## Integration Points

### Priority 1: Rainfocus Export → Spreadsheet
- Automate import of Rainfocus data
- Parse and normalize data
- Update calculated fields

### Priority 2: Spreadsheet → Dashboard
- Display current state
- Show what needs attention
- Timeline of upcoming tasks

### Priority 3: Slack → Self-Service Workflow
- Bot for shift swap requests
- Automated approvals (where possible)
- Notifications to relevant people

### Priority 4: Calendar Sync
- Generate calendars from schedule data
- Send reminders
- Detect conflicts

## Technical Risks

| Risk | Impact | Mitigation |
|------|--------|------------|
| Can't export from Rainfocus | High | Manual CSV export as backup |
| Rainfocus data format changes | Medium | Flexible parsing, validation |
| Google Sheets hits limits (rows, API calls) | Medium | Monitor usage, optimize |
| Authentication/access control | High | Use Google Workspace SSO |
| Tools break during event | High | Manual backup processes documented |

## Technical Requirements

### Must Have
- Import data from Rainfocus (manually if needed)
- Calculate staffing requirements
- Show current state clearly
- Track pass allocation vs. needs
- Work on Summer's devices (laptop, phone)

### Should Have
- Automated import (not manual copy/paste)
- Slack integration for notifications
- Self-service shift swaps
- Historical tracking

### Nice to Have
- Real-time sync with Rainfocus
- Predictive analytics
- Mobile-optimized dashboard
- Automated matching (shift swaps)

## Technology Stack Recommendations

**Data Layer:** Google Sheets (familiar, accessible, no hosting)  
**Automation:** Google Apps Script + Python scripts  
**Dashboard:** Google Sheets dashboard or simple HTML/JS  
**Communication:** Slack API  
**Hosting:** Google Cloud Functions or Apps Script web app  
**Authentication:** Google Workspace SSO

**Rationale:** Maximize use of Google Workspace tools Summer already has access to, minimize hosting/maintenance burden, enable rapid iteration.

---

**Last Updated:** May 21, 2026  
**Next Review:** After Rainfocus export test
