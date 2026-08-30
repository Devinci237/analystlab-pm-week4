# AI-Powered Customer Intelligence Transformation Project

**AnalystLab Africa — Project Management Internship, Weeks 1–4**
**Author:** Devinci Ebaha Djoki ([LinkedIn](https://linkedin.com/in/ebaha-devinci))

## Overview

This repository contains the Week 1 through Week 4 deliverables of the AnalystLab Africa Project Management Internship Programme.

Weeks 1–3 apply project initiation, planning, and detailed scheduling to a real Cameroonian retail company, **DOVV Distribution SA**, rather than a purely fictional case. As set out in the Week 4 brief, that work is retained as-is and not redone.

Starting Week 4, the programme moves to a new, shared case study: the **HealthConnect Clinic Experience Lab**, worked in parallel by five internship tracks (Project Management, Data Analytics, Data Science, ML Engineering, Generative AI). This section of the repository covers the Project Management track's contribution, starting with Problem Understanding.

All figures tied to fictional entities (DOVV's internal metrics in Weeks 1–3, HealthConnect's operational data in Week 4+) are working assumptions built for the purpose of each exercise, in the absence of real internal data — a standard practice at the scoping stage in consulting.

## Week 4: HealthConnect Project Kickoff & Problem Understanding

Week 4 marks the transition to the HealthConnect Clinic Experience Lab. The Project Management track's role is to coordinate the four technical tracks (Data Analytics, Data Science, ML Engineering, Generative AI) across five project phases, starting with the governance foundation below: a full Project Initiation Package plus a standalone weekly summary.

**Central project question:** How can HealthConnect Clinic use data and AI to reduce missed appointments and improve the patient support experience?

| Document | Description |
|---|---|
| [Project Charter](deliverables/week4/Project_Charter_HealthConnect.docx) | Project mandate: business case, objectives per track, PM authority and scope, assumptions, constraints, high-level milestones and success criteria |
| [Scope Statement](deliverables/week4/Scope_Statement_HealthConnect.docx) | In-scope and out-of-scope boundaries, project deliverables by phase, acceptance criteria, and exclusions |
| [Stakeholder Register](deliverables/week4/Stakeholder_Register_HealthConnect.docx) | All six project stakeholders mapped by role, phase involvement, influence/interest (power-interest matrix), attitude, and engagement strategy |
| [Work Breakdown Structure](deliverables/week4/WBS_HealthConnect.docx) | PM-governance scope only, decomposed to work-package level for the confirmed Week 4 phase, with Weeks 5–8 kept at phase level as a planning assumption |
| [High-Level Timeline](deliverables/week4/High_Level_Timeline_HealthConnect.xlsx) | Two-part Gantt: a day-by-day Week 4 schedule (confirmed) and a phase-level Weeks 4–8 overview (assumed beyond Week 4), built directly from the WBS |
| [Initial Risk and Dependency Register](deliverables/week4/Risk_Dependency_Register_HealthConnect.docx) | Six risks scored by Probability × Impact with PMBOK response strategies, and four cross-track dependencies, explicitly cross-referenced to each other |
| [Communication Approach](deliverables/week4/Communication_Approach_HealthConnect.docx) | Slack-based communication cadence, reporting format, and a three-level escalation procedure calibrated against the Risk Register |
| [Week 4 Project Summary](deliverables/week4/Week4_Project_Summary_HealthConnect.docx) | Standalone summary: problem addressed, resources used, key observations, proposed approach, key considerations, and focus for Week 5 |

### Notable design decisions — Week 4

- **Assumptions are flagged, not smoothed over.** The assignment brief confirms only the five project phases and the Week 4 deadline; it does not confirm that each phase maps to exactly one week. Rather than presenting a full Weeks 4–8 calendar as fact, every document that touches scheduling (Charter, Scope Statement, WBS, Timeline, Risk Register) explicitly labels this "one phase per week" mapping as a planning assumption, tied to risk R4 in the Risk Register.
- **The WBS stays in its lane.** The Work Breakdown Structure decomposes the Project Management track's governance work only (coordination, documentation, communication), not the technical work of the other four tracks, which each define and own their own deliverables. This boundary is stated explicitly in the WBS's Purpose and Scope section.
- **Coordination is scheduled early, not reactively.** The cross-track coordination touchpoint (WBS item 1.1.10) is placed on Day 2 of Week 4, immediately after the Charter is drafted, so that misalignment surfaces before the rest of the Initiation Package is finalized. This sequencing directly implements the "early alert" mitigation defined for risk R1 (upstream delays) in the Risk and Dependency Register.
- **Risks and dependencies are cross-referenced, not siloed.** Each risk in the register that stems from a cross-track dependency (R1, R3, R4) is explicitly linked to the corresponding dependency entry (D1/D2, D3, D4), so the two tables read as one coherent risk model rather than two disconnected lists.

## Week 1–3: DOVV Distribution SA — AI-Powered Customer Intelligence Transformation

*(Retained from the previous submission, unchanged — see "Notable design decisions" below for context.)*

### Business Scenario

DOVV Distribution SA, a Cameroonian retail chain established in Yaounde, does not yet have a structured system to identify customers at checkout, track purchase history over time, or personalise offers. This project designs and schedules a solution combining a loyalty identification system with an AI-driven churn prediction and personalisation engine, aimed at increasing the proportion of regular customers within the existing customer base from 15 percent to 25 percent over 16 months.

### Week 3: Project Scheduling, Resource Planning & Execution Planning

Week 3 formalises the project's schedule into a full network model: every one of the 42 activities carries a calculated Earliest Start, Earliest Finish, Latest Start, Latest Finish, and Total Float, and the Critical Path is identified and explained rather than assumed.

| Document | Description |
|---|---|
| [Part 1 — Review of Week 2 Documents](deliverables/week3/Part1_Review_Week2_Documents.docx) | Documents two dependency corrections and the WBS granularity update surfaced while preparing this week's Critical Path Analysis |
| [Project Schedule](deliverables/week3/Dovv_Project_Schedule.docx) | 42 activities with Activity ID, Name, Duration, Start/Finish Date, Dependencies, and Assigned Resource |
| [Gantt Chart](deliverables/week3/Dovv_Gantt_Chart.xlsx) | Weekly-calendar Gantt chart with phase colour coding; every bar's start and end date verified programmatically against the schedule, not just visually |
| [Network Diagram](deliverables/week3/Dovv_Network_Diagram.pdf) | Activity-on-Node diagram showing ES, EF, LS, LF and Total Float for all 42 activities, critical path highlighted in red |
| [Critical Path Analysis](deliverables/week3/Dovv_Critical_Path_Analysis.docx) | Explains why the adoption campaign chain, not the technical or data science work, controls the project's completion date |
| [Resource Allocation Plan](deliverables/week3/Dovv_Resource_Allocation_Plan_Week3.docx) | Human, technical, and budget resources, extended this week with two roles (Business Analyst, QA Tester) found to be genuine gaps in the Week 2 plan |
| [Project Execution Plan](deliverables/week3/Dovv_Project_Execution_Plan_Week3.docx) | Governance, communication, task assignment, and escalation, calibrated against verified critical-path ownership by role, not assumed at the team level |
| [Schedule Risk Assessment](deliverables/week3/Dovv_Schedule_Risk_Assessment.docx) | Six scheduling-specific risks, each grounded in the Critical Path Analysis rather than generic project risk language |

#### Notable design decisions — Week 3

- **The critical path was verified twice, not assumed once.** Every Total Float value was calculated independently through a Python reference implementation and cross-checked line by line against the Excel formulas before either was trusted, after an earlier Gantt chart iteration was found, on inspection, to render bars incorrectly despite appearing correct on screen.
- **Critical-path ownership was checked role by role, not phase by phase.** An early draft of the Execution Plan claimed only two roles carried critical-path responsibility; re-verifying against the actual Assigned Resource data showed six different roles each own at least one critical-path task at different points in the 16-month timeline. The Execution Plan and Schedule Risk Assessment were corrected accordingly.
- **Waiting periods are treated as real schedule elements, not gaps.** The three data-accumulation and three adoption-ramp-up periods are modelled as explicit tasks with duration, not implicit blank space, since they collectively account for the largest single block of critical-path time in the project (160 calendar days for the adoption ramp-up alone).

### Week 1–2: Initiation and Execution Planning

| Document | Description |
|---|---|
| [Project Charter](deliverables/week1/Dovv_Project_Charter.pdf) | Project mandate: background, SMART objective, scope, deliverables, sponsor, constraints, timeline, success criteria |
| [Stakeholder Register](deliverables/week1/Dovv_Stakeholder_Register.pdf) | Stakeholder mapping by influence and interest, with engagement strategies |
| [Work Breakdown Structure](deliverables/week1/Dovv_WBS.pdf) | Project decomposition into phases and tasks, updated in Week 3 to match the full 42-task granularity used in the Schedule |
| [Risk Register](deliverables/week1/Dovv_Risk_Register.pdf) | Eight identified risks across technical, organisational, legal and strategic categories, with mitigation plans |
| [Communication Plan](deliverables/week1/Dovv_Communication_Plan.pdf) | Two-layer communication structure: routine cadence tied to the WBS, and exception alerts tied to high-impact risks |
| [Project Budget](deliverables/week2/Dovv_Project_Budget.pdf) | Seven budget categories with a 15 percent contingency reserve, sized against the Risk Register's risk profile |
| [Project Execution Strategy](deliverables/week2/Dovv_Project_Execution_Strategy.pdf) | Week 2 execution approach, monitoring, risk management, communication, and change control |
| [PM Deliverables Methodology Guide](deliverables/week1/Guide_Methodologique_Livrables_PM.pdf) | General reference guide on the structure and content of each core PM deliverable, independent of this specific case |

#### Notable design decisions — Weeks 1–2

- **Retention, not acquisition.** The SMART objective explicitly targets DOVV's existing customer base, with customer acquisition marketing intentionally placed out of scope.
- **Parallel, not sequential, execution.** The WBS reflects that technical development and data collection run concurrently, and that the customer adoption campaign cannot start before the loyalty card itself is available.
- **A strategic risk, not just an operational one.** The Risk Register includes the possibility that the chosen solution itself may not be the most efficient approach, with a mitigation pointing to existing local alternatives (such as Koree or Gwassou) as a partnership option worth evaluating before building in house.

## Methodology

This work follows a PMBOK-aligned approach throughout. Weeks 1–3 apply it to a pilot-scale retail transformation project, including formal network scheduling (forward pass / backward pass, Activity-on-Node) for the Critical Path Analysis. Week 4 onward applies the same standard (charter, scope, stakeholder analysis, WBS, scheduling, risk management, communication planning) to a multi-track, cross-functional case study, with explicit flagging of any assumption not yet confirmed by the programme. AI tools were used to assist with research, drafting, and calculation verification, in line with the internship's guidelines; all reasoning, decisions, and final content were reviewed and validated by the author.

## Programme Context

Produced as part of the AnalystLab Africa Project Management Internship Programme (August–October 2026), alongside the Google and IBM Project Management and Data Analytics professional certificates (Coursera).

---

*This project is an academic exercise conducted within a structured internship programme. It does not represent an engagement commissioned by DOVV Distribution SA or by any real healthcare provider.*
