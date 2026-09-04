# AIDAN Business User Guide

**Audience:** Operations leaders, department managers, team members, and approvers  
**Purpose:** Explain how a non-technical business team should use AIDAN safely and consistently  
**Product stage:** This guide describes the intended experience shown in the current low-fidelity wireframe. Features and numbers are illustrative until the product is built and connected to real company systems.

---

## 1. What AIDAN Does

AIDAN is a control center for company-approved AI workers.

An AI worker—called an **agent** in AIDAN—handles a specific, repeatable business process. Examples include:

- Following up with new sales leads
- Reviewing invoice exceptions
- Preparing customer escalation briefs
- Creating weekly operating reports

AIDAN is not meant to be an open-ended chatbot that can do anything. Each agent receives:

- A clear job and measurable outcome
- A step-by-step process to follow
- Access only to approved business systems
- Rules defining what it can and cannot do
- Spending and usage limits
- Approval checkpoints for risky decisions
- An audit record of every action

The goal is simple: let AI handle routine work while people keep control of judgment, risk, and accountability.

---

## 2. The Two Ways People Use AIDAN

Use the **View as** menu at the top of the product to switch between the two experiences.

### Operations Admin / Buyer

This view is for the person responsible for the AI program. This may be an operations leader, department manager, process owner, or approved administrator.

Admins use AIDAN to:

- Choose which workflows should be automated
- Deploy and manage agents
- Connect company systems
- Set permissions and approval rules
- Monitor active work and exceptions
- Review audit records
- Measure business value and operating cost

### Employee / Approver

This view is for employees who delegate work to agents or make decisions when an agent reaches a boundary.

Employees use AIDAN to:

- Submit a business request
- Review the proposed plan before work starts
- Follow progress
- Add missing information
- Approve, edit, or decline sensitive actions
- Review completed work and its sources

Employees do not need to choose AI models, configure software, or build automations.

---

## 3. Before the First Workflow Is Launched

The workflow owner should answer five questions:

1. **What business outcome are we trying to improve?**  
   Example: Contact every qualified inbound lead within five minutes.

2. **How is the process handled today?**  
   Write down the current steps, owner, systems used, common exceptions, and typical handling time.

3. **How will we measure success?**  
   Use a business measure such as response time, appointments booked, hours saved, errors reduced, or revenue protected.

4. **Which decisions require a person?**  
   Examples include pricing changes, refunds, external messages, contract decisions, access to sensitive files, or low-confidence recommendations.

5. **Who owns the workflow after launch?**  
   Every workflow needs one named business owner who reviews performance and handles problems.

Do not automate a process that the team cannot explain. First simplify the process, then automate the stable steps.

---

## 4. How an Admin Launches a Workflow

Select **Deploy workflow** and complete the four setup stages.

### Step 1: Choose the Outcome

Choose one measurable process from the available templates or start from scratch.

Good first workflows are:

- Repeated frequently
- Based on clear business rules
- Time-consuming but not highly creative
- Easy for a person to verify
- Valuable when completed faster or more consistently

Avoid starting with a company-wide agent that has broad access and an unclear job.

### Step 2: Confirm the Runbook

The runbook is the approved step-by-step process the agent follows.

Review:

- What starts the workflow
- What information the agent may read
- What actions the agent may take
- What result it should produce
- Where work should be delivered
- When the agent must stop and ask for help

If the written process does not match how the team actually works, fix the runbook before continuing.

### Step 3: Set Guardrails

Guardrails define the agent's safe operating boundary.

For the first launch, use **Execute with gates**:

- Routine actions happen automatically within approved limits.
- Sensitive or unusual actions pause for a person.
- Low-confidence decisions are never treated as certain.
- Destructive actions remain blocked.
- Every action is logged.

Examples of sensible first-launch rules:

- Require approval for discounts above 15%.
- Require approval when confidence is below 80%.
- Block record deletion and pricing changes.
- Set a maximum operating cost per run.

Start conservatively. Expand autonomy only after the workflow produces reliable results over multiple real runs.

### Step 4: Test and Launch

Run the workflow in the sandbox before it touches live business data.

The test should confirm that the agent:

- Follows the correct steps
- Uses only approved systems and data
- Stops at the correct approval gates
- Produces a complete audit record
- Does not send messages or change records during the test

