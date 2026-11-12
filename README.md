> [!IMPORTANT]
> **Live workbench: https://gmrmk.github.io/mythos-gatekeeper/**

# Mythos 5.2 Gatekeeper

A simulated review desk for access cases in the launch week of Claude Fable 5.2 and Claude Mythos 5.2. It is one HTML file. It makes no network calls and all of its data is invented.

**Independent concept prototype. Not affiliated with, endorsed by or connected to Anthropic.** Every organization, person and log line is synthetic. The program rules are paraphrased from public program pages read on 11 Nov 2026 and can be out of date. The desk procedures and the telemetry schema are simulated.

## Operational context

- **The review step.** Fable 5.2 is generally available, with safeguards that block or limit risky cybersecurity and biology work. Mythos 5.2 is the same model for vetted users in two programs: the Cyber Verification Program (CVP) and the Life Sciences Verification Program (LSVP). When an account asks for Mythos 5.2 and cannot have it, Fable 5.2 answers instead. A human reviewer decides the cases that sit between the two. This workbench models that step.
- **The point of view.** The view is that of a researcher with CVP approval, who knows the access process from the applicant side. The workbench maps the other side of the same process: what a reviewer reads, checks and decides.
- **The output.** Each decision feeds a week 1 report. The report names three gaps in the written runbook and gives a checklist change and a detection rule in SQL and Splunk SPL for each gap.

## The five cases

| Case | Request | Telemetry checked (SQL and Splunk SPL) | Reference decision | Gap |
|---|---|---|---|---|
| GK-4471, Quillmere Security LLC (CVP) | Red Team Access, Fast mode and a rate-limit raise for a 19-day-old pentest LLC | Token velocity. IP and ASN shifts. Fable limit reset. Classifier interventions. Payment and enforcement linkage. | Decline and refer to Investigations | GAP-1 |
| GK-4489, Lumen Fold Therapeutics (LSVP) | Life Sciences enrollment for a protein-design agent swarm on a BAA organization | Token velocity. IP and ASN shifts. Fable limit reset. Classifier interventions. Compliance state and PHI boundary. | Approve Standard Use on a new non-BAA organization, with conditions | GAP-2 |
| GK-4502, Cedar Hollow Regional Water Authority (CVP) | Defense Access or Red Team Access for a water utility and two maintainers before a Saturday patch window | Token velocity. IP and ASN shifts. Fable limit reset. Classifier interventions. Program enrollment and application state. | Defense Access now, Red Team application left open | GAP-1 |
| GK-4517, Harborline Financial Group (CVP) | Fallback appeal: a Defense Access workspace is answered by Fable 5.2 and its incident automation is failing | Token velocity. IP and ASN shifts. Fable limit reset. Classifier interventions. Retention and enrollment state. Bedrock calls (customer evidence). | Confirm eligibility and extend the retention exemption to Mythos 5.2 on cfc-ir | GAP-2 |
| GK-4533, Solvanger Lab, Ostrander University (LSVP) | Account takeover or shared key: one seat in a life sciences lab spends three limit resets overnight | Token velocity. IP and ASN shifts. Fable limit reset. Classifier interventions. Auth events and credential lineage. | Quarantine seat gsr-14 and keep the lab running | GAP-3 |

The three gaps:

- **GAP-1.** Defense Access as the interim tier has no linkage precondition, no owner and no clock.
- **GAP-2.** Eligibility rules name the path out of a blocking compliance state and give it no owner, clock or check.
- **GAP-3.** A grant attaches to the organization, while its requirements and its compromises live at the seat and the credential.

The full report for the five reference decisions is in this repository: [WEEK1_SAFEGUARDS_RUNBOOK_GAPS.md](WEEK1_SAFEGUARDS_RUNBOOK_GAPS.md). The workbench built it: the walkthrough decided the five cases, and the report tab gave the file.

## How to use it

1. Open the live link.
2. Select **Run auto-triage walkthrough (60s demo)**. It opens each case, shows the rule that is not met, runs one search, files the reference decision and builds the report.
3. Or do a case by hand. Read who asks. Run the checks. Choose a verdict and commit it. Copy the two notices.
4. Open the report tab and download the report.

## Files

| File | Content |
|---|---|
| `index.html` | The workbench. Styles, icons, data and code are inside the file. |
| `WEEK1_SAFEGUARDS_RUNBOOK_GAPS.md` | The report that the workbench builds from the five reference decisions. |

## Notes

- The page keeps its state in the local storage of the browser. It sends nothing. Reset clears the state.
- Tested in Chrome and Microsoft Edge on Windows, with keyboard, mouse and emulated touch. Not yet run in Firefox or Safari. By its code the page needs Chrome 105, Firefox 121 or Safari 15.5, or a later version.
- Built with Tailwind CSS 3.4.17 (MIT) and Lucide 0.544.0 icons (ISC). Both are compiled into the file.
- Made by Claude Mythos 5.2 in Claude Code, with Claude Opus 5.5 and Sonnet 5.5 workers.
