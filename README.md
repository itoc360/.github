<div align="center">
  <img src="https://raw.githubusercontent.com/itoc360/.github/main/profile/logo.svg" alt="ITOC360" width="100"/>
  <h1>ITOC360</h1>
  <p><strong>AI-First Incident Orchestration for SRE & DevOps Teams</strong></p>
  <p>
    Stop fighting alert storms. Start resolving incidents faster.
  </p>

  [![Website](https://img.shields.io/badge/Website-itoc360.com-0066FF?style=flat-square)](https://itoc360.com)
  [![Docs](https://img.shields.io/badge/Docs-docs.itoc360.com-orange?style=flat-square)](https://docs.itoc360.com)
  [![Integrations](https://img.shields.io/badge/Integrations-50+-brightgreen?style=flat-square)](https://itoc360.com/integrations)
  [![Free Trial](https://img.shields.io/badge/Free_Trial-No_CC_Required-success?style=flat-square)](https://itoc360.com)
</div>

---

## The SRE Problem We Solve

You built a robust monitoring stack. Prometheus scrapes every metric. Grafana fires on every threshold. CloudWatch watches every Lambda. Zabbix tracks every host.

And yet — **your on-call engineers are exhausted.**

Because monitoring tools detect problems. They don't manage them.

- 3 AM. 47 alerts firing simultaneously for the same root cause.
- No clear owner. No escalation. No context.
- Engineer spends 40 minutes triaging noise instead of fixing the issue.

**This is alert fatigue. This is on-call burnout. This is what ITOC360 eliminates.**

---

## What ITOC360 Does

ITOC360 sits between your monitoring stack and your engineering team — correlating, enriching, and orchestrating every alert into a single actionable incident.


**Key capabilities:**

- **Alert Correlation & Deduplication** — Group hundreds of related alerts into a single incident. Eliminate duplicate pages.
- **AI-Powered Prioritization** — Severity, environment, service tags, and custom rules determine who gets paged and when.
- **Automated Escalation Policies** — Define policy-driven escalation chains. If unacknowledged, it escalates. Automatically. Always.
- **On-Call Schedule Management** — Primary/secondary rotations, follow-the-sun coverage, holiday overrides, multi-team handoffs.
- **Multi-Channel Notifications** — Phone call, SMS, email, Slack, Microsoft Teams. Simultaneously. No missed pages.
- **Maintenance Windows** — Silence alerts during deployments and patch cycles. Zero false pages.
- **Full Incident Timeline** — Automatic ownership assignment, acknowledgement tracking, and audit trail from alert to resolution.

---

## Impact on SRE Metrics

| Metric | Before ITOC360 | After ITOC360 |
|--------|---------------|---------------|
| Alert noise | Hundreds of raw alerts | **70% reduction** |
| MTTA (Mean Time to Acknowledge) | Minutes of triage | Instant — right engineer paged |
| MTTR (Mean Time to Resolve) | Slowed by context-gathering | Reduced — enriched incident delivered |
| Missed incidents | Risk during alert storms | Eliminated via guaranteed escalation |
| On-call burnout | High | Significantly reduced |
| SLA/SLO compliance | At risk | Protected |

---

## Products

### [On Call](https://itoc360.com/products/on-call/)
Intelligent on-call scheduling and escalation automation for SRE teams.  
Supports primary & secondary rotations · Follow-the-sun · Holiday overrides · Multi-team coverage

### [IncidentOps](https://itoc360.com/products/incidentops/)
End-to-end incident detection, correlation, and response.  
AI-powered grouping · Root cause context · Automatic assignment · Full timeline visibility

---

## Integrations

### Monitoring & Observability
Prometheus · Grafana · Grafana Mimir · Zabbix · PRTG Network Monitor · Nagios · SolarWinds Orion · Instana · SigNoz · AppDynamics

### APM & Error Tracking
New Relic · Datadog · Dynatrace · Rollbar · Elastic / Kibana

### Cloud & Infrastructure
Amazon CloudWatch · AWS Budgets · Google Cloud Monitoring · Google Security Command Center · Azure Monitor · Azure Activity Logs · Microsoft Sentinel · Terraform Cloud

### ChatOps & Collaboration
Slack · Microsoft Teams · Statuspage.io

### Security
Amazon GuardDuty · CrowdStrike

### CI/CD & Developer Tools
GitHub · GitLab · Jenkins · n8n

### Ticketing & ITSM
Jira · Linear

→ **[View all 50+ integrations with setup guides](https://itoc360.com/integrations/)**

---

## Quick Start

Send your first alert in under 60 seconds:

```bash
curl -X POST https://api.itoc360.com/v1/alerts \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "title": "High CPU on prod-server-01",
    "severity": "critical",
    "source": "custom",
    "description": "CPU usage at 98% for 5 minutes"
  }'