Launch only after the business owner reviews the test result.

---

## 5. The Employee's Daily Workflow

### Start in My Work

**My Work** is the employee's home screen. It shows:

- Items waiting for the employee
- Work currently being handled by agents
- Recently completed requests
- Agents available to that employee

Start here each morning and check **Waiting on me** first. An agent may be paused because it needs approval, missing information, or a business judgment.

### Submit a New Request

Select **New request** or **Ask an agent**.

Describe the result you need, not the AI technique you think should be used.

**Good request:**

> Prepare a renewal brief for Brightpath before my 2:00 PM call. Include account risks, recent activity, and recommended next actions.

**Weak request:**

> Analyze Brightpath.

Include:

- The desired outcome
- The deadline
- Important business context
- The correct data-sensitivity level
- Any limits the agent should respect

### Review the Plan

Before work starts, AIDAN shows:

- Which approved agent will handle the request
- Which company systems it will read
- What it plans to produce
- Whether it will take external actions
- Its estimated cost limit
- Where approval may be required

Do not start the request if the plan includes unnecessary access or does not match the intended outcome.

### Follow Progress

After the request starts, return to **My Work**.

The employee normally does not need to watch every step. AIDAN should notify the employee only when:

- The agent needs missing information
- A policy requires approval
- The workflow encounters an exception
- The final result is ready

### Review the Result

Before using the result:

- Check that the correct customer, account, time period, or project was used.
- Review the cited business sources.
- Confirm that recommendations make sense in the current situation.
- Correct the result if important context was missing.

AIDAN can prepare and recommend. The employee remains responsible for professional judgment.

---

## 6. How to Handle an Approval

The **Approvals** screen should make a decision fast without hiding the risk.

For every approval, review:

1. **Proposed action** — What exactly will happen?
2. **Business impact** — Which customer, record, amount, or team is affected?
3. **Reason** — Why is the agent recommending this action?
4. **Evidence** — Which company sources support the recommendation?
5. **Policy gate** — Which company rule caused the pause?
6. **Confidence** — How certain is the agent, and what remains unknown?
7. **Deadline** — When does the decision need to be made?

Then choose one action:

- **Approve:** The recommendation is correct, supported, and within company policy.
- **Edit terms:** The general action is right, but a value, message, date, amount, or condition needs to change.
- **Decline:** The action is wrong, unsafe, unnecessary, or unsupported.

Never approve an item simply to clear the queue. If the evidence is incomplete, decline it or request more context.

The decision, approver, time, and resulting agent action should be added automatically to the audit log.

---

## 7. Admin Screen Guide

### Command Center

Use this screen for the daily operating check.

Review:

- Work completed
- Estimated hours returned to teams
- Revenue or pipeline protected
- Items needing human decisions
- Live workflows
- Connection problems
- Automation rate

Focus on exceptions and business outcomes. A high number of agent runs is not success by itself.

### Workflows

Use this screen to manage repeatable business processes.

For each workflow, confirm:

- A named owner is assigned.
- The runbook matches the real process.
- The success rate remains acceptable.
- Exceptions are understood.
- The workflow is live, paused, or still a draft for a clear reason.

Use **Test run** after changing steps, permissions, policies, or connected systems.

### Agent Team

Use this screen to understand each agent's job and limits.

Each agent should have:

- One clear business goal
- A department owner
- A short list of approved tools
- A monthly or per-run spending limit
- Defined escalation conditions
- A clear list of prohibited actions

If two agents have overlapping jobs, simplify their responsibilities before adding more agents.

### Approvals

Use this screen to review sensitive decisions and monitor approval delays.

If the same safe decision appears repeatedly, the workflow owner may consider adjusting the policy. Do not remove an approval gate until real evidence shows the action is predictable and low risk.

### Audit Log

Use this screen to answer:

- What started the workflow?
- What information did the agent use?
- Which policy was applied?
- What did the agent decide?
- Who approved the action?
- What changed in the business system?
- How much did the run cost?

Use **Export evidence** for compliance review, customer disputes, internal investigations, or process improvement.

### Connections

Use this screen to control access to business systems such as the CRM, email, messaging, finance, support, or file storage platforms.

Connecting a system should not automatically grant every agent access. Grant only the minimum access required for the agent's job.

