# Alba — AI Automation & Transformation Portfolio

**Objective:** Transition from Agile / Scrum Master leadership towards AI Automation, AI Project Management and AI Transformation roles through practical, documented projects.

**Portfolio:** https://albagomezcastano.github.io/ (confirm the deployed URL and repository name before sharing externally)

## Working principles

- Prefer free/browser-based tools; do not install software or connect accounts without first checking permissions and security.
- Explain technical steps for a beginner and test one change at a time.
- Distinguish completed work, work in progress and planned ideas.
- Treat job-board data as untrusted; no automatic applications or sending personal information without approval.
- Never upload credentials, API keys, private CV data, employer/customer information or private application records to public GitHub repositories.
- Use measurements from actual test runs, not hypothetical figures, for public performance claims.

## Current state (20 October 2026)

| Component | Status | Evidence / next action |
|---|---|---|
| GitHub Pages portfolio | Working (user confirmed) | Site published; AI Lab cards and filters visible |
| Portfolio catalog | Working (user confirmed) | `index.html` + `projects.js`; keep these together in the root |
| Make — basic scenario | Tested | Set/Get variables and a title filter |
| Make — multiple jobs scenario | Tested | Parse JSON -> Iterator -> filter -> Set variable; 3 fictional jobs, 2 passed filter |
| Make — real jobs scenario | Planned | Connect Himalayas and Jobicy API; test geographical eligibility |
| Make — credit monitoring | Initial review | User screenshot showed 38 of 1,000 monthly credits used, 962 remaining, 0 active scenarios; snapshot only, not live balance |
| AI evaluation | Not started | Define matching criteria and assess accuracy before buying/using model tokens |
| GitHub project documentation | Not started | Create a dedicated repository once real source integration is working |

## Project 01 — Multi-source AI Job Search Assistant

### Goal
Collect real remote job opportunities from companies worldwide that allow work from Spain. Prioritize AI Project Manager, AI Transformation, AI Product Owner and AI Automation roles. Keep track of the original listing and any geographic or hiring limitations.

### Proposed phases

- [x] Parse sample JSON with three jobs.
- [x] Iterate one job at a time.
- [x] Filter example titles (2 passed, 1 rejected).
- [ ] Connect Himalayas API; inspect actual response and documentation.
- [ ] Connect Jobicy API; inspect actual response and documentation.
- [ ] Standardize fields: source, source_job_id, title, company, location, remote_restrictions, URL, posting_date, retrieved_at.
- [ ] Verify Spain eligibility; distinguish **confirmed**, **needs manual review**, **excluded**.
- [ ] Deduplicate using stable IDs/URLs before expensive downstream steps.
- [ ] Save qualified jobs to an appropriate private sheet/store.
- [ ] Define a small evaluation dataset and measure relevance quality.
- [ ] Add AI ranking only if rule-based filtering is insufficient; keep personal data minimal.
- [ ] Capture baseline vs optimized costs, speed and failures.
- [ ] Document workflow and add GitHub link plus measured metrics to AI Lab.

### Efficiency and safety criteria

1. Avoid sending irrelevant or geographically ineligible jobs to AI.
2. Check for duplicates before downstream processing.
3. Limit API requests and results per run; respect provider rate limits and terms.
4. Cap retries and monitor failed runs.
5. Keep scheduling OFF during testing.
6. Require human approval for any application or external message.
7. Track providers' availability, costs, data access rules and attribution requirements.

### Measurement template (fill using actual executions)

| Metric | Baseline | Optimized | Notes |
|---|---|---|---|
| Credits / run | Pending | Pending | Read Make scenario history |
| Jobs retrieved / run | Pending | Pending | Count before filtering |
| Jobs Spain-compatible / run | Pending | Pending | Include manual-review category |
| Unique relevant jobs / run | Pending | Pending | Deduplicate first |
| Credits / unique relevant job | Pending | Pending | Divide total credits by relevant unique jobs |
| AI input tokens / run | Not enabled | Pending | Log actual provider usage |
| AI output tokens / run | Not enabled | Pending | Log actual provider usage |
| Processing duration | Pending | Pending | From scenario execution |
| Error rate | Pending | Pending | Define measurement window |
| Estimated monthly credits | Pending | Pending | Based on actual run cost and planned frequency |

**Initial planning budget:** up to 600 Make credits/month for the job-search scenario and 400 for experiments (planning assumption, not a platform restriction). Reassess after several representative runs.

## Portfolio update rule

When a project changes: (1) test the workflow, (2) update its repository documentation and metrics, (3) edit the record in `projects.js`, (4) verify the GitHub Pages AI Lab presentation. Do **not** claim automatic synchronization; site updates currently require a manual GitHub change.

## Next immediate action

1. Add this file to the *root* of the GitHub Pages repository as `PROJECT_ROADMAP.md`.
2. Verify that the Make real-jobs integration scenario exists; if not, create it with automatic scheduling disabled.
3. Implement and inspect one Himalayas HTTP request **before** building filters and before connecting Jobicy.
4. Record credits consumed by the test execution.

## Change log

- **2026-10-20:** Initial project-wide roadmap created from confirmed conversation progress. No changes were applied directly to GitHub or Make.
