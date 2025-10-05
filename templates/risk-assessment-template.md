# Risk Assessment Template

Use this template to document new risk assessments or periodic reviews. Align scoring with the Risk Assessment Methodology and capture decisions in the Risk Treatment Plan.

## 1. Context

| Item | Details |
| --- | --- |
| Assessment Name | |
| Business Function / Process | |
| Assessment Trigger (project, change, review) | |
| Prepared By | |
| Date Initiated | |
| Review Cycle | |

## 2. Scope and Assumptions

- **In-Scope Assets / Services:** 
- **Excluded Items:** 
- **Assumptions / Dependencies:** 

## 3. Risk Matrix (define scoring reference)

| Likelihood Score | Description |
| --- | --- |
| 1 | Rare – Exceptional circumstances only |
| 2 | Unlikely – Could occur at some time |
| 3 | Possible – Might occur at least annually |
| 4 | Likely – Expected to occur multiple times per year |
| 5 | Almost Certain – Expected to occur frequently |

| Impact Score | Description |
| --- | --- |
| 1 | Negligible – Minimal impact, easily contained |
| 2 | Minor – Limited operational disruption |
| 3 | Moderate – Noticeable service impact or regulatory concern |
| 4 | Major – Significant disruption, reportable breach likely |
| 5 | Severe – Critical failure, substantial legal/financial penalties |

### Likelihood vs Impact Heat Map

Use the heat map to plot each risk based on its likelihood and impact scores. Update the colour or labels to reflect your organisational scoring bands.

```mermaid
%%{init: {"theme": "neutral"}}%%
heatmap
    title Risk Heat Map (Higher values = greater risk)
    xAxis Likelihood 1 2 3 4 5
    yAxis Impact 5 4 3 2 1
    data
        1 5 1
        2 5 2
        3 5 3
        4 5 4
        5 5 5
        1 4 2
        2 4 3
        3 4 4
        4 4 5
        5 4 6
        1 3 3
        2 3 4
        3 3 5
        4 3 6
        5 3 7
        1 2 4
        2 2 5
        3 2 6
        4 2 7
        5 2 8
        1 1 5
        2 1 6
        3 1 7
        4 1 8
        5 1 9
```

> **How to use:** Place the Risk ID in the relevant likelihood/impact cell. Highlight cells (e.g., green/amber/red) according to your risk appetite.

## 4. Risk Register

| Risk ID | Threat / Vulnerability Description | Impacted Assets / Processes | Existing Controls | Likelihood | Impact | Inherent Risk (L × I) | Control Effectiveness (0–1) | Additional Controls / Actions | Control Owner | Target Date | Residual Risk |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |  |  |  |  |  |

> **Residual Risk Formula:** Residual Risk = (Likelihood × Impact) × (1 − Control Effectiveness). Adjust the formula if your methodology uses alternative scaling (e.g., qualitative bands or weighted factors).

## 5. Risk Acceptance and Treatment Decisions

| Risk ID | Decision (Accept / Mitigate / Transfer / Avoid) | Decision Rationale | Approver | Approval Date |
| --- | --- | --- | --- | --- |
|  |  |  |  |  |
|  |  |  |  |  |

## 6. Review and Closure

- **Follow-up Actions Tracked In:** 
- **Next Scheduled Review:** 
- **Additional Notes:** 

> **Reminder:** Communicate high and critical risks to the Risk and Compliance Committee and ensure actions are reflected in the Corrective and Preventive Action (CAPA) log where applicable.