Review connections when:

- A credential or connection is expiring
- A team changes software
- An employee or vendor loses access
- A workflow starts reading unexpected data
- A new agent is launched

### Policies & Access

Use this screen to set company-wide safety rules.

Typical rules include:

- Approval before external communication
- Blocking destructive data actions
- Masking sensitive customer information
- Pausing low-confidence decisions
- Limiting which agents can use finance, email, file, or CRM systems

Policy changes should have a named approver and a recorded reason.

### ROI Report

Use this screen for the weekly or monthly leadership review.

Track:

- Verified time saved
- Revenue protected or created
- Platform and AI operating cost
- Net operating value
- Error and exception rates
- Approval speed
- Unauthorized actions or policy breaches

Review the assumptions behind ROI calculations. Time saved should be based on a real baseline, not a guess designed to make the result look impressive.

---

## 8. Recommended Operating Rhythm

### Employees — Daily

- Check **My Work**.
- Handle items waiting for input or approval.
- Review completed results before using them.
- Report inaccurate or unsafe behavior to the workflow owner.

### Workflow Owners — Weekly

- Review success, exception, and approval rates.
- Sample several completed runs for quality.
- Review failed or declined actions.
- Confirm integrations are healthy.
- Update the runbook when the real process changes.

### Operations Leadership — Monthly

- Review verified ROI and operating cost.
- Decide whether to expand, pause, or retire each workflow.
- Review access and policy changes.
- Check for repeated exceptions that indicate a broken process.
- Approve additional autonomy only when supported by evidence.

---

## 9. Safety Rules for Every User

1. Do not place passwords, private keys, payment details, or unnecessary personal information into a request.
2. Select the correct data-sensitivity level.
3. Verify important names, amounts, dates, recipients, and source records.
4. Treat confidence as a warning signal, not proof that an answer is correct.
5. Never approve an action without understanding its effect.
6. Do not disable a policy gate just to make the workflow faster.
7. Pause the workflow if behavior is unexpected or potentially harmful.
8. Use the audit log to investigate what happened before rerunning work.
9. Report repeated errors to the workflow owner so the process can be corrected.
10. Keep final accountability with a named person or department.

---

## 10. Troubleshooting

### The Agent Is Waiting

Open **My Work** or **Approvals**. The agent may need a decision, missing context, or access to an approved source.

### A Connection Has Expired

Open **Connections**, reconnect the system, and verify the allowed permissions. Do not rerun failed work until the connection is confirmed.

### The Result Is Inaccurate

Do not use or approve it. Check whether the source data was wrong, important context was missing, or the runbook used the wrong rule. Correct the source or runbook before trying again.

### The Agent Took an Unexpected Action

Pause the workflow, open the **Audit Log**, record the affected systems and records, and notify the workflow owner. Do not hide or silently correct the incident.

### Too Many Items Require Approval

Review the repeated approval type with the workflow owner. The underlying process or policy may need improvement. Keep the gate in place until the team has enough evidence to make a safe change.

### The ROI Report Looks Too High or Too Low

Review the baseline time, labor cost, business outcome value, and attribution assumptions. Use conservative, documented numbers.

---

## 11. Status Glossary

| Status | Meaning | User action |
|---|---|---|
| Draft | The workflow or agent is not live | Finish setup and testing |
| Live | The workflow is available for real work | Monitor outcomes and exceptions |
| Active / Running | The agent is currently working | No action unless requested |
| Scheduled | Work will begin at a defined time | Confirm the schedule is still correct |
| Waiting | The agent needs input, access, or approval | Open the item and respond |
| Needs review | A quality, policy, or operating issue needs attention | Assign the business owner |
| Completed / Delivered | The workflow finished | Review the result before using it |
| Blocked | A policy prevented the action | Investigate; do not bypass casually |

---

## 12. The Best First Rollout

Start with one department, one workflow, one owner, and one measurable outcome.

For the first 30 days:

1. Run with approval gates enabled.
2. Review a sample of completed work every week.
3. Record errors, missing context, and employee feedback.
4. Compare the results with the previous manual process.
5. Expand only after the workflow proves useful, safe, and understandable.

The objective is not to deploy the most agents. The objective is to improve a real business outcome without creating new operational risk.

