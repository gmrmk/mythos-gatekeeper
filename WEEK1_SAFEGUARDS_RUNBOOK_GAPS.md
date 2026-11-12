# Week-1 Launch Surge Insights Report

Policy gap and telemetry runbook. Claude Fable 5.2 and Mythos 5.2 launch: Mon 9 Nov to Wed 11 Nov 2026, launch day to launch day +2

Status: Complete (5 of 5 cases decided). Prepared by: specialist\-01. Generated: 12 Nov 2026 03:04:57 UTC.
Audience: Safeguards Policy and Safeguards Engineering leads.

> Simulation. This report comes from an independent concept prototype that is not affiliated with or endorsed by Anthropic. Every organization, person, log line and identifier in this report is synthetic. Written criteria are paraphrased from the public program pages listed under Sources; desk procedures and the telemetry schema are simulated.

## 1. Executive summary

- In the first three days of the Fable 5.2 / Mythos 5.2 launch, five escalated access cases reached specialist review. 5 of 5 are decided: 1 approved or routed, 2 conditionally approved, 1 declined, 1 contained.
- The written access criteria held where a case matched the form the page describes. They fell short in three places where a page names a condition and leaves the procedure unwritten.
- GAP-1 (P1, evidenced, 2 of 2 linked cases decided): Defense Access as the interim tier has no linkage precondition, no owner and no clock.
- GAP-2 (P1, evidenced, 2 of 2 linked cases decided): Eligibility rules name the path out of a blocking compliance state and give it no owner, clock or check.
- GAP-3 (P0, evidenced, 1 of 1 linked case decided): A grant attaches to the organization, while its requirements and its compromises live at the seat and the credential.
- Median handle time for decided cases: 8s.

## 2. Case dispositions

| Case | Organization | Program | Verdict | Handle time | Conditions |
|---|---|---|---|---|---|
| GK-4471 | Quillmere Security LLC | CVP, Red Team Access | Decline and refer to Investigations | 8s | 5 |
| GK-4489 | Lumen Fold Therapeutics | LSVP, Standard Use | Approve Standard Use on a new non-BAA organization, with conditions | 8s | 7 |
| GK-4502 | Cedar Hollow Regional Water Authority | CVP, Defense Access (applied for Red Team Access) | Defense Access now, Red Team application left open | 8s | 6 |
| GK-4517 | Harborline Financial Group | CVP, Defense Access, retention exemption | Confirm eligibility and extend the retention exemption to Mythos 5.2 on cfc-ir | 8s | 7 |
| GK-4533 | Solvanger Lab, Ostrander University | LSVP, Standard Use, security alert | Quarantine seat gsr-14 and keep the lab running | 56s | 6 |

## 3. Policy gaps

### GAP-1: Defense Access as the interim tier has no linkage precondition, no owner and no clock

Priority: P1. Owner: Safeguards Policy, with CVP intake. Evidence: Evidenced (2 of 2 linked cases decided). Criteria: CVP-RT-EVID, CVP-INTERIM, CVP-PENDING, CVP-DEF-ELIG, CVP-DEF-WHO, CVP-DEF-TIME, CVP-SCOPE, CVP-REAPPLY.

**Written criterion.** The Cyber Verification Program help article gives Red Team Access to organizations that show a firm credential or, for a smaller firm, a registration at least one year old with public services, certified testers and recent client evidence. An applicant for a higher tier that qualifies for a lower one receives the lower tier during review, and the announcement says qualifying organizations are enrolled in Defense Access while their Red Team application is reviewed, without defining qualifying. Defense Access is open to organizations and individuals on paid plans for defensive work, with a two-day review target and no evidence rows. An applicant who is not approved can reapply after seven days.

**What happened.**

- GK-4471: A 19-day-old LLC applied for Red Team Access with six attestations ticked and no evidence. The written evidence rows stopped it: no firm credential, and a registration far short of one year. The applicant then asked for "whatever tier turns the blocks off". Nothing written asks about its payment instrument, which sits in a cluster where 37 organizations were suspended by 17 September, or about the three sibling organizations that filed near-identical applications on 9 and 10 November. Defense Access, the tier it asked for by description, has no evidence rows to fail.
- GK-4502: A municipal water utility and two open-source maintainers needed to confirm a controller firmware flaw on a test bench before a patch window on 14 and 15 November. They filed for Red Team Access because the form's wording matched the task. The pages write a route for that situation: Defense Access while the Red Team application is reviewed. Nearly two days later the application was queued with no reviewer and no Defense Access enrollment. Nothing triggers that enrollment or owns it, nothing gives a dated deadline a faster lane, and the two maintainers, who cannot hold a Red Team application, were outside it altogether.

**Why the written rule falls short.** The interim rule is one sentence doing two jobs, and it is written for neither. For a linked applicant it is the weakest route in the program: Defense Access is granted on a description of defensive work, so an operator who fails the Red Team evidence rows can ask for the lower tier, or return through a sibling organization seven days later, and no written step looks at who else pays with the same instrument. For a legitimate applicant it is the right answer with nobody assigned to give it: the rule says what the applicant receives, and not who decides, by when, or how an organization and the individuals working with it are handled together.

**Risk if unaddressed.** Output-extraction rings obtain relaxed cyber safeguards through Defense Access by description, one organization at a time. Critical infrastructure operators and maintainers wait in a Red Team queue through disclosure and patch windows for access the page already gives them.

**Proposed change.** Give the interim tier a procedure. Run a linkage check against enforcement records before any tier decision, and let an adverse result end the review at every tier. Require one piece of positive evidence of defensive work before Defense Access is granted as the lower tier. Give the interim decision an owner and the two-day Defense target from the moment a Red Team application is filed, with a one-business-day lane for a dated external deadline. Route by the work described, not the tier ticked. Attach the reapply wait and the decline reason to the linked cluster. Define a joint case for an organization and named individuals.

**Proposed checklist updates**

- [ ] Intake, every tier: run the payment, device and infrastructure linkage check against enforcement clusters before reading the application. Adverse linkage ends the review and opens a referral.
- [ ] Intake, Red Team: test the evidence rows first. No firm credential and a registration under one year is a decline on the written criteria. Record the date the registration reaches one year.
- [ ] Lower tier during review: grant Defense Access only with no adverse linkage and one piece of positive evidence of defensive work on the applicant's own systems. Record both in the decision.
- [ ] Interim decision: every Red Team application gets a Defense Access decision inside the two-day Defense target, with a named owner. A queued application with no interim decision after two days raises an alert.
- [ ] Urgency lane: an applicant with a dated external deadline (a patch window, a disclosure embargo, an active incident) gets the interim decision within one business day.
- [ ] Routing: classify by the work described, not the tier ticked. Vulnerability validation, patch verification and detection writing are Defense Access work even when the form says Red Team.
- [ ] Joint cases: one case for an organization plus named individual maintainers. Individuals enroll on their own plans, covering only themselves, and are linked to the case.
- [ ] Team plans: access covers every seat. Name the users who do the work in the decision record and state the scope in the notice.
- [ ] Reapply: the seven-day wait and the decline reason attach to the linked cluster, so a sibling organization cannot refile the same application.
- [ ] External use: when the stated work is for clients, say in the notice that it needs its own approval after program approval.
- [ ] Notices: a decline states what the published criteria require and the reapply rule, and never the linkage.

**Evidence from this shift**

- GK-4471: Decline and refer to Investigations. The written evidence rows stopped this application on their own: no firm credential, and a registration 19 days old against the one-year test. But the written criteria do not reach the applicant behind the form. Nothing in them asks about the payment link to a cluster under enforcement or about the three other applications from the same cluster. The seven-day reapply wait follows the organization and not the cluster. Defense Access, which the applicant asked for by description, has no evidence rows at all.
- GK-4502: Defense Access now, Red Team application left open. The form offered one option, and the words "exploit development" sent the utility toward a tier that it is unlikely to hold in time. The announcement names open-source maintainers and critical infrastructure operators of any size (CVP-DEF-WHO), and it enrolls a qualifying organization in Defense Access while its Red Team application is reviewed (CVP-PENDING). The help article gives the lower tier to an applicant that qualifies (CVP-INTERIM), and nobody applied that route to the application as filed. So the gap is not a missing rule: nothing triggers or owns the interim enrollment, and the pages give no urgency lane for a dated patch window. The maintainers sit outside the route because individuals cannot hold a Red Team application. These gaps leave the outcome to a specialist who reads the work and not the form.

Linked detections: DET-01, DET-02.

### GAP-2: Eligibility rules name the path out of a blocking compliance state and give it no owner, clock or check

Priority: P1. Owner: Safeguards Policy, with Legal and Privacy and Sales operations. Evidence: Evidenced (2 of 2 linked cases decided). Criteria: LSVP-BAA, LSVP-REQ, LSVP-RET, LSVP-TYPES, RET-01, RET-02, RET-04, CVP-ZDR, CVP-EVAL, RET-BEDROCK, RET-ZDR-EFS.

**Written criterion.** The Life Sciences Verification Program help article says an organization under a Business Associate Agreement cannot receive a grant, and that research without protected health information is eligible in a separate organization that is not under a BAA. It requires a dedicated workspace, phishing-resistant MFA and Workload Identity Federation, and says decisions typically come within about three business days. For zero-retention customers, the Mythos model page says eligible Cyber Verification Program customers who already have zero data retention can keep it for Mythos 5.2 until Enterprise Frontier Safeguards is available. The program help article gives an organization with a data retention exemption zero retention on all program models, for internal use, and the retention article says some organizations receive a notice that they may use Fable with zero retention. For a model called through Amazon Bedrock, the AWS pages put the data retention mode in the customer's own AWS account (RET-BEDROCK) and make zero retention there a question for its AWS account team (RET-ZDR-EFS); the desk sees none of that traffic.

**What happened.**

- GK-4489: A verified biotech on a HIPAA-ready Enterprise plan asked for a life sciences grant for its protein-design swarm, with a funder milestone on 1 December. The page says what blocks it and names the way through in one clause. It does not say who opens the second organization, how long that takes, what the customer attests to, or what stops health data or a credential from following the team across. The swarm ran on two stored keys shared by up to 180 workers, where the program asks for Workload Identity Federation, and one of those keys also reached the workspace that holds health information.
- GK-4517: A bank's Cyber Fusion Center, enrolled in Defense Access since August under a zero data retention addendum with an exemption on file, saw every Mythos 5.2 request answered by Fable 5.2 from launch. The help article gives an exemption holder zero retention on all program models, so Mythos 5.2 was covered on the page from launch. Nothing owns applying that to the exemption on file, verifying it or delivering the notice: the desk pass that does it had not reached this customer, and the notice had bounced off a contact who left in September. Its automation retried failed calls up to five times and drove the workspace into its rate limit during a live investigation.
- GK-4517: The same customer's disaster-recovery playbooks call Fable 5.2 through Amazon Bedrock, and every call since 9 November fails because a service control policy of its own AWS organization pins the retention mode to none. The mode is the customer's to change in its AWS account, and the desk saw only the CloudTrail excerpt the customer sent.

**Why the written rule falls short.** Each rule is a gate with its exit described in a subordinate clause. The exit has no owner, no target time, no verification steps and no scope, so the specialist improvises it under time pressure and the customer learns about the gate by hitting it. Both teams qualified. The BAA organization needed the written route out, and the exemption holder needed the written rule applied. In each case the procedure failed, not the policy.

**Risk if unaddressed.** Verified life sciences customers under a BAA are declined or stalled past funded milestones, or are approved on the wrong organization and put health data under 30-day program retention. Eligible zero-retention customers fall back silently at every model launch, and their automation turns a routing decision into an outage. Each improvised fix sets a different precedent for scope.

**Proposed change.** Write the exits as procedures. For the BAA split: an owner, a five-business-day target, a health-data attestation, a check that no credential or identity reaches both organizations, and the program's own requirements (dedicated workspace, phishing-resistant MFA, identity federation) confirmed before the grant goes live. For the retention exemption: verification steps the specialist can run from records, a default scope of the enrolled workspace, a notice that goes to the program's security contact and is tracked to delivery, and exemptions applied to a new program model before its launch hour, not after it.

**Proposed checklist updates**

- [ ] BAA organizations: when a life sciences request arrives from one, open the organization split on day one. Owner: the account team. Target: five business days to a live organization that is not under a BAA.
- [ ] BAA split: collect a signed attestation that no protected health information enters the new organization, and name the customer's owner for it.
- [ ] BAA split: before the grant goes live, confirm the written requirements in the new organization: a dedicated workspace, phishing-resistant MFA on every seat that uses the apps, and Workload Identity Federation for API access, with no identity that reaches the BAA organization.
- [ ] Agent pipelines under a grant: require a human checkpoint before any tool that orders, synthesizes or ships, and a cap on run length and worker count, written into the grant.
- [ ] Approval notices: say that Fable keeps its biology safeguards, that the pipeline must call a program model in the program organization, and whether the work is covered by Standard Use or needs the High-risk Use add-on.
- [ ] Retention exemption: verify from records in this order: zero-retention addendum date, exemption on file and the models it lists, program enrollment and its workspace, internal use, notice delivery. Extend the exemption to the enrolled workspace only.
- [ ] Retention exemption: record internal-use scope and the customer's Enterprise Frontier Safeguards intent in the decision.
- [ ] Notices: send eligibility notices to the program security contact as well as the billing contact, and treat a bounce as an open task with an owner.
- [ ] Model launches: apply existing exemptions to the new program model before the launch hour. If the backlog is not zero at launch, publish its size to the queue.
- [ ] Fallback appeals: check for client retry storms on every appeal and put the fix in the notice.

**Evidence from this shift**

- GK-4489: Approve Standard Use on a new non-BAA organization, with conditions. The BAA rule on the Life Sciences Verification Program help article names the state that blocks a grant and the separate organization, and nothing else. It gives no owner who opens the new organization, no schedule for the move itself and no control that keeps health data out of the new organization. This decision supplies all three as conditions (the account team as owner, access the week of 16 Nov 2026, a signed attestation and identity separation). No page writes them down. The swarm's workers share two stored API keys, and one of them reached the health-data workspace 26 times in seven days. These keys do not meet the program's Workload Identity Federation requirement (LSVP-REQ), and that shortfall is the credential-scope gap that GAP-3 cites.
- GK-4517: Confirm eligibility and extend the retention exemption to Mythos 5.2 on cfc-ir. The Mythos model page says that eligible customers keep zero retention. The Cyber Verification Program help article says that an organization with a retention exemption can use the program with zero retention for internal use. That page covers every program model, Mythos 5.2 included. The pages do not say who applies the exemption to a new model, who verifies it, what unit it attaches to or how the program delivers the notice. So a desk eligibility pass that did not reach Harborline left an enrolled workspace answered by Fable 5.2 for 43 hours, and a bounced notice kept the customer unaware. The extension of the exemption to one enrolled workspace, with conditions, shows the scope and the verification that the pages leave implicit.

Linked detections: DET-03, DET-04.

### GAP-3: A grant attaches to the organization, while its requirements and its compromises live at the seat and the credential

Priority: P0. Owner: Safeguards Engineering, with Safeguards Policy. Evidence: Evidenced (1 of 1 linked case decided). Criteria: LSVP-REQ, LSVP-GRANT, LSVP-MONITOR, LSVP-THREATS, LSVP-CYBER, OFFER-RESET, DESK-SCOPE, DESK-REMEDY, CVP-SEC-INCIDENT, DESK-XPROG.

**Written criterion.** The Life Sciences Verification Program help article requires phishing-resistant MFA for the Claude apps, Workload Identity Federation for the API and a dedicated workspace, and on a Team plan a grant attaches to the whole organization. It says usage is checked against the organization's stated scope, and that when activity looks out of scope the admin is notified and has one week to explain, narrow the scope or dispute. The announcement names access compromise, insider threats and agent misuse as the threat models. The launch offers article says a used limit reset cannot be undone. The Cyber Verification Program security requirements write the report within 72 hours for a breach or misuse involving the grant (CVP-SEC-INCIDENT). The duties of 24 hours and 48 hours do not carry that phrase, and no page reaches an incident in another organization or under another program.

**What happened.**

- GK-4533: At 02:47 on 11 November a graduate researcher's seat in a verified lab was entered from a hosting network after fourteen failed sign-ins. The program requires phishing-resistant MFA; the seat had none, two weeks after the grant was given to the organization. Two minutes later the intruder created a long-lived token, then spent the seat's three limit resets to keep a 70-minute burst of vulnerability-rediscovery requests going, including 96 requests through the lab's life sciences grant. The written response to out-of-scope activity is a notice to the admin and a week to reply. The same lab also ran its pipeline on a token shared by nine people, which looks similar on a dashboard and is a different problem.
- GK-4533: The university that holds Defense Access on a separate Enterprise organization shows no activity from the intruder's network, and no page binds its grant to an incident in the lab's organization. The desk therefore asked the university's security contact, as a request and not a rule, to work to the same times: report within 24 hours and investigate within 48 hours (DESK-XPROG).
- GK-4489: The protein-design swarm ran up to 180 workers on two stored keys, with no human checkpoint in three of five runs. The program asks for Workload Identity Federation. A grant given to that organization as it stood would have attached to credentials that no single person or workload owns.

**Why the written rule falls short.** A grant is given to an organization after a review of the organization, and on a Team plan it covers every seat. The pages state what each seat and workload must have. They do not say that anything checks a seat against those requirements when it uses the grant. An intruder needs one seat. Nothing written says what the specialist does in the first hour of a takeover, tells a takeover from a shared credential, or covers the launch offers a stolen seat inherits from its owner.

**Risk if unaddressed.** A single phished seat in a verified organization gives an outsider program-level access and three limit resets, for as long as it takes someone to read an alert. The available responses are too small (a notice) or too large (suspending the organization or revoking the grant), and the large ones act against the victim and stop verified research.

**Proposed change.** Enforce the written requirements where the grant is used: a seat that does not meet its program's MFA requirement, or a workload without a federated identity, cannot use a program model. Add a containment ladder that starts at the credential and climbs only on evidence: token, seat, workspace, organization. Give the specialist a written takeover-or-sharing test built on sign-in history. Alert when a program seat acts outside its program's domain, and when a limit reset is followed by a burst from a network the seat has never used.

**Proposed checklist updates**

- [ ] Enforcement at the seat: a seat that does not meet its program's MFA requirement cannot use a program model, whatever the organization attested at review (phishing-resistant for life sciences, Red Team and Specialized grants now, and for Defense Access from 15 Dec 2026). Check at sign-in, not only when the grant is given.
- [ ] Grant go-live: list every seat and workload identity that will use the grant and confirm each meets the written requirements. On a Team plan that is every seat in the organization.
- [ ] First hour: on a takeover pattern, lock the seat, end its sessions and revoke its tokens before any notice is drafted. The organization and its other seats keep working.
- [ ] Takeover or sharing: a takeover shows failed sign-ins, a network never seen for the organization, a new token and a change of subject. Sharing shows known networks, a stable subject and many people over weeks. Record which, and why.
- [ ] Scope of action: use the smallest scope that contains the incident. Suspending an organization or revoking a grant needs evidence that the organization, not a seat, is the problem.
- [ ] Notice: tell the organization owner and its security contact within one hour of containment: the seat, the window, what was locked and what they need to do. The one-week window for out-of-scope activity starts after containment, not in place of it.
- [ ] Cross-program alert: cyber safeguard events on a seat whose only grant is life sciences, or the reverse, page the on-call specialist.
- [ ] Incidents across programs: write down who reports and who investigates when an incident crosses programs or organizations. Until it is written, ask the holder of the related grant, as a request, to report within 24 hours and investigate within 48 hours (DESK-XPROG).
- [ ] Limit resets: a reset redeemed from a network the seat has not used in 30 days is held for review. Resets spent by an intruder are restored to the owner, as a written remedy.
- [ ] Shared credentials: one key or token used by many people or many agent workers is a finding with a seven-day fix, and it blocks a new grant until it is fixed.
- [ ] After action: restore the seat only after the owner re-verifies and enrolls phishing-resistant MFA. Record the incident against the seat, not the grant.

**Evidence from this shift**

- GK-4533: Quarantine seat gsr-14 and keep the lab running. Verification attaches to the organization and the program, but this compromise sat on one seat and one credential and crossed programs (Fable outside the grant, Mythos 5.2 inside it). The Life Sciences Verification Program help article writes phishing-resistant MFA and Workload Identity Federation as requirements (LSVP-REQ) and attaches a Team grant to the whole organization (LSVP-GRANT). Nothing written enforces those requirements at the seat, and the one written response to out-of-scope activity is a notice and a one-week wait (LSVP-MONITOR), too slow for a live token. So the seat quarantine, with the admin told within the hour, rests on a desk rule and not on a program page, and that is the gap to close. The cyber program writes its 72-hour report for a breach or misuse involving the grant, and its 24-hour and 48-hour duties carry no word on an incident in another organization. So no page clearly binds the university's grant, and the desk asks its security contact for the same 24 and 48 hours from the decision, as a request (DESK-XPROG, DESK-CLOCK).

Linked detections: DET-05, DET-06, DET-07, DET-08.

## 4. Telemetry handoff

Proposed detections for Safeguards Engineering. Table and index names follow the simulated schema. Numeric cut-offs are starting values to tune against a baseline before any alert routes to a person.

### DET-01: Synchronized limit-reset redemption across a payment cluster

Closes: GAP-1. Purpose: Finds groups of organizations that share a payment cluster and redeem the Fable limit reset within the same ten minutes: one operator running many accounts. Lists the organizations in the burst, and how many organizations on the cluster have a program application open or an enforcement action in the last 365 days.

Routing: Runs hourly. Investigations queue, one alert per payment cluster, throttled on payment cluster and bucket for 24 hours, with the organization list from the query. Hold any open program application on those organizations until the alert is closed.

Tuning and false positives: Starting values: 3 or more organizations and 10 or more seats in one ten-minute bucket. The minutes after an offer opens are busy for everyone, so the shared payment cluster is the condition and timing alone never fires. Exclude known resellers and institutional purchasing accounts. Fixed buckets split a burst that straddles a boundary; a sliding window is the upgrade. The Splunk version expects three hourly lookups: payment_cluster_by_org (key organization, output payment_cluster_id); open_applications_by_cluster (key payment cluster, output cluster_orgs_with_open_applications), which counts organizations with an open row for a tier they do not already hold, read from the latest enrollment row per organization, workspace, tier and model scope; and actioned_orgs_by_cluster (key payment cluster, output cluster_orgs_actioned), which counts organizations with a suspension or termination in the last 365 days. The SQL bounds its read of enforcement_prod.actions to those 365 days so the hourly scan can prune; an older action does not count, and a summary table refreshed daily is the upgrade. bucket_start is a UTC timestamp in the SQL and text in the search time zone in the Splunk version: set that zone to UTC, or read the Splunk value as local time.

```sql
-- One row per payment cluster and ten-minute bucket in which 3 or more of its
-- organizations (10 or more seats) redeemed a Fable limit reset. The two cluster_ columns
-- count organizations anywhere on the cluster, not only those in the burst.
WITH org_cluster AS (
  SELECT DISTINCT org_id, payment_cluster_id
  FROM `billing_prod.payment_instruments`
),
resets AS (
  SELECT
    c.payment_cluster_id,
    r.org_id,
    r.seat_id,
    TIMESTAMP_SECONDS(600 * DIV(UNIX_SECONDS(r.reset_ts), 600)) AS bucket_start
  FROM `safeguards_prod.limit_reset_events` AS r
  JOIN org_cluster AS c
    ON c.org_id = r.org_id
  WHERE r.reset_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 24 HOUR)
),
bursts AS (
  SELECT
    payment_cluster_id,
    bucket_start,
    COUNT(DISTINCT org_id) AS orgs,
    COUNT(DISTINCT seat_id) AS seats,
    STRING_AGG(DISTINCT org_id, ', ' ORDER BY org_id) AS orgs_in_burst
  FROM resets
  GROUP BY payment_cluster_id, bucket_start
  HAVING COUNT(DISTINCT org_id) >= 3 AND COUNT(DISTINCT seat_id) >= 10
),
latest_enrollment AS (
  SELECT org_id, tier, status
  FROM `access_prod.program_enrollments`
  QUALIFY ROW_NUMBER() OVER (PARTITION BY org_id, workspace_id, tier, model_scope ORDER BY enrolled_ts DESC) = 1
),
-- An open application is an open row for a tier the organization does not already hold.
applicants AS (
  SELECT DISTINCT org_id
  FROM (
    SELECT
      org_id,
      tier,
      LOGICAL_OR(status IN ('queued', 'in_review')) AS has_open,
      LOGICAL_OR(status = 'active') AS has_active
    FROM latest_enrollment
    GROUP BY org_id, tier
  )
  WHERE has_open AND NOT has_active
),
open_apps AS (
  SELECT c.payment_cluster_id, COUNT(DISTINCT e.org_id) AS cluster_orgs_with_open_applications
  FROM applicants AS e
  JOIN org_cluster AS c
    ON c.org_id = e.org_id
  GROUP BY c.payment_cluster_id
),
actioned AS (
  SELECT c.payment_cluster_id, COUNT(DISTINCT a.org_id) AS cluster_orgs_actioned
  FROM `enforcement_prod.actions` AS a
  JOIN org_cluster AS c
    ON c.org_id = a.org_id
  WHERE a.action_type IN ('suspend', 'terminate')
    -- A constant bound, so the scan can prune: an action older than 365 days does not count.
    AND a.action_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 365 DAY)
  GROUP BY c.payment_cluster_id
)
SELECT
  b.payment_cluster_id,
  b.bucket_start,
  b.orgs,
  b.seats,
  b.orgs_in_burst,
  IFNULL(o.cluster_orgs_with_open_applications, 0) AS cluster_orgs_with_open_applications,
  IFNULL(x.cluster_orgs_actioned, 0) AS cluster_orgs_actioned
FROM bursts AS b
LEFT JOIN open_apps AS o
  ON o.payment_cluster_id = b.payment_cluster_id
LEFT JOIN actioned AS x
  ON x.payment_cluster_id = b.payment_cluster_id
ORDER BY b.seats DESC;
```

```spl
index=safeguards sourcetype=limit:reset earliest=-24h
| lookup payment_cluster_by_org org_id OUTPUT payment_cluster_id
| where isnotnull(payment_cluster_id)
| bin _time span=10m
| stats dc(org_id) AS orgs, dc(seat_id) AS seats, values(org_id) AS orgs_in_burst BY payment_cluster_id, _time
| where orgs >= 3 AND seats >= 10
| eval orgs_in_burst=mvjoin(orgs_in_burst, ", ")
| lookup open_applications_by_cluster payment_cluster_id OUTPUT cluster_orgs_with_open_applications
| lookup actioned_orgs_by_cluster payment_cluster_id OUTPUT cluster_orgs_actioned
| fillnull value=0 cluster_orgs_with_open_applications, cluster_orgs_actioned
| rename _time AS bucket_start
| eval bucket_start=strftime(bucket_start, "%Y-%m-%d %H:%M")
| table payment_cluster_id, bucket_start, orgs, seats, orgs_in_burst, cluster_orgs_with_open_applications, cluster_orgs_actioned
| sort - seats
```

### DET-02: Bulk-collection request shape on an organization with an open cyber application

Closes: GAP-1. Purpose: Scores every organization with an open Cyber Verification Program application for a tier it does not already hold on three measures of request shape over 14 days: share of single-turn requests, share of responses that end at max_tokens, and requests per distinct prompt template. Surfaces applicants whose traffic contradicts the stated use case before anyone reads the application, at any tier. Two counts ride along as context and do not enter the vote: the Mythos requests that ran in fast mode from a workspace that holds no cyber grant (cvp_tier is null; Mythos fast mode is for organizations in the verification programs, MOD-02), and the events where the output-extraction probe scored 0.80 or above, the action band (distillation_probe_score).

Routing: Runs daily and when an application is filed. CVP intake, as a flag on the application. Two of three measures over their starting value moves the application to specialist review with the linkage check attached, and the two context counts go with it.

Tuning and false positives: Starting values: single-turn share 0.90, max_tokens share 0.70, 100 requests per template, and at least 2,000 requests in the window. Batch evaluation and data labeling can look the same, so read the stated use case before acting. Baseline all three measures against approved program members before any alert routes to a person. The 0.80 probe cut is the written action band; the probe count has no starting value of its own and is read beside the vote. The fast mode count reads Mythos requests only: fast mode on Fable is open to customers on the platforms the launch page lists, so it is not counted. A Mythos fast mode count on a null cyber tier is a request for the premium lane and not a finding by itself; an organization that holds a life sciences grant also qualifies for Mythos fast mode and shows a null cyber tier, so read its enrollment first.

```sql
-- Request shape over 14 days for organizations with an open cyber application for a tier they do
-- not already hold. A member with a queued row for a new model under its own tier is not an
-- applicant; a Defense Access member with an open Red Team application is.
-- measures_over counts how many of the three shape measures pass their starting value.
-- fast_mode_no_grant (Mythos fast mode requests from a workspace with no cyber grant) and probe_hits
-- (probe score 0.80 or above) are context for the reviewer and do not enter the count.
WITH latest AS (
  SELECT org_id, program, tier, status
  FROM `access_prod.program_enrollments`
  QUALIFY ROW_NUMBER() OVER (PARTITION BY org_id, workspace_id, tier, model_scope ORDER BY enrolled_ts DESC) = 1
),
applicants AS (
  SELECT DISTINCT org_id
  FROM (
    SELECT
      org_id,
      tier,
      LOGICAL_OR(status IN ('queued', 'in_review')) AS has_open,
      LOGICAL_OR(status = 'active') AS has_active
    FROM latest
    WHERE program = 'CVP'
    GROUP BY org_id, tier
  )
  WHERE has_open AND NOT has_active
),
shape AS (
  SELECT
    a.org_id,
    COUNT(*) AS requests,
    SAFE_DIVIDE(COUNTIF(a.turn_index = 1), COUNT(*)) AS single_turn_share,
    SAFE_DIVIDE(COUNTIF(a.output_tokens >= a.max_tokens), COUNT(*)) AS max_tokens_share,
    COUNT(DISTINCT a.prompt_template_hash) AS templates,
    COUNTIF(a.fast_mode_16_80_mtok AND a.cvp_tier IS NULL AND STARTS_WITH(a.model_id, 'claude-mythos')) AS fast_mode_no_grant
  FROM `safeguards_prod.api_requests` AS a
  JOIN applicants AS p
    ON p.org_id = a.org_id
  WHERE a.request_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 14 DAY)
    AND a.http_status = 200
  GROUP BY a.org_id
),
-- The output-extraction probe: 0.80 and above is the action band.
probe AS (
  SELECT
    e.org_id,
    COUNTIF(e.distillation_probe_score >= 0.80) AS probe_hits
  FROM `safeguards_prod.classifier_events` AS e
  JOIN applicants AS p
    ON p.org_id = e.org_id
  WHERE e.event_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 14 DAY)
  GROUP BY e.org_id
),
scored AS (
  SELECT
    s.org_id,
    s.requests,
    ROUND(s.single_turn_share, 3) AS single_turn_share,
    ROUND(s.max_tokens_share, 3) AS max_tokens_share,
    s.templates,
    ROUND(SAFE_DIVIDE(s.requests, s.templates), 1) AS requests_per_template,
    IF(s.single_turn_share >= 0.90, 1, 0)
      + IF(s.max_tokens_share >= 0.70, 1, 0)
      + IF(SAFE_DIVIDE(s.requests, s.templates) >= 100, 1, 0) AS measures_over,
    s.fast_mode_no_grant,
    IFNULL(pr.probe_hits, 0) AS probe_hits
  FROM shape AS s
  LEFT JOIN probe AS pr
    ON pr.org_id = s.org_id
  WHERE s.requests >= 2000
)
SELECT
  org_id,
  requests,
  single_turn_share,
  max_tokens_share,
  templates,
  requests_per_template,
  measures_over,
  fast_mode_no_grant,
  probe_hits
FROM scored
WHERE measures_over >= 2
ORDER BY measures_over DESC, requests DESC;
```

````spl
``` One pass over requests and probe events, merged by organization. fast_mode_no_grant and probe_hits are context and do not enter measures_over. ```
(index=claude_api sourcetype=api:request http_status=200) OR (index=safeguards sourcetype=classifier:event) earliest=-14d
    [ search index=access sourcetype=program:enrollment program="CVP" earliest=0 | fillnull value="(organization)" workspace_id | fillnull value="(none)" model_scope | stats latest(status) AS status BY org_id, workspace_id, tier, model_scope | stats count(eval(status="queued" OR status="in_review")) AS open_rows, count(eval(status="active")) AS active_rows BY org_id, tier | where open_rows > 0 AND active_rows = 0 | dedup org_id | fields org_id ]
| stats count(eval(sourcetype="api:request")) AS requests, count(eval(sourcetype="api:request" AND turn_index=1)) AS opening_turns, count(eval(sourcetype="api:request" AND output_tokens>=max_tokens)) AS saturated, dc(prompt_template_hash) AS templates, count(eval(sourcetype="api:request" AND fast_mode_16_80_mtok="true" AND isnull(cvp_tier) AND like(model_id, "claude-mythos%"))) AS fast_mode_no_grant, count(eval(sourcetype="classifier:event" AND distillation_probe_score>=0.80)) AS probe_hits BY org_id
| where requests >= 2000
| eval measures_over=if(opening_turns / requests >= 0.90, 1, 0) + if(saturated / requests >= 0.70, 1, 0) + if(requests / templates >= 100, 1, 0)
| where measures_over >= 2
| eval single_turn_share=round(opening_turns / requests, 3), max_tokens_share=round(saturated / requests, 3), requests_per_template=round(requests / templates, 1)
| table org_id, requests, single_turn_share, max_tokens_share, templates, requests_per_template, measures_over, fast_mode_no_grant, probe_hits
| sort - measures_over, - requests
````

### DET-03: Enrolled zero-retention workspace falling back from Mythos

Closes: GAP-2. Purpose: Finds workspaces with an active Cyber Verification Program enrollment, in a zero-retention organization, whose Mythos requests fall back for retention reasons: an eligible customer whose exemption has not reached the model it asked for. Shows the model that answered in its place (model_id), the exemption on file, the state of the notice and rate limiting in the same hour, so the specialist sees a retry storm before the customer reports an outage.

Routing: Runs every 5 minutes. Safeguards Account Access queue, one alert per workspace, within 15 minutes of the first fallback. Copy the account team. The alert carries the verification order from the GAP-2 checklist.

Tuning and false positives: Starting value: 20 retention fallbacks in an hour. A fallback with this reason already means the exemption on file does not list the requested model, so no separate exemption test is needed. Suppress when the customer has opted in to 30-day retention. The rate-limit count is context for the notice, not an alert condition. The Splunk version expects two lookups refreshed every 15 minutes. cvp_active_workspaces (key organization and workspace, output enrolled) is built from the latest enrollment row per organization, workspace, tier and model scope, kept when its status is active, with an organization-level row expanded to every workspace of the organization. retention_state_by_workspace (key organization and workspace; outputs zdr_enabled, retention_exemption and notice_status) is built from the latest compliance row per organization and workspace.

```sql
-- Enrolled workspaces in zero-retention organizations whose Mythos requests fell back
-- for retention reasons in the last hour, with the exemption and the notice on file.
-- compliance_state and program_enrollments are versioned: read the latest row.
WITH enrolled AS (
  SELECT DISTINCT org_id, workspace_id
  FROM (
    SELECT org_id, workspace_id, program, status
    FROM `access_prod.program_enrollments`
    QUALIFY ROW_NUMBER() OVER (PARTITION BY org_id, workspace_id, tier, model_scope ORDER BY enrolled_ts DESC) = 1
  )
  WHERE program = 'CVP'
    AND status = 'active'
),
state AS (
  SELECT org_id, workspace_id, zdr_enabled, retention_exemption, notice_status
  FROM `org_prod.compliance_state`
  QUALIFY ROW_NUMBER() OVER (PARTITION BY org_id, workspace_id ORDER BY updated_ts DESC) = 1
),
req AS (
  SELECT
    a.org_id,
    a.workspace_id,
    a.request_ts,
    a.http_status,
    a.fallback_reason,
    a.model_id
  FROM `safeguards_prod.api_requests` AS a
  WHERE a.request_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 1 HOUR)
    AND STARTS_WITH(a.requested_model, 'claude-mythos')
    -- An organization-level enrollment row has a null workspace and covers every workspace.
    -- EXISTS keeps one row per request when both kinds of row match.
    AND EXISTS (
      SELECT 1
      FROM enrolled AS e
      WHERE e.org_id = a.org_id
        AND (e.workspace_id = a.workspace_id OR e.workspace_id IS NULL)
    )
)
SELECT
  r.org_id,
  r.workspace_id,
  COUNT(*) AS mythos_requests,
  COUNTIF(r.fallback_reason = 'retention_not_enabled') AS retention_fallbacks,
  COUNTIF(r.http_status = 429) AS rate_limited,
  MIN(IF(r.fallback_reason = 'retention_not_enabled', r.request_ts, NULL)) AS first_fallback_ts,
  MAX(IF(r.fallback_reason = 'retention_not_enabled', r.model_id, NULL)) AS answering_model,
  IFNULL(s.retention_exemption, 'none') AS retention_exemption,
  IFNULL(s.notice_status, 'none') AS notice_status
FROM req AS r
JOIN state AS s
  ON s.org_id = r.org_id
 AND s.workspace_id = r.workspace_id
WHERE s.zdr_enabled = TRUE
GROUP BY r.org_id, r.workspace_id, s.retention_exemption, s.notice_status
HAVING COUNTIF(r.fallback_reason = 'retention_not_enabled') >= 20
ORDER BY retention_fallbacks DESC;
```

```spl
index=claude_api sourcetype=api:request requested_model="claude-mythos*" earliest=-60m
| lookup cvp_active_workspaces org_id, workspace_id OUTPUT enrolled
| where enrolled="true"
| lookup retention_state_by_workspace org_id, workspace_id OUTPUT zdr_enabled, retention_exemption, notice_status
| where zdr_enabled="true"
| fillnull value="none" retention_exemption, notice_status
| stats count AS mythos_requests, count(eval(fallback_reason="retention_not_enabled")) AS retention_fallbacks, count(eval(http_status=429)) AS rate_limited, min(eval(if(fallback_reason="retention_not_enabled", _time, null()))) AS first_fallback_ts, max(eval(if(fallback_reason="retention_not_enabled", model_id, null()))) AS answering_model BY org_id, workspace_id, retention_exemption, notice_status
| where retention_fallbacks >= 20
| eval first_fallback_ts=strftime(first_fallback_ts, "%Y-%m-%d %H:%M:%S")
| table org_id, workspace_id, mythos_requests, retention_fallbacks, rate_limited, first_fallback_ts, answering_model, retention_exemption, notice_status
| sort - retention_fallbacks
```

### DET-04: Life sciences demand on a BAA organization

Closes: GAP-2. Purpose: Finds organizations set up under a BAA (baa_org_flag) with no life sciences enrollment whose Fable traffic (model_id) meets the biology safeguard repeatedly, and shows their agent runs for the week. This is a likely program candidate that the BAA rule will block, found before the customer files an appeal, so the account team can start the organization split.

Routing: Runs hourly. Account team and LSVP intake: a weekly digest, plus an immediate note when the count passes its starting value. This is a service signal about a customer who needs a path, not an abuse signal. Word the alert that way.

Tuning and false positives: Starting value: 50 biology safeguard events in 24 hours, counted on Fable events only (model_id begins claude-fable): Mythos is reached through a program, so a customer on it already has a path. Exclude organizations with an open life sciences case. A run of events from one misconfigured pipeline can pass the value in minutes, so read the agent columns before contacting the customer. The Splunk version expects two hourly lookups. compliance_state_by_org (key organization; outputs baa_org_flag and plan) is built from the latest compliance row of each workspace: baa_org_flag is true when the latest row of any workspace of the organization says so, as in the SQL, and plan is read from one of those rows. lsvp_enrolled_orgs (key organization, output enrolled) lists organizations whose latest life sciences row, per organization, workspace, tier and model scope, is active, queued or in review.

```sql
-- BAA-enabled organizations without a life sciences enrollment whose traffic met the
-- biology safeguard 50 or more times in 24 hours, with their agent runs for the week.
-- compliance_state is versioned: an organization counts as BAA-enabled when the latest
-- row of any of its workspaces says so.
WITH state AS (
  SELECT org_id, workspace_id, baa_org_flag, plan
  FROM `org_prod.compliance_state`
  QUALIFY ROW_NUMBER() OVER (PARTITION BY org_id, workspace_id ORDER BY updated_ts DESC) = 1
),
baa AS (
  SELECT org_id, ANY_VALUE(plan) AS plan
  FROM state
  WHERE baa_org_flag = TRUE
  GROUP BY org_id
),
bio AS (
  SELECT
    e.org_id,
    COUNT(*) AS biology_events,
    COUNTIF(e.action = 'intervene') AS intervened,
    COUNTIF(e.action = 'fallback') AS fell_back
  FROM `safeguards_prod.classifier_events` AS e
  JOIN baa AS b
    ON b.org_id = e.org_id
  WHERE e.classifier_family = 'biology'
    AND STARTS_WITH(e.model_id, 'claude-fable')
    AND e.action IN ('intervene', 'fallback')
    AND e.event_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 24 HOUR)
  GROUP BY e.org_id
),
runs AS (
  SELECT
    org_id,
    COUNT(*) AS agent_runs_7d,
    COUNTIF(human_checkpoint_count = 0) AS runs_without_checkpoint,
    MAX(worker_count) AS peak_workers
  FROM `agents_prod.runs`
  WHERE ended_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 7 DAY)
  GROUP BY org_id
),
enrolled AS (
  SELECT DISTINCT org_id
  FROM (
    SELECT org_id, program, status
    FROM `access_prod.program_enrollments`
    QUALIFY ROW_NUMBER() OVER (PARTITION BY org_id, workspace_id, tier, model_scope ORDER BY enrolled_ts DESC) = 1
  )
  WHERE program = 'LSVP'
    AND status IN ('active', 'queued', 'in_review')
)
SELECT
  bio.org_id,
  b.plan,
  bio.biology_events,
  bio.intervened,
  bio.fell_back,
  IFNULL(r.agent_runs_7d, 0) AS agent_runs_7d,
  IFNULL(r.runs_without_checkpoint, 0) AS runs_without_checkpoint,
  IFNULL(r.peak_workers, 0) AS peak_workers
FROM bio
JOIN baa AS b
  ON b.org_id = bio.org_id
LEFT JOIN runs AS r
  ON r.org_id = bio.org_id
LEFT JOIN enrolled AS n
  ON n.org_id = bio.org_id
WHERE bio.biology_events >= 50
  AND n.org_id IS NULL
ORDER BY bio.biology_events DESC;
```

````spl
``` One pass over both sources, merged by organization, so no join row limit applies. An agent:run event is written when the run ends. ```
(index=safeguards sourcetype=classifier:event classifier_family="biology" model_id="claude-fable*" action IN ("intervene", "fallback") earliest=-24h) OR (index=agents sourcetype=agent:run earliest=-7d)
| eval is_run=if(sourcetype="agent:run", 1, 0)
| stats count(eval(sourcetype="classifier:event")) AS biology_events, count(eval(action="intervene")) AS intervened, count(eval(action="fallback")) AS fell_back, sum(is_run) AS agent_runs_7d, count(eval(is_run=1 AND human_checkpoint_count=0)) AS runs_without_checkpoint, max(worker_count) AS peak_workers BY org_id
| where biology_events >= 50
| lookup compliance_state_by_org org_id OUTPUT baa_org_flag, plan
| where baa_org_flag="true"
| lookup lsvp_enrolled_orgs org_id OUTPUT enrolled
| where isnull(enrolled)
| fillnull value=0 peak_workers
| table org_id, plan, biology_events, intervened, fell_back, agent_runs_7d, runs_without_checkpoint, peak_workers
| sort - biology_events
````

### DET-05: Seat takeover sequence: failed sign-ins, new network, new token, limit reset, burst

Closes: GAP-3. Purpose: Chains five steps on one seat inside two hours: a run of failed sign-ins, a successful sign-in from a network the organization has not used in 30 days, a new OAuth grant, a limit reset, and a request burst. The first new-network sign-in is one step; the query counts how many of the other four surround it.

Routing: Runs every 15 minutes. One rule: page the on-call Safeguards specialist at five steps, or at three or more when the organization holds a program grant; otherwise open a ticket in the account security queue. The alert carries the first-hour steps from the GAP-3 checklist: lock the seat, end sessions, revoke tokens, then notify.

Tuning and false positives: Starting values: 5 or more failed sign-ins before the first new-network success, and 200 or more requests after it. Travel and a new VPN exit match single steps, so the sequence is the condition. A sign-in without MFA from a hosting network weighs more than one with MFA from a residential network: the query returns all three fields for that reason. The known-network set must end two hours before now, or the sign-in under test makes its own network known and the alert suppresses itself. In production, read the request step from an accelerated data model, not raw events.

```sql
-- Seats with a first successful sign-in from a network unseen for the organization in
-- 30 days, scored on the steps that came before and after it in the last two hours.
-- known_asn stops two hours ago, so the sign-in under test cannot make itself known.
WITH window_auth AS (
  SELECT org_id, seat_id, event_ts, event_type, asn, ip_type, mfa_used
  FROM `identity_prod.auth_events`
  WHERE event_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 2 HOUR)
),
known_asn AS (
  SELECT DISTINCT org_id, asn
  FROM `identity_prod.auth_events`
  WHERE event_type = 'login_success'
    AND event_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 30 DAY)
    AND event_ts <  TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 2 HOUR)
),
new_login AS (
  SELECT a.org_id, a.seat_id, a.event_ts AS login_ts, a.asn, a.ip_type, a.mfa_used
  FROM window_auth AS a
  LEFT JOIN known_asn AS k
    ON k.org_id = a.org_id
   AND k.asn = a.asn
  WHERE a.event_type = 'login_success'
    AND k.asn IS NULL
  QUALIFY ROW_NUMBER() OVER (PARTITION BY a.org_id, a.seat_id ORDER BY a.event_ts) = 1
),
failed AS (
  SELECT f.org_id, f.seat_id, COUNT(*) AS failed_before
  FROM window_auth AS f
  JOIN new_login AS l
    ON l.org_id = f.org_id
   AND l.seat_id = f.seat_id
  WHERE f.event_type = 'login_failed'
    AND f.event_ts < l.login_ts
  GROUP BY f.org_id, f.seat_id
),
grants AS (
  SELECT g.org_id, g.seat_id, MIN(g.event_ts) AS grant_ts
  FROM window_auth AS g
  JOIN new_login AS l
    ON l.org_id = g.org_id
   AND l.seat_id = g.seat_id
  WHERE g.event_type = 'oauth_grant_created'
    AND g.event_ts >= l.login_ts
  GROUP BY g.org_id, g.seat_id
),
resets AS (
  SELECT r.org_id, r.seat_id, COUNT(*) AS resets_redeemed
  FROM `safeguards_prod.limit_reset_events` AS r
  JOIN new_login AS l
    ON l.org_id = r.org_id
   AND l.seat_id = r.seat_id
  WHERE r.reset_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 2 HOUR)
    AND r.reset_ts >= l.login_ts
  GROUP BY r.org_id, r.seat_id
),
burst AS (
  SELECT q.org_id, q.seat_id, COUNT(*) AS requests_after_login
  FROM `safeguards_prod.api_requests` AS q
  JOIN new_login AS l
    ON l.org_id = q.org_id
   AND l.seat_id = q.seat_id
  WHERE q.request_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 2 HOUR)
    AND q.request_ts >= l.login_ts
  GROUP BY q.org_id, q.seat_id
),
programs AS (
  SELECT org_id, STRING_AGG(DISTINCT program, ', ') AS active_programs
  FROM (
    SELECT org_id, program, status
    FROM `access_prod.program_enrollments`
    QUALIFY ROW_NUMBER() OVER (PARTITION BY org_id, workspace_id, tier, model_scope ORDER BY enrolled_ts DESC) = 1
  )
  WHERE status = 'active'
  GROUP BY org_id
),
scored AS (
  SELECT
    l.org_id,
    l.seat_id,
    l.login_ts,
    l.asn,
    l.ip_type,
    l.mfa_used,
    IFNULL(f.failed_before, 0) AS failed_before,
    g.grant_ts,
    IFNULL(r.resets_redeemed, 0) AS resets_redeemed,
    IFNULL(b.requests_after_login, 0) AS requests_after_login,
    IFNULL(p.active_programs, 'none') AS active_programs,
    1
      + IF(IFNULL(f.failed_before, 0) >= 5, 1, 0)
      + IF(g.grant_ts IS NOT NULL, 1, 0)
      + IF(IFNULL(r.resets_redeemed, 0) >= 1, 1, 0)
      + IF(IFNULL(b.requests_after_login, 0) >= 200, 1, 0) AS steps_matched
  FROM new_login AS l
  LEFT JOIN failed AS f
    ON f.org_id = l.org_id AND f.seat_id = l.seat_id
  LEFT JOIN grants AS g
    ON g.org_id = l.org_id AND g.seat_id = l.seat_id
  LEFT JOIN resets AS r
    ON r.org_id = l.org_id AND r.seat_id = l.seat_id
  LEFT JOIN burst AS b
    ON b.org_id = l.org_id AND b.seat_id = l.seat_id
  LEFT JOIN programs AS p
    ON p.org_id = l.org_id
)
SELECT
  org_id,
  seat_id,
  login_ts,
  asn,
  ip_type,
  mfa_used,
  failed_before,
  grant_ts,
  resets_redeemed,
  requests_after_login,
  active_programs,
  steps_matched
FROM scored
WHERE steps_matched >= 3
ORDER BY steps_matched DESC, requests_after_login DESC;
```

````spl
``` Expects the lookup org_known_asn_30d (key organization and ASN, output known): every successful sign-in between 30 days and 2 hours ago. Build it with latest=-2h so the sign-in under test cannot make its own network known. Also expects the lookup active_programs_by_org (key organization; outputs active_programs, has_lsvp, has_cvp), built from the latest enrollment row per organization, workspace, tier and model scope, kept when its status is active. ```
(index=identity sourcetype=auth:event event_type IN ("login_failed", "login_success", "oauth_grant_created")) OR (index=safeguards sourcetype=limit:reset) OR (index=claude_api sourcetype=api:request) earliest=-2h
| lookup org_known_asn_30d org_id, asn OUTPUT known
| eval step=case(sourcetype="auth:event" AND event_type="login_failed", "failed", sourcetype="auth:event" AND event_type="login_success" AND isnull(known), "new_login", sourcetype="auth:event" AND event_type="oauth_grant_created", "grant", sourcetype="limit:reset", "reset", sourcetype="api:request", "request")
| where isnotnull(step)
| eventstats min(eval(if(step="new_login", _time, null()))) AS login_time BY org_id, seat_id
| where isnotnull(login_time)
| stats count(eval(step="failed" AND _time < login_time)) AS failed_before, min(eval(if(step="grant" AND _time >= login_time, _time, null()))) AS grant_time, count(eval(step="reset" AND _time >= login_time)) AS resets_redeemed, count(eval(step="request" AND _time >= login_time)) AS requests_after_login, first(login_time) AS login_time, first(eval(if(step="new_login" AND _time=login_time, asn, null()))) AS asn, first(eval(if(step="new_login" AND _time=login_time, ip_type, null()))) AS ip_type, first(eval(if(step="new_login" AND _time=login_time, mfa_used, null()))) AS mfa_used BY org_id, seat_id
| eval steps_matched=1 + if(failed_before>=5, 1, 0) + if(isnotnull(grant_time), 1, 0) + if(resets_redeemed>=1, 1, 0) + if(requests_after_login>=200, 1, 0)
| where steps_matched >= 3
| lookup active_programs_by_org org_id OUTPUT active_programs
| fillnull value="none" active_programs
| eval login_ts=strftime(login_time, "%Y-%m-%d %H:%M:%S"), grant_ts=strftime(grant_time, "%Y-%m-%d %H:%M:%S")
| table org_id, seat_id, login_ts, asn, ip_type, mfa_used, failed_before, grant_ts, resets_redeemed, requests_after_login, active_programs, steps_matched
| sort - steps_matched, - requests_after_login
````

### DET-06: Program seat acting outside its program

Closes: GAP-3. Purpose: Finds a seat in an organization that holds only a life sciences grant meeting the cyber safeguard, or a seat under a cyber-only grant meeting the biology safeguard, when that seat met no such intervention in the 60 days before. A sudden change of subject on a trusted seat is the earliest sign that someone else is using it.

Routing: Runs every 15 minutes, one alert per seat per day. A page to the on-call Safeguards specialist, joined to any open DET-05 alert on the same seat. It replaces the weekly scope review as the first response for this pattern.

Tuning and false positives: Starting value: 20 interventions in any one hour of the last 24, with no intervention of that family on the seat in the 60 days before those 24 hours. History counts interventions, not every logged evaluation, because ordinary traffic is evaluated all the time. A lab that starts a legitimate security project will match once: one confirmation from the organization owner clears it and records the new scope. Organizations that hold both grants are excluded.

```sql
-- Seats under a single-program grant that met the other program's safeguard 20 or more
-- times in one hour of the last 24, with no such intervention in the 60 days before.
WITH grants AS (
  SELECT
    org_id,
    LOGICAL_OR(program = 'LSVP') AS has_lsvp,
    LOGICAL_OR(program = 'CVP') AS has_cvp
  FROM (
    SELECT org_id, program, status
    FROM `access_prod.program_enrollments`
    QUALIFY ROW_NUMBER() OVER (PARTITION BY org_id, workspace_id, tier, model_scope ORDER BY enrolled_ts DESC) = 1
  )
  WHERE status = 'active'
  GROUP BY org_id
),
hourly AS (
  SELECT
    org_id,
    seat_id,
    classifier_family,
    TIMESTAMP_TRUNC(event_ts, HOUR) AS hour_start,
    COUNTIF(action IN ('intervene', 'fallback')) AS interventions
  FROM `safeguards_prod.classifier_events`
  WHERE event_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 24 HOUR)
    AND classifier_family IN ('cyber', 'biology')
  GROUP BY org_id, seat_id, classifier_family, hour_start
),
recent AS (
  SELECT
    org_id,
    seat_id,
    classifier_family,
    MAX(interventions) AS peak_interventions_per_hour,
    SUM(interventions) AS interventions_24h,
    MIN(IF(interventions > 0, hour_start, NULL)) AS first_hour
  FROM hourly
  GROUP BY org_id, seat_id, classifier_family
),
history AS (
  SELECT
    org_id,
    seat_id,
    classifier_family,
    COUNTIF(action IN ('intervene', 'fallback')) AS interventions_prior_60d
  FROM `safeguards_prod.classifier_events`
  WHERE event_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 60 DAY)
    AND event_ts <  TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 24 HOUR)
    AND classifier_family IN ('cyber', 'biology')
  GROUP BY org_id, seat_id, classifier_family
)
SELECT
  r.org_id,
  r.seat_id,
  r.classifier_family AS off_program_family,
  IF(g.has_lsvp, 'LSVP', 'CVP') AS held_program,
  r.peak_interventions_per_hour,
  r.interventions_24h,
  IFNULL(h.interventions_prior_60d, 0) AS interventions_prior_60d,
  r.first_hour
FROM recent AS r
JOIN grants AS g
  ON g.org_id = r.org_id
LEFT JOIN history AS h
  ON h.org_id = r.org_id
 AND h.seat_id = r.seat_id
 AND h.classifier_family = r.classifier_family
WHERE ((g.has_lsvp AND NOT g.has_cvp AND r.classifier_family = 'cyber')
    OR (g.has_cvp AND NOT g.has_lsvp AND r.classifier_family = 'biology'))
  AND r.peak_interventions_per_hour >= 20
  AND IFNULL(h.interventions_prior_60d, 0) = 0
ORDER BY r.peak_interventions_per_hour DESC;
```

````spl
``` Expects the lookup active_programs_by_org (key organization; outputs active_programs, has_lsvp, has_cvp; the last two are "true" or "false"), built from the latest enrollment row per organization, workspace, tier and model scope, kept when its status is active. ```
index=safeguards sourcetype=classifier:event classifier_family IN ("cyber", "biology") earliest=-60d
| lookup active_programs_by_org org_id OUTPUT has_lsvp, has_cvp
| fillnull value="false" has_lsvp, has_cvp
| where (has_lsvp="true" AND has_cvp="false" AND classifier_family="cyber") OR (has_cvp="true" AND has_lsvp="false" AND classifier_family="biology")
| eval hit=if(action="intervene" OR action="fallback", 1, 0)
| eval recent=if(_time >= relative_time(now(), "-24h"), 1, 0)
| eval hour_start=if(recent=1, relative_time(_time, "@h"), 0)
| stats sum(hit) AS interventions BY org_id, seat_id, classifier_family, recent, hour_start
| stats max(eval(if(recent=1, interventions, 0))) AS peak_interventions_per_hour, sum(eval(if(recent=1, interventions, 0))) AS interventions_24h, sum(eval(if(recent=0, interventions, 0))) AS interventions_prior_60d, min(eval(if(recent=1 AND interventions>0, hour_start, null()))) AS first_hour BY org_id, seat_id, classifier_family
| where peak_interventions_per_hour >= 20 AND interventions_prior_60d = 0
| eval held_program=if(classifier_family="cyber", "LSVP", "CVP")
| eval first_hour=strftime(first_hour, "%Y-%m-%d %H:%M")
| rename classifier_family AS off_program_family
| table org_id, seat_id, off_program_family, held_program, peak_interventions_per_hour, interventions_24h, interventions_prior_60d, first_hour
| sort - peak_interventions_per_hour
````

### DET-07: Credential fan-out: one credential, many devices or many agent workers

Closes: GAP-3. Purpose: Finds a single key or token used from many devices, or from many addresses with several devices or many sign-ins (the shape of a token on one shared workstation), or an API key in an organization whose agent runs peak at 50 workers or more, or an API key in an organization with a run whose tool calls matched the sandbox-escape evaluation set (sandbox_escape_eval_flag), or a credential used in a Red Team or Specialized Access workspace (cvp_tier) that never expires or expires after more than 12 hours (credential_ttl_hours; CVP-SEC-RT writes 12 and no static keys), in organizations that hold or have applied for a program grant. It separates a shared credential, which is a hygiene finding with a deadline, from a takeover, and it catches both before a grant attaches to a credential nobody owns.

Routing: Runs daily. Safeguards Account Access queue as a finding on the organization, with a seven-day fix. It becomes a blocker on any pending grant. It is not a page: a shared credential with a stable subject and known networks is not an incident. An expiry finding on a Red Team or Specialized Access workspace asks the customer for a credential system that issues credentials expiring within 12 hours.

Tuning and false positives: Starting values over 60 days: 5 or more devices; or 10 or more addresses together with 3 or more devices; or 10 or more addresses together with 20 or more sign-ins, which is what a token on one shared workstation looks like (GK-4533: 187 sign-ins and 15 request addresses in 60 days); or an API key in an organization with a run of 50 or more workers in the last seven days. An organization that has asked for a grant through its account team and has no enrollment row yet, as in GK-4489, is outside this query until an application is filed. Addresses alone never fire: one person who roams between home, office and mobile networks, or an autoscaled service behind many egress addresses, passes ten addresses on one device. The sign-in leg does fire on a single automated workload that signs in again from many addresses, and on one person who signs in daily from changing networks. It measures how often a credential signs in, not how many people use it: confirm the number of users before treating a hit as sharing. Until 15 Dec 2026 a key held by one workload is allowed for a Defense Access member (CVP-SEC-CREDS), so a hit on such a key is not a finding by itself; for the same reason the expiry leg reads only Red Team and Specialized Access workspaces, where static keys are not permitted and a credential must expire within 12 hours (CVP-SEC-RT). The 12 hours is the written limit and not a starting value, and one request from a credential with no expiry is enough to fire it. The sandbox leg starts at one flagged run in seven days: the flag means the tool calls matched an evaluation set, not that an escape was attempted, and a team that tests its own sandbox will match, so read the run before acting. This is one reason the detection opens a review item and never pages. Worker count is per organization in this schema; a per-credential count is the upgrade. The Splunk version expects two hourly lookups: peak agent workers per organization over seven days, and organizations with an active, queued or in-review enrollment.

```sql
-- Credentials used from many devices, or from many addresses with several devices or many
-- sign-ins, in 60 days, or API keys in organizations with large agent runs in the last
-- seven days. A token on one shared workstation shows one device and many sign-ins.
-- Two more findings: a credential used in a Red Team or Specialized Access workspace that never
-- expires or lives longer than 12 hours (credential_ttl_hours, CVP-SEC-RT), and an API key in an
-- organization with a run that matched the sandbox-escape evaluation set. Limited to organizations whose
-- latest enrollment row is active, queued or in review.
WITH use_60d AS (
  SELECT
    org_id,
    credential_id,
    ANY_VALUE(credential_type) AS credential_type,
    COUNT(DISTINCT client_ip) AS distinct_ips,
    COUNT(DISTINCT workspace_id) AS workspaces_reached,
    STRING_AGG(DISTINCT cvp_tier, ', ' ORDER BY cvp_tier) AS cvp_tiers,
    COUNTIF(cvp_tier IN ('red_team_access', 'specialized_access')) AS strict_tier_requests,
    MAX(credential_ttl_hours) AS longest_ttl_hours,
    COUNTIF(credential_ttl_hours IS NULL) AS requests_without_expiry
  FROM `safeguards_prod.api_requests`
  WHERE request_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 60 DAY)
    AND credential_id IS NOT NULL
  GROUP BY org_id, credential_id
),
devices AS (
  SELECT
    org_id,
    credential_id,
    COUNT(DISTINCT device_id) AS distinct_devices,
    COUNTIF(event_type = 'login_success') AS sign_ins
  FROM `identity_prod.auth_events`
  WHERE event_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 60 DAY)
    AND credential_id IS NOT NULL
  GROUP BY org_id, credential_id
),
swarm AS (
  SELECT
    org_id,
    MAX(worker_count) AS peak_workers_in_org,
    COUNTIF(sandbox_escape_eval_flag) AS runs_sandbox_flagged
  FROM `agents_prod.runs`
  WHERE ended_ts >= TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL 7 DAY)
  GROUP BY org_id
),
programs AS (
  SELECT org_id, STRING_AGG(DISTINCT CONCAT(program, ':', status), ', ') AS programs
  FROM (
    SELECT org_id, program, status
    FROM `access_prod.program_enrollments`
    QUALIFY ROW_NUMBER() OVER (PARTITION BY org_id, workspace_id, tier, model_scope ORDER BY enrolled_ts DESC) = 1
  )
  WHERE status IN ('active', 'queued', 'in_review')
  GROUP BY org_id
)
SELECT
  u.org_id,
  u.credential_id,
  u.credential_type,
  u.distinct_ips,
  IFNULL(d.distinct_devices, 0) AS distinct_devices,
  IFNULL(d.sign_ins, 0) AS sign_ins,
  u.workspaces_reached,
  IFNULL(s.peak_workers_in_org, 0) AS peak_workers_in_org,
  IFNULL(s.runs_sandbox_flagged, 0) AS runs_sandbox_flagged,
  u.cvp_tiers,
  u.longest_ttl_hours,
  u.requests_without_expiry,
  p.programs
FROM use_60d AS u
JOIN programs AS p
  ON p.org_id = u.org_id
LEFT JOIN devices AS d
  ON d.org_id = u.org_id
 AND d.credential_id = u.credential_id
LEFT JOIN swarm AS s
  ON s.org_id = u.org_id
WHERE IFNULL(d.distinct_devices, 0) >= 5
   OR (u.distinct_ips >= 10 AND IFNULL(d.distinct_devices, 0) >= 3)
   OR (u.distinct_ips >= 10 AND IFNULL(d.sign_ins, 0) >= 20)
   OR (u.credential_type = 'api_key' AND IFNULL(s.peak_workers_in_org, 0) >= 50)
   OR (u.credential_type = 'api_key' AND IFNULL(s.runs_sandbox_flagged, 0) >= 1)
   OR (u.strict_tier_requests > 0 AND (u.requests_without_expiry > 0 OR u.longest_ttl_hours > 12))
ORDER BY distinct_devices DESC, u.distinct_ips DESC;
```

````spl
``` One pass over requests, sign-ins and the agent runs that matched the sandbox-escape evaluation set, merged by credential, so no join row limit applies. The flagged runs of the last seven days are counted per organization with eventstats and then dropped. Expects the lookups agent_peak_workers_7d_by_org (key organization, output peak_workers_in_org) and program_state_by_org (key organization, output programs: the program and status of each latest enrollment row, per organization, workspace, tier and model scope, that is active, queued or in review). ```
(index=claude_api sourcetype=api:request credential_id=*) OR (index=identity sourcetype=auth:event credential_id=*) OR (index=agents sourcetype=agent:run sandbox_escape_eval_flag="true") earliest=-60d
| eventstats count(eval(sourcetype="agent:run" AND _time >= relative_time(now(), "-7d"))) AS runs_sandbox_flagged BY org_id
| where sourcetype!="agent:run"
| stats max(runs_sandbox_flagged) AS runs_sandbox_flagged, dc(eval(if(sourcetype="api:request", client_ip, null()))) AS distinct_ips, dc(eval(if(sourcetype="auth:event", device_id, null()))) AS distinct_devices, count(eval(sourcetype="auth:event" AND event_type="login_success")) AS sign_ins, dc(eval(if(sourcetype="api:request", workspace_id, null()))) AS workspaces_reached, first(credential_type) AS credential_type, count(eval(sourcetype="api:request")) AS requests, values(eval(if(sourcetype="api:request", cvp_tier, null()))) AS cvp_tiers, count(eval(sourcetype="api:request" AND (cvp_tier="red_team_access" OR cvp_tier="specialized_access"))) AS strict_tier_requests, max(eval(if(sourcetype="api:request", credential_ttl_hours, null()))) AS longest_ttl_hours, count(eval(sourcetype="api:request" AND isnull(credential_ttl_hours))) AS requests_without_expiry BY org_id, credential_id
| where requests > 0
| lookup program_state_by_org org_id OUTPUT programs
| where isnotnull(programs)
| lookup agent_peak_workers_7d_by_org org_id OUTPUT peak_workers_in_org
| fillnull value=0 distinct_devices, peak_workers_in_org, runs_sandbox_flagged
| where distinct_devices >= 5 OR (distinct_ips >= 10 AND distinct_devices >= 3) OR (distinct_ips >= 10 AND sign_ins >= 20) OR (credential_type="api_key" AND peak_workers_in_org >= 50) OR (credential_type="api_key" AND runs_sandbox_flagged >= 1) OR (strict_tier_requests > 0 AND (requests_without_expiry > 0 OR longest_ttl_hours > 12))
| eval cvp_tiers=mvjoin(cvp_tiers, ", ")
| table org_id, credential_id, credential_type, distinct_ips, distinct_devices, sign_ins, workspaces_reached, peak_workers_in_org, runs_sandbox_flagged, cvp_tiers, longest_ttl_hours, requests_without_expiry, programs
| sort - distinct_devices, - distinct_ips
````

### DET-08: Cyber grant over its approved-user cap

Closes: GAP-3. Purpose: Finds an active Red Team Access grant with more than 75 approved users, or an active Specialized Access grant with more than 25 (seat_count_over_25), the caps the program pages write (CVP-RT-ELIG, CVP-SPEC, CVP-SEC-RT). The page says Red Team and Specialized Access switch off when the organization exceeds the tier's seat limit (CVP-SCOPE), so the account team can narrow the grant or take the written seat request before the customer meets the switch-off in the middle of work.

Routing: Runs daily. Safeguards Account Access queue, as a finding on the organization, with the cyber tier (cvp_tier) and the number of users over the cap. It is not a page and not an enforcement action: the cap is written, and the page asks for more seats in writing. The finding asks the customer to narrow the approved users or to send the written request.

Tuning and false positives: Both numbers are the written caps, 75 and 25, and not starting values. Workload identities do not count toward them, so confirm that approved_user_count leaves them out before any alert routes to a person. seat_count_over_25 is true for every Red Team grant of 26 to 75 users, which is allowed, so the query reads it for Specialized Access rows only. A grant is read from the latest row per organization, workspace, tier and model scope, so a decline or a withdrawal after an over-cap row clears it. On a Team plan a grant covers the whole organization (CVP-SCOPE), so the seat count of the organization is the upgrade; this version reads the approved users on the grant.

```sql
-- Active Red Team or Specialized Access grants whose approved users are over the written cap:
-- 75 for Red Team Access, 25 for Specialized Access. seat_count_over_25 is true when
-- approved_user_count is over 25, which is the Specialized cap and is also true for a Red Team
-- grant of 26 to 75 users, so it is read for Specialized rows only. program_enrollments is
-- versioned and small: the latest row per grant is read with no time bound, as in DET-01.
WITH latest AS (
  SELECT org_id, workspace_id, model_scope, cvp_tier, approved_user_count, seat_count_over_25, status
  FROM `access_prod.program_enrollments`
  WHERE program = 'CVP'
  QUALIFY ROW_NUMBER() OVER (PARTITION BY org_id, workspace_id, cvp_tier, model_scope ORDER BY enrolled_ts DESC) = 1
)
SELECT
  org_id,
  IFNULL(workspace_id, '(organization)') AS workspace_id,
  IFNULL(model_scope, '(none)') AS model_scope,
  cvp_tier,
  approved_user_count,
  IF(cvp_tier = 'red_team_access', 75, 25) AS tier_cap,
  approved_user_count - IF(cvp_tier = 'red_team_access', 75, 25) AS users_over_cap,
  seat_count_over_25
FROM latest
WHERE status = 'active'
  AND ((cvp_tier = 'specialized_access' AND IFNULL(seat_count_over_25, FALSE))
    OR (cvp_tier = 'red_team_access' AND approved_user_count > 75))
ORDER BY users_over_cap DESC;
```

```spl
index=access sourcetype=program:enrollment program="CVP" cvp_tier IN ("red_team_access", "specialized_access") earliest=0
| fillnull value="(organization)" workspace_id
| fillnull value="(none)" model_scope
| stats latest(status) AS status, latest(approved_user_count) AS approved_user_count, latest(seat_count_over_25) AS seat_count_over_25 BY org_id, workspace_id, model_scope, cvp_tier
| where status="active"
| where (cvp_tier="specialized_access" AND seat_count_over_25="true") OR (cvp_tier="red_team_access" AND approved_user_count > 75)
| eval tier_cap=if(cvp_tier="red_team_access", 75, 25), users_over_cap=approved_user_count - tier_cap
| table org_id, workspace_id, model_scope, cvp_tier, approved_user_count, tier_cap, users_over_cap, seat_count_over_25
| sort - users_over_cap
```

## 5. What held up

- The Red Team evidence rows did their job: a 19-day-old registration with no firm credential fails on the page, without any signal.
- The cyber safeguard stayed on under a life sciences grant, as the announcement says it does: every one of the 96 Mythos requests an intruder sent through a verified lab's grant was stopped.
- Fable kept its biology safeguards for a pipeline with no grant: 236 events on the protein-design swarm since launch. The control did its job; the customer needed a path, not an exception.
- The route for the water utility was already written: Defense Access while a Red Team application is reviewed. The fix is an owner and a clock, not a new rule.
- The BAA rule and the retention exemption are sound as policy. Both teams qualified; what was missing was the procedure that applies each rule.
- A decline, a hold and a containment notice can each state the decision and the next step without naming a signal. Every generated message in this workbench passes the detection-detail lint.

## 6. Decisions needed

| Owner | Ask | By |
|---|---|---|
| Safeguards Engineering | Apply existing retention exemptions to Mythos 5.2 for every eligible enrolled workspace, and re-send each bounced notice to the program security contact (GAP-2). | Thu 12 Nov 2026 |
| Safeguards Policy | Approve the interim-tier procedure: a linkage precondition, positive evidence, a named owner and the two-day clock, with a one-business-day lane for dated deadlines (GAP-1). | Fri 13 Nov 2026 |
| Safeguards Engineering | Route DET-05 and DET-06 to the on-call page, with the first-hour containment steps in the alert body (GAP-3). | Fri 13 Nov 2026 |
| CVP intake | Add the linkage check to intake at every tier, and attach the reapply wait and the decline reason to the linked cluster (GAP-1). | Mon 16 Nov 2026 |
| Investigations | Report on payment cluster BC-0447 (13 active organizations) and on the three sibling Red Team applications. | Tue 17 Nov 2026 |
| Sales operations, with Legal and Privacy | Own the BAA organization split: a five-business-day target, the attestation text and the identity boundary check (GAP-2). | Wed 18 Nov 2026 |
| Safeguards Engineering, with Identity | Enforce phishing-resistant MFA at the seat for every life sciences, Red Team and Specialized grant now, and for Defense Access from 15 Dec 2026, starting with Team organizations, where a grant covers every seat (GAP-3). | Fri 20 Nov 2026 |

## Appendix A. Queries exercised during triage

- GK-4471, Token velocity: The traffic is one-shot, templated and maximum-length. The window holds 83,920 requests in 8 days, 96.0% of them single-turn, 88.0% saturated at max_tokens and spread over 212 templates.
- GK-4471, Payment and enforcement linkage: Enforcement suspended 37 of the 50 organizations on payment cluster BC-0447 under KF-0921 for coordinated output extraction. The applicant's two organizations are among the other 13, first seen since 19 Oct.
- GK-4489, Classifier interventions: The swarm has met the biology safeguard on Fable 236 times since launch: 163 intervene and 73 fallback. 220 of the 236 fell on de novo binder design, and run_fs_0426 met 9 with that stage off.
- GK-4489, Compliance state and PHI boundary: A BAA has been in force since 14 Mar 2026 on a HIPAA-ready Enterprise plan. The workspace clinical-ops holds PHI at 0 retention days. The key cred_fs_main has reached comp-design with 78,410 requests and clinical-ops with 26 requests. Both swarm keys are static, with no expiry.
- GK-4502, Classifier interventions: 32 of 200 evaluated Fable requests met the cyber safeguard (16.0%), 23 fallback and 9 intervene, across three OT seats on Tue 10 Nov, 14:00 to 20:00 PT. Seats rephrased after 9.4% of events, against 8.3% after a normal response.
- GK-4502, Program enrollment and application state: The Red Team application entered the queue on 9 Nov and still has no reviewer. The utility and both maintainers have no Defense Access enrollment, although CVP-PENDING and CVP-INTERIM write a route for an application under review. Nobody applied that route. The Red Team review target is Mon 23 Nov, nine days after the window opens, and reviews are currently taking longer.
- GK-4517, Token velocity: Mythos 5.2 served none of 231,800 requests since 10:20 on 9 Nov. Fable 5.2 answered 137,610 of them, and the service refused 94,190 with HTTP 429. By the retry rule, playbook retries make up 61.0% of requests and 58.0% of 429s, an upper bound. The other 90,380 requests are first calls, about 2,100 an hour against 1,100 before, as the live investigation runs more playbooks.
- GK-4517, Retention and enrollment state: The zero retention addendum took effect on 3 Feb 2025. Defense Access is active on cfc-ir with scope up to Mythos 5.1, and the Mythos 5.2 row has the status queued. The exemption on file lists claude-fable-* and claude-mythos-5-1, not Mythos 5.2. The 9 Nov notice bounced. The other 3 workspaces hold zero retention and no enrollment. The BAA organization flag is false, so the organization is not under a BAA.
- GK-4533, IP and ASN shifts: Seat gsr-14 sent 2,008 requests from AS64511 from 02:58, a hosting network that the organization had never seen. The previous 60 days came from campus only. The Enterprise organization shows no traffic from AS64511. Nothing ran on gsr-14 from 04:08 to 05:30.
- GK-4533, Auth events and credential lineage: Seat gsr-14 shows 14 failed password sign-ins from 02:31 to 02:46, a success at 02:47 without MFA and a new OAuth token at 02:49. All of it came from AS64511. Seat svc-pipeline shows one credential, one campus network and 187 sign-ins from 15 addresses, with no failures.

## Appendix B. Decision records

### GK-4471-D1

```text
DECISION RECORD GK-4471-D1
Simulation record: synthetic case, no real customer, account or decision.
Case:             GK-4471 | Quillmere Security LLC
Program:          CVP | Red Team Access
Verdict:          DENY | Decline and refer to Investigations
Reviewer:         specialist-01
Decided:          12 Nov 2026 03:04:04 UTC
Handle time:      8s
Written criteria: CVP-RT-ELIG, CVP-RT-EVID, CVP-USE, CVP-INTERIM, CVP-REAPPLY, MOD-01, MOD-02, DESK-LINK, DESK-COMMS

BASIS
The smaller-firm route (CVP-RT-EVID) needs a registration at least one year old, public
service information, two certified testers and a recent statement of work, report or client
reference. The applicant shows none of these and none of the four firm credentials, and its
registration is 19 days old, so it fails the written evidence rows on its own. Its stated
work, testing for clients, also needs a separate external-use approval (CVP-USE).
Separately, the payment instrument sits in a cluster where 37 organizations were suspended
by 17 September for coordinated output extraction, and the traffic has the same one-shot,
templated, maximum-length shape. Defense Access is no answer: nothing shows defensive work
on the applicant's own systems, and DESK-LINK (desk rule) rules out approval at any tier
from this queue. So the desk declines on the written criteria, refers the linkage to
Investigations and tells the applicant what the criteria need.

EVIDENCE CITED
- [KYR] Legal entity: The state registry shows a Delaware LLC filed on 23 Oct 2026, 19 days ago. Its registered agent shares one address with several hundred entities. The smaller-firm route to Red Team Access needs a registration at least one year old (CVP-RT-EVID).
- [KYR] Engagement evidence: The application supplies no evidence. It shows no firm credential: no CVE Numbering Authority listing, no FIRST membership, no CVE credit and no testing accreditation (CVP-RT-EVID). It shows none of the smaller-firm items either: no certified testers, no statement of work, test report or client reference. The message cites an NDA to explain why it shares no contracts.
- [KYR] Payment instrument: The applicant pays with a virtual prepaid card in payment cluster BC-0447. Billing and enforcement records link BC-0447 to enforcement cluster KF-0921, and enforcement suspended the 37 organizations of KF-0921 by 17 September 2026.
- [BILLING] Payment instrument sits in a cluster under enforcement
- [TELEMETRY] Request shape is bulk collection, not testing
- [TELEMETRY] Limit resets redeemed by script, across the cluster

TELEMETRY REVIEWED
- Token velocity: The traffic is one-shot, templated and maximum-length. The window holds 83,920 requests in 8 days, 96.0% of them single-turn, 88.0% saturated at max_tokens and spread over 212 templates.
- Payment and enforcement linkage: Enforcement suspended 37 of the 50 organizations on payment cluster BC-0447 under KF-0921 for coordinated output extraction. The applicant's two organizations are among the other 13, first seen since 19 Oct.

ACTIONS AND CONDITIONS
1. The desk declined Red Team Access on CVP-RT-EVID. The programs grant Mythos 5.2 (MOD-01), and Mythos fast mode is only for organizations in them (MOD-02), so the request for fast mode on Mythos 5.2 closes with the decline. The rate-limit request closes as a desk action, and the organization keeps generally available models (CVP-REAPPLY).
2. The notice states the firm route of CVP-RT-EVID. The route needs one of four, in the firm's own name: a CVE Numbering Authority listing, full FIRST membership, a recent CVE credit, or a testing accreditation such as CREST.
3. The notice states the smaller-firm route of CVP-RT-EVID. A smaller firm shows a registration at least one year old, which this LLC reaches on 23 Oct 2027. It also shows public information about its testing services and at least two testers with offensive security certifications. It shows a redacted statement of work, test report or client reference from the last 12 months as well.
4. The notice states that client work needs a separate external-use approval (CVP-USE).
5. The desk opened a cluster referral under DESK-LINK, the desk linkage rule. The referral covers BC-0447, which has 13 active organizations and links to KF-0921, and the evidence pack holds payment linkage, reset times, request shape and network spread.

FOLLOW-UPS
- Investigations: Payment cluster BC-0447 has 13 active organizations, and 52 of their seats redeemed the limit reset within 236 seconds after the offer opened. Review the cluster and decide on action.
- CVP intake: Hold the three other Red Team applications from the same payment cluster until Investigations reports, and check whether any of the 13 organizations holds or has applied for Defense Access.
- Safeguards Policy: GAP-1: the written criteria ask no linkage question at intake. Add a linkage check to intake at every tier. Make the reapply wait and the decline reason follow the linked cluster, and give Defense Access granted during a Red Team review a positive-evidence test.

POLICY CHECKS
- PASS CVP-RT-EVID: no firm credential, and the registration is 19 days old against one year, so the smaller-firm route fails its first test
- PASS CVP-USE: testing for clients is external use, which needs its own approval after program approval
- PASS DESK-LINK (desk rule): the card sits in a cluster under enforcement, so the case goes to referral and not to approval
- PASS CVP-REAPPLY and DESK-COMMS: the notice states what the program needs and the reapply rule, and names no signal
- PASS Required telemetry reviewed: Token velocity
- PASS Required telemetry reviewed: Payment and enforcement linkage
- PASS Evidence cited: 6
- PASS Messages name no detection method, signal or count

SPECIALIST NOTE
The auto-triage walkthrough made this decision in demo mode. A reviewer did not make it.
```

### GK-4489-D1

```text
DECISION RECORD GK-4489-D1
Simulation record: synthetic case, no real customer, account or decision.
Case:             GK-4489 | Lumen Fold Therapeutics
Program:          LSVP | Standard Use
Verdict:          CONDITIONAL | Approve Standard Use on a new non-BAA organization, with conditions
Reviewer:         specialist-01
Decided:          12 Nov 2026 03:04:16 UTC
Handle time:      8s
Written criteria: LSVP-BAA, LSVP-RET, LSVP-GRANT, LSVP-REQ, LSVP-SWITCH, LSVP-TYPES, LSVP-MODELS, LSVP-MONITOR, LSVP-THREATS, MOD-01, RET-01, DESK-AGENT, DESK-COMMS, DESK-RECORD

BASIS
A Series B company, a contact whose ORCID record and papers match, a biosafety registration
and a screened synthesis vendor show that Lumen Fold is a verified lab. 220 of the 236
biology safeguard events on Fable since launch fell on de novo binder design, so the need is
real. The checks rule out the network and the limit reset offer as causes. LSVP-BAA bars a
grant on a BAA organization and names the way through, a separate organization that is not
BAA-enabled, so the obstacle is the account and not the lab. LSVP-RET retains program usage
for 30 days while clinical-ops runs at 0 retention days, so the grant cannot sit beside that
workspace. Three of five runs had no human checkpoint, the longest ran 31 h 12 m at 180
workers, and the drafting tool can prepare a vendor order alone. The two shared keys fall
short of LSVP-REQ, and cred_fs_main reaches comp-design and clinical-ops, so the desk writes
these risks as conditions (LSVP-THREATS). Access can then be live ahead of the 1 Dec
milestone, and whether Standard Use covers de novo binder design is for LSVP intake to
confirm (LSVP-TYPES).

EVIDENCE CITED
- [KYR] Business Associate Agreement: A BAA has been in force on org_3b8e52c1 since 14 Mar 2026 (Enterprise, HIPAA-ready), and an organization set up under a BAA cannot receive a grant, so this one cannot.
- [KYR] Agent swarm: The swarm foldswarm made five runs in seven days, at up to 180 workers, and the longest ran 31 h 12 m. Three of the five had no human checkpoint, and three of the four since launch aborted. No run matched the sandbox-escape evaluation set.
- [COMPLIANCE] One key reaches the swarm and the health-data workspace
- [AGENTS] The drafting tool can prepare a vendor order with no person in the loop
- [OSINT] Verified lab with a real need
- [TELEMETRY] Safeguard events sit on the stage the lab says is blocked

TELEMETRY REVIEWED
- Classifier interventions: The swarm has met the biology safeguard on Fable 236 times since launch: 163 intervene and 73 fallback. 220 of the 236 fell on de novo binder design, and run_fs_0426 met 9 with that stage off.
- Compliance state and PHI boundary: A BAA has been in force since 14 Mar 2026 on a HIPAA-ready Enterprise plan. The workspace clinical-ops holds PHI at 0 retention days. The key cred_fs_main has reached comp-design with 78,410 requests and clinical-ops with 26 requests. Both swarm keys are static, with no expiry.

ACTIONS AND CONDITIONS
1. With the account team, the customer opens a new organization that is not BAA-enabled, and the grant takes effect there, while org_3b8e52c1 receives no grant (LSVP-BAA). The grant attaches to a custom role for the computational design team, up to 100 seats (LSVP-GRANT). The new organization has a dedicated program workspace, and every seat that uses the Claude apps has phishing-resistant MFA (LSVP-REQ). People who use Claude.ai start on the one preselected default grant, and the swarm chooses its grant natively on the API (LSVP-SWITCH).
2. The program help article puts work with protected health information out of scope (LSVP-BAA), so the desk asks for a signed attestation that no such information enters the new organization. It is a desk control, due Mon 16 Nov 2026, and enrollment of the new organization waits for it.
3. API access in the new organization uses Workload Identity Federation, with one identity per workload and no stored API key shared across workers (LSVP-REQ). The customer does not carry cred_fs_main over, because it also reached clinical-ops. No identity may reach org_3b8e52c1, a condition of this approval that keeps the new organization clear of the BAA exclusion (LSVP-BAA).
4. Agent misuse is a named threat model (LSVP-THREATS) and the pages write no guardrail, so these are desk conditions (DESK-AGENT). A person approves each vendor order the drafting tool prepares. Runs have a cap of 60 workers and 8 hours unless a person approves more, the shape of run_fs_0426, which completed with three checkpoints.
5. Fable keeps its biology safeguards under any grant (LSVP-MODELS, MOD-01), so the pipeline moves to Mythos 5.2 in the new organization, and the current organization stays on Fable.
6. The customer acknowledges 30-day retention of program usage in the new organization, and retention in the current organization stays as it is (LSVP-RET, RET-01).
7. Standard Use classifiers are more permissive than those of generally available models, but not absent (LSVP-TYPES). So LSVP intake confirms this week whether Standard Use covers de novo binder design or it needs the High-risk Use add-on. At launch, High-risk Use on Mythos stays limited to a small set of entities with additional vetting (LSVP-TYPES, LSVP-GRANT).

FOLLOW-UPS
- Account team: Open the new non-BAA organization with Imani Okafor's team, and collect the attestation, the seat list and the retention acknowledgement by Mon 16 Nov 2026.
- LSVP intake: Confirm by Fri 13 Nov 2026 whether Standard Use covers de novo binder design or it needs the High-risk Use add-on (LSVP-TYPES). At launch, High-risk Use on Mythos stays limited to a small set of entities with additional vetting. Enroll the new organization for Standard Use once the attestation is in. With the documents in on Mon 16 Nov, a decision typically comes by Thu 19 Nov (LSVP-REQ), so access can be live the week of 16 Nov 2026.
- Safeguards Engineering: Confirm that no identity or key from the new organization can reach org_3b8e52c1, and alert on any credential or seat that appears in both organizations.
- Legal and Privacy: Review the 26 requests that cred_fs_main sent to clinical-ops, the last on 5 Nov 2026 at 14:58 PT. Telemetry shows no content, so the customer decides whether it is a BAA matter on its side.
- Safeguards Policy: GAP-2 and GAP-3 inputs: write the path out of the BAA exclusion with an owner and a schedule to open the new organization. Add a control that keeps health data out of the new organization, and a credential-scope rule for agent swarms.
- Trust and Safety operations: Review the new organization after its first seven days (LSVP-REQ). Check for a dedicated program workspace and phishing-resistant MFA on the seats that use the Claude apps. Check for Workload Identity Federation with one identity per workload, and for run caps and the approval step.

POLICY CHECKS
- PASS LSVP-BAA: an organization set up under a BAA cannot receive a grant, so the grant goes on a new organization that is not BAA-enabled, where the exclusion does not apply
- PASS LSVP-RET: 30-day retention applies to program usage in the new organization only, so the health-data workspace stays where it is
- PASS LSVP-GRANT and LSVP-MODELS: the grant gives Standard Use to up to 100 seats, and Fable keeps its biology safeguards under any grant
- PASS LSVP-THREATS and LSVP-MONITOR: agent misuse is a named threat model, so the desk writes conditions that keep activity inside the scope the lab stated
- PASS LSVP-REQ: the new organization gets a dedicated program workspace, phishing-resistant MFA on every seat that uses the Claude apps, and Workload Identity Federation for API access
- PASS LSVP-TYPES: Standard Use classifiers are more permissive than those of generally available models, but not absent, so the notice leaves binder design coverage to LSVP intake. The notice does not imply that binder design runs freely
- PASS DESK-COMMS: the notice gives the decision, the steps and the date, and it names no signal
- PASS Required telemetry reviewed: Classifier interventions
- PASS Required telemetry reviewed: Compliance state and PHI boundary
- PASS Evidence cited: 6
- PASS Messages name no detection method, signal or count

SPECIALIST NOTE
The auto-triage walkthrough made this decision in demo mode. A reviewer did not make it.
```

### GK-4502-D1

```text
DECISION RECORD GK-4502-D1
Simulation record: synthetic case, no real customer, account or decision.
Case:             GK-4502 | Cedar Hollow Regional Water Authority
Program:          CVP | Defense Access (applied for Red Team Access)
Verdict:          APPROVE | Defense Access now, Red Team application left open
Reviewer:         specialist-01
Decided:          12 Nov 2026 03:04:28 UTC
Handle time:      8s
Written criteria: CVP-DEF-ELIG, CVP-DEF-WHO, CVP-PENDING, CVP-INTERIM, CVP-USE, CVP-SCOPE, CVP-DEF-TIME, CVP-RT-ELIG, CVP-BLOCK, CVP-SEC-INCIDENT, CVP-SEC-CREDS, SEC-CLAUDE, DESK-COMMS

BASIS
The applicants asked for the tier the form named, but the work is vulnerability validation,
detection work and patch verification on the utility's own controllers (CVP-DEF-ELIG). A
coordinated disclosure that is not done for a client counts as internal use (CVP-USE), and
the announcement names critical infrastructure operators of any size and open-source
maintainers (CVP-DEF-WHO). The written route enrolls a qualifying organization in Defense
Access while its Red Team application is reviewed, and the utility qualifies (CVP-PENDING,
CVP-INTERIM). The enrollment check shows no Defense Access row for the application as filed
on 9 Nov. Nothing triggers or owns that enrollment, and no faster lane exists for a dated
patch window. On a Team plan access covers the whole organization, all 12 seats (CVP-SCOPE),
so the record names the three OT security users who do the work. Telemetry shows
human-paced, multi-turn analysis and no sign of probing, so the one real risk is physical:
46 controllers run treatment plants, and CVP-BLOCK blocks physical-world damage at every
tier. The utility starts today on the isolated bench only, without the maintainers, whose
own Defense Access review target of Fri 13 Nov is a target and not a promise.

EVIDENCE CITED
- [KYR] Open-source maintainers: Sofia Lindgren and Tomasz Baran maintain the PLC runtime openladder-rt, with six years of signed releases on the public code host. Both are named in the project's security policy as contacts for vulnerability reports.
- [KYR] Coordinated disclosure: The vendor was told on 4 Nov 2026, and the embargo lifts on Tue 24 Nov. The vendor has a draft patch. The utility must verify it before its window on Sat 14 and Sun 15 Nov.
- [ACCOUNT] Patch window opens before a Red Team decision is likely
- [INBOUND] Applied for the tier the form wording suggested
- [TELEMETRY] Cyber safeguard met on 32 requests in six hours
- [INBOUND] The subject matter is physical plant equipment

TELEMETRY REVIEWED
- Classifier interventions: 32 of 200 evaluated Fable requests met the cyber safeguard (16.0%), 23 fallback and 9 intervene, across three OT seats on Tue 10 Nov, 14:00 to 20:00 PT. Seats rephrased after 9.4% of events, against 8.3% after a normal response.
- Program enrollment and application state: The Red Team application entered the queue on 9 Nov and still has no reviewer. The utility and both maintainers have no Defense Access enrollment, although CVP-PENDING and CVP-INTERIM write a route for an application under review. Nobody applied that route. The Red Team review target is Mon 23 Nov, nine days after the window opens, and reviews are currently taking longer.

ACTIONS AND CONDITIONS
1. Defense Access enabled for the Cedar Hollow Team organization under CVP-PENDING and CVP-INTERIM. On a Team plan the access covers all 12 seats (CVP-SCOPE). This record names the three OT security users who do the work: seat_ch_02, seat_ch_05 and seat_ch_08. The utility confirms the bench work stays with those three. Each signs in as themselves with MFA on now and moves to phishing-resistant MFA by 15 Dec 2026 (CVP-SEC-CREDS).
2. Individual Defense Access for Sofia Lindgren and Tomasz Baran fast-tracked and linked to GK-4502. The review target is Fri 13 Nov 2026, a target and not a promise (CVP-DEF-ELIG, CVP-DEF-WHO, CVP-DEF-TIME).
3. The grant covers flaw confirmation, detection work and patch verification on the isolated AQ-17 test bench only. Live-plant testing is outside the grant. Physical-world damage is blocked at every tier (CVP-BLOCK). The customer also confirms that findings stay private until the vendor's embargo lifts on Tue 24 Nov 2026. That part is a desk condition with no written clause. The nearest is CVP-BLOCK.
4. The customer names a security contact and acknowledges the incident duties. The customer reports a suspected breach or misuse within 72 hours and a security incident within 24 hours (CVP-SEC-INCIDENT).
5. The Red Team application stays open. The desk withdraws it if the customer confirms that Defense Access covers the work (CVP-PENDING, CVP-INTERIM).
6. The utility is on a Team plan. Claude Security is for Claude Enterprise customers and needs no Cyber Verification Program access (SEC-CLAUDE). So the notice names it to the customer as the path to scan the openladder-rt runtime code. This is information about a path and not an offer of access today.

FOLLOW-UPS
- CVP intake: Fast-track the Defense Access applications from Sofia Lindgren and Tomasz Baran as individuals, and link both to GK-4502. Aim to review them by Fri 13 Nov 2026 (CVP-DEF-TIME).
- CVP intake: On Mon 16 Nov 2026, decide on the Red Team application. Withdraw it if the customer confirms that Defense Access covers the work, and otherwise leave it in the queue.
- Account team: By Thu 12 Nov 2026, confirm that the security contact and the incident-duty acknowledgement are on file. Hold the check-in with the customer on Mon 16 Nov.
- Trust and Safety operations: On Mon 16 Nov 2026, review cyber safeguard activity on the utility's organization and the two maintainers' accounts. Compare it with the bench-only scope and the three named OT security users, and report anything outside it to CVP intake.
- Safeguards Policy: GAP-1: nobody applied the written route (CVP-PENDING, CVP-INTERIM) to the application filed on 9 Nov. Give the interim Defense Access enrollment a trigger and an owner when a Red Team application arrives. Add an urgency lane for a dated patch window. Describe how individual maintainers who work with an organization get routed and linked.

POLICY CHECKS
- PASS The utility is a critical infrastructure operator on a paid plan and does vulnerability validation and detection engineering, so it qualifies for Defense Access (CVP-DEF-ELIG).
- PASS Each maintainer holds an individual paid plan, and the announcement names open-source maintainers (CVP-DEF-WHO). So each qualifies for Defense Access, and an individual's access covers only that person (CVP-DEF-ELIG).
- PASS The utility qualifies, so the written route enrolls it in Defense Access while its Red Team application is reviewed (CVP-PENDING, CVP-INTERIM). Nobody applied that route to the application filed on 9 Nov.
- PASS The work is internal use, because it runs on the utility's own controllers and is a coordinated disclosure that is not done for a client (CVP-USE).
- PASS On a Team plan access covers the whole organization, so it is enabled for all 12 seats and the decision record names the three users who do the work (CVP-SCOPE).
- PASS Physical-world damage stays blocked at every tier, and the grant is tied to an isolated bench (CVP-BLOCK).
- PASS Three conditions come with the grant: a security contact, sign-in by each user as themselves with MFA now (phishing-resistant from 15 Dec 2026), and the incident duties (CVP-SEC-INCIDENT, CVP-SEC-CREDS).
- PASS Claude Enterprise customers can use Claude Security to scan the runtime code without being in the Cyber Verification Program (SEC-CLAUDE). The utility is on a Team plan, so the notice names it as a path and does not offer it today.
- PASS The notice gives the decision, the scope and the dates, and it names no signal (DESK-COMMS).
- PASS Required telemetry reviewed: Classifier interventions
- PASS Required telemetry reviewed: Program enrollment and application state
- PASS Evidence cited: 6
- PASS Messages name no detection method, signal or count

SPECIALIST NOTE
The auto-triage walkthrough made this decision in demo mode. A reviewer did not make it.
```

### GK-4517-D1

```text
DECISION RECORD GK-4517-D1
Simulation record: synthetic case, no real customer, account or decision.
Case:             GK-4517 | Harborline Financial Group
Program:          CVP | Defense Access, retention exemption
Verdict:          CONDITIONAL | Confirm eligibility and extend the retention exemption to Mythos 5.2 on cfc-ir
Reviewer:         specialist-01
Decided:          12 Nov 2026 03:04:40 UTC
Handle time:      8s
Written criteria: RET-02, RET-03, RET-04, CVP-ZDR, CVP-EVAL, CVP-SCOPE, CVP-DEF-ELIG, CVP-SEC-CREDS, RET-BEDROCK, RET-ZDR-EFS, DESK-SCOPE, DESK-COMMS, DESK-RECORD, DESK-COND

BASIS
The records show a zero retention addendum from 3 Feb 2025, an exemption on file for cfc-ir,
and Defense Access there since 18 Aug 2026 for incident response (CVP-DEF-ELIG). An eligible
program customer with zero data retention keeps it for Mythos 5.2 (RET-02), and an exemption
holder has zero retention on all program models, for internal use (CVP-ZDR). Harborline
meets both, yet the exemption lists Fable and Mythos 5.1 but not Mythos 5.2, because a
launch eligibility pass, a simulated desk process, did not reach it. So since 10:20 on 9 Nov
Fable 5.2 answers in place of Mythos 5.2, retries hit the rate limit, and the stricter
safeguards block live work. The desk extends the exemption to Mythos 5.2 on cfc-ir only, the
enrolled workspace (CVP-SCOPE), and assigns Mythos 5.2 there under the smallest-scope rule
(DESK-SCOPE). The static key and the retry loop become conditions, and the Amazon Bedrock
path stays separate because the customer sets its retention mode in its own AWS account
(RET-BEDROCK, RET-ZDR-EFS).

EVIDENCE CITED
- [KYR] Defense Access enrollment: The program records show CVP Defense Access approved on 18 Aug 2026 for the Cyber Fusion Center, on one workspace, cfc-ir. The status is active and the model scope runs up to Mythos 5.1. The Mythos 5.2 scope is a second row with status queued, so that row does not yet cover Mythos 5.2 requests.
- [KYR] Zero data retention: The zero data retention addendum took effect on 3 Feb 2025. The retention exemption on file for cfc-ir dates from 18 Aug 2026 and lists claude-fable-* and claude-mythos-5-1, not Mythos 5.2, so it does not yet cover Mythos 5.2. Enterprise Frontier Safeguards is compatible with zero retention (RET-03), but it is in private beta and not yet available to Harborline.
- [KYR] Notice to the organization: The notice log shows a notice of 9 Nov at 10:05 PT. It told Harborline that it keeps zero retention for Mythos 5.2 and that an admin assigns Mythos 5.2 to the workspace. The notice went to a billing contact who left in September, and it bounced, so nobody at Harborline saw it. No page gives a delivery method for a program notice, and the notice that the retention article describes concerns Fable with zero retention (RET-04).
- [TELEMETRY] Every Mythos 5.2 request from cfc-ir is answered by Fable 5.2
- [TELEMETRY] The SOAR playbook retries failed calls with no backoff

TELEMETRY REVIEWED
- Token velocity: Mythos 5.2 served none of 231,800 requests since 10:20 on 9 Nov. Fable 5.2 answered 137,610 of them, and the service refused 94,190 with HTTP 429. By the retry rule, playbook retries make up 61.0% of requests and 58.0% of 429s, an upper bound. The other 90,380 requests are first calls, about 2,100 an hour against 1,100 before, as the live investigation runs more playbooks.
- Retention and enrollment state: The zero retention addendum took effect on 3 Feb 2025. Defense Access is active on cfc-ir with scope up to Mythos 5.1, and the Mythos 5.2 row has the status queued. The exemption on file lists claude-fable-* and claude-mythos-5-1, not Mythos 5.2. The 9 Nov notice bounced. The other 3 workspaces hold zero retention and no enrollment. The BAA organization flag is false, so the organization is not under a BAA.

ACTIONS AND CONDITIONS
1. Eligibility rests on the zero retention addendum (3 Feb 2025), the exemption on file, Defense Access on cfc-ir (18 Aug 2026) and internal use. So the desk extends the exemption on cfc-ir to claude-mythos-5-2 (RET-02, CVP-ZDR) and assigns Mythos 5.2 to workspace cfc-ir in org_5e2f81b7, and to no other workspace. The smallest scope applies under the desk rule DESK-SCOPE (simulated).
2. The customer acknowledges that program use under the exemption is for internal use only (CVP-ZDR).
3. The launch announcement (RET-03) says only that Enterprise Frontier Safeguards is in private beta and that eligible customers keep zero retention before they implement it. It asks for no statement of intent, so this is a desk condition, simulated (DESK-COND): the customer records its intent to move to Enterprise Frontier Safeguards when it is available. It is the desk's request and not a published duty.
4. The customer replaces the notice contact with a named current owner by Fri 13 Nov 2026. The desk then re-sends the 9 Nov notice to that owner.
5. The customer adds backoff to the SOAR playbook and stops retries when the model that answers differs from the requested model. The customer confirms when the change is live, by Fri 13 Nov 2026.
6. The static key cred_soar_01 (created Aug 2026, never rotated) must rotate at least every seven days now and retire by 15 Dec 2026 (CVP-SEC-CREDS). A long-lived IAM user access key also signs the customer's Bedrock calls, but that key is a desk observation, not a program condition (DESK-COND, a simulated desk procedure). The CVP Security Requirements article bars IAM user access keys on Amazon Bedrock for Defense Access from 15 Dec 2026. A short-term Bedrock API key that expires within 12 hours or with the Bedrock session, whichever is shorter, is the exception. That rule would apply if the AWS account were linked to the program, and the case links none. So the desk records this observation for the file and does not send it to the customer.
7. Bedrock content stays inside AWS, so the desk saw only the customer's CloudTrail excerpt, where the calls fail under mode none set by a service control policy. The customer learns that on Bedrock the mode is set in its own AWS account (aws_review, on the account in us-east-1, where the calls run: RET-BEDROCK). The customer can ask its AWS account team about zero retention for internal use (RET-ZDR-EFS), and the desk changes neither. AWS evaluates zero retention per account and per model with the model provider, and gives it to customers eligible for Enterprise Frontier Safeguards through at least 30 June 2027. The calls are signed with a long-lived IAM user access key, a desk observation, not a program condition. The CVP Security Requirements article would bar it on Bedrock from 15 Dec 2026 if the AWS account were linked to the program (DESK-COND, a simulated desk procedure).

FOLLOW-UPS
- Safeguards Engineering: Extend the cfc-ir exemption to claude-mythos-5-2 (RET-02, CVP-ZDR). Assign Mythos 5.2 to cfc-ir today and confirm that Mythos 5.2 requests are served as asked. After that, check that request volume and HTTP 429 responses return to the pre-launch level.
- Safeguards Engineering: List every zero-retention CVP member whose requests fell back with reason retention_not_enabled since 9 Nov 10:00 PT, and every exemption that does not list Mythos 5.2. The same fix then reaches them.
- CVP intake: Activate the queued Mythos 5.2 enrollment row for cfc-ir, which this decision confirms (CVP-EVAL). The enrollment scope and the exemption then agree.
- Account team: Replace the notice contact on the account record and the zero retention addendum. Re-send the 9 Nov notice to the new owner. On Tue 15 Dec 2026, confirm that the customer retired cred_soar_01 (CVP-SEC-CREDS).
- Account team: Tell Dana that the Amazon Bedrock retention mode is set in her own AWS account and that she asks her AWS account team about any zero retention for internal use. This desk saw only the CloudTrail excerpt she sent, and it changes neither (RET-BEDROCK, RET-ZDR-EFS).
- Safeguards Policy: GAP-2: write down who applies an exemption to a new program model, who verifies it, what unit it attaches to and how the program delivers a notice that bounces. Stop launch-day fallback for members whose exemption does not yet list the new model.

POLICY CHECKS
- PASS The zero retention addendum took effect on 3 Feb 2025, so Harborline already has zero data retention (RET-02)
- PASS The exemption on file for cfc-ir lists Fable and Mythos 5.1, and it is the exemption that the program names for zero retention on program models (CVP-ZDR)
- PASS Defense Access is active on cfc-ir, the one workspace with an enrollment, and its Mythos 5.2 row has the status queued (RET-02, CVP-DEF-ELIG)
- PASS The use is internal to Harborline, and zero retention in the program is for internal use (CVP-ZDR)
- PASS The desk extends the exemption to cfc-ir only and assigns Mythos 5.2 to that workspace, because access applies to workspaces in Console and admins assign it (CVP-SCOPE, CVP-EVAL). The desk rule asks for the smallest scope (DESK-SCOPE)
- PASS The notice went to a billing contact who left in September, so it never reached Harborline. No page gives a delivery method for a program notice, and the notice in RET-04 concerns Fable with zero retention, so the customer does not opt in or wait
- PASS The static key and the retry loop are conditions and not grounds to refuse (CVP-SEC-CREDS)
- PASS The Amazon Bedrock question is a scope line: Bedrock needs the retention mode aws_review, and the customer sets that mode in its own AWS account (RET-BEDROCK). A customer eligible for Enterprise Frontier Safeguards can use zero retention for internal use through at least 30 June 2027, and it asks its AWS account team about eligibility (RET-ZDR-EFS). The desk changes neither
- PASS Both notices state the decision and the steps, and they name no detection detail (DESK-COMMS, DESK-RECORD)
- PASS Required telemetry reviewed: Token velocity
- PASS Required telemetry reviewed: Retention and enrollment state
- PASS Evidence cited: 5
- PASS Messages name no detection method, signal or count

SPECIALIST NOTE
The auto-triage walkthrough made this decision in demo mode. A reviewer did not make it.
```

### GK-4533-D1

```text
DECISION RECORD GK-4533-D1
Simulation record: synthetic case, no real customer, account or decision.
Case:             GK-4533 | Solvanger Lab, Ostrander University
Program:          LSVP | Standard Use, security alert
Verdict:          QUARANTINE | Quarantine seat gsr-14 and keep the lab running
Reviewer:         specialist-01
Decided:          12 Nov 2026 03:04:52 UTC
Handle time:      56s
Written criteria: DESK-SCOPE, LSVP-THREATS, LSVP-MONITOR, LSVP-REQ, LSVP-GRANT, LSVP-MODELS, LSVP-CYBER, CVP-SEC-INCIDENT, CVP-SEC-CREDS, CVP-SEC-SPEC, OFFER-RESET, DESK-REMEDY, DESK-CLOCK, DESK-XPROG, DESK-COND, DESK-COMMS, DESK-RECORD

BASIS
gsr-14 shows 14 failed password sign-ins from a hosting network new to the organization, a
success at 02:47 on a password alone and an OAuth token two minutes later. All three limit
resets go in 67 minutes, and 1,912 Fable and 96 Mythos 5.2 requests ask for vulnerability
rediscovery, a subject new to the seat in 60 days. The owner last signed in from campus at
18:40, and every step came from the hosting network, so the sequence is a takeover and the
lab is the victim. The shared token on svc-pipeline falls short of LSVP-REQ, but its
network, volume and subject did not move overnight, so it is hygiene and not part of the
incident. The seat is the smallest scope that contains the incident (DESK-SCOPE), and a live
token cannot wait for the week of LSVP-MONITOR, so the desk acts now. No page clearly binds
the university, so the desk asks its security contact to report in 24 hours and investigate
in 48 from this decision, as a request (DESK-XPROG, DESK-CLOCK).

EVIDENCE CITED
- [IDENTITY] Failed sign-ins, then a success, then a new long-lived token in 18 minutes
- [TELEMETRY] A hosting network the organization has never seen
- [TELEMETRY] All three limit resets spent in 67 minutes
- [TELEMETRY] Requests ask for vulnerability rediscovery, outside the grant
- [TELEMETRY] Nothing ties the university's Enterprise organization to the events

TELEMETRY REVIEWED
- IP and ASN shifts: Seat gsr-14 sent 2,008 requests from AS64511 from 02:58, a hosting network that the organization had never seen. The previous 60 days came from campus only. The Enterprise organization shows no traffic from AS64511. Nothing ran on gsr-14 from 04:08 to 05:30.
- Auth events and credential lineage: Seat gsr-14 shows 14 failed password sign-ins from 02:31 to 02:46, a success at 02:47 without MFA and a new OAuth token at 02:49. All of it came from AS64511. Seat svc-pipeline shows one credential, one campus network and 187 sign-ins from 15 addresses, with no failures.

ACTIONS AND CONDITIONS
1. The desk locks seat gsr-14, ends its sessions, revokes its OAuth grants and tokens and pauses its program access, for gsr-14 only. The other 13 seats, svc-pipeline among them, and the organization grant stay as they were (DESK-SCOPE). The desk restores the seat only after its owner re-verifies identity, resets the password and enrolls phishing-resistant MFA (LSVP-REQ).
2. The desk notifies Professor Solvanger, the organization owner, and Kofi Mensah, the Research Security Officer, within the hour of the containment decision. Kofi Mensah is the named security contact of the university's Defense Access grant. LSVP-THREATS and LSVP-MONITOR write the notice to the admin, and this decision sets the hour.
3. The owner did not make the redemptions at 02:51, 03:27 and 03:58 on 11 Nov 2026. A used reset cannot be undone under the offer (OFFER-RESET). So the desk restores three Fable limit resets on gsr-14 as a one-off exception, at its discretion (DESK-REMEDY, a simulated desk procedure, not a program rule).
4. Seat gsr-14 had no MFA, and the shared token on svc-pipeline is a hygiene finding and not part of the compromise. So the desk sets two conditions, both due Wed 18 Nov 2026 (LSVP-REQ). All 14 seats need phishing-resistant MFA. The shared token behind svc-pipeline moves to Workload Identity Federation for the pipeline or to individual sign-in. This decision sets the date.
5. The cyber program writes its 72-hour report for a breach or misuse involving the grant (CVP-SEC-INCIDENT). Its 24-hour and 48-hour duties carry no word on an incident in another organization, so no page clearly binds the university to this incident in the lab's organization. The university's Office of Information Security holds Defense Access on org_18f7b2e5, and Kofi Mensah is its named security contact. We ask him, as a request and not a program duty (DESK-XPROG), to report the incident within 24 hours and to investigate the abuse we identified within 48 hours. The cyber program's security page names no event that starts a clock, so the two requests run from this decision, which the record states (DESK-CLOCK, a simulated desk procedure). The lab's admin has one week from our out-of-scope notice, which this decision sends, to explain, narrow or dispute it (LSVP-MONITOR).
6. The cyber program's security page writes single sign-on for Specialized Access only, and the lab holds a life sciences grant, so no page asks for it here. The desk borrows it as a desk condition, simulated and not a program rule (DESK-COND). The lab's sign-ins move behind the university's federated single sign-on, and the Research Security Officer confirms the plan by Wed 18 Nov 2026. This decision sets the date.

FOLLOW-UPS
- Trust and Safety operations: Preserve the sign-in, request and grant records for gsr-14 from 02:31 to 04:08 on 11 Nov 2026, before the 30-day retention window closes. LSVP-RET sets that window for the 96 program requests. The plan's standard retention covers the Fable requests.
- Investigations: Check whether the network that reached gsr-14 (203.0.113.0/24) touched other organizations in the same period. Review the 688 Fable requests that the model answered.
- LSVP intake: Record the 11 Nov incident on the lab's grant file. Make no change to the grant.
- Safeguards Account Access: Write the time of this decision on the record as the start of the two desk requests. The university's security contact gets 24 hours to report and 48 hours to investigate, as desk requests (DESK-XPROG). The lab's admin gets 168 hours from the out-of-scope notice, which this decision sends, to answer it (LSVP-MONITOR). Tell the Research Security Officer which clock is which.
- Safeguards Policy: GAP-3: write a seat and credential response into the monitoring rule (contain at once, tell the admin, no one-week wait when a credential is under another party's control). Enforce the written MFA requirement (LSVP-REQ) at the seat after the program gives the grant. Write how to restore limit resets that a compromised seat spent.

POLICY CHECKS
- PASS One seat shows the takeover and nothing else does, and the Enterprise organization shows no related activity, so the seat is the smallest scope that contains it (DESK-SCOPE)
- PASS The grant belongs to the organization, so it stays with the other 13 seats. The desk pauses only gsr-14 (LSVP-GRANT)
- PASS The cyber safeguard stayed on under the grant and stopped every Mythos 5.2 request, so the desk need not withdraw program access to limit exposure (LSVP-CYBER)
- PASS LSVP-THREATS names access compromise as a threat model, and LSVP-MONITOR writes only an out-of-scope notice and a one-week window, so neither bars a lock on the seat now (LSVP-THREATS, LSVP-MONITOR). The desk tells the admin and the Research Security Officer within the hour
- PASS The program writes phishing-resistant MFA for the Claude apps and Workload Identity Federation for the API as requirements (LSVP-REQ). Seat gsr-14 had no MFA and svc-pipeline runs on a shared token, so the desk sets both as dated conditions
- PASS The cyber program writes its 72-hour report for a breach or misuse involving the grant (CVP-SEC-INCIDENT). Its 24-hour and 48-hour duties carry no word on an incident in another organization, so no page clearly binds the university. The desk asks its security contact to report in 24 hours and investigate in 48 from the decision, as a request (DESK-XPROG, DESK-CLOCK). The lab's admin has a week from our out-of-scope notice, which this decision sends, to answer (LSVP-MONITOR)
- PASS The cyber program writes the ban on shared sign-ins (CVP-SEC-CREDS) and Specialized Access alone writes single sign-on (CVP-SEC-SPEC), so neither binds the lab's life sciences grant. The desk sets both as conditions and not as rules (DESK-COND)
- PASS The customer notice gives the decision, what stays live and the next steps. It names no detection method (DESK-COMMS, DESK-RECORD)
- PASS Required telemetry reviewed: IP and ASN shifts
- PASS Required telemetry reviewed: Auth events and credential lineage
- PASS Evidence cited: 5
- PASS Messages name no detection method, signal or count

SPECIALIST NOTE
The auto-triage walkthrough made this decision in demo mode. A reviewer did not make it.
```

## Sources

Public program pages the written criteria are paraphrased from, as read on 11 November 2026:

- Claude Mythos 5.2 (model page): https://www.anthropic.com/claude/mythos
- Expanding the Cyber Verification Program (announcement): https://www.anthropic.com/news/cyber-verification-program
- Cyber Verification Program (help article): https://support.claude.com/en/articles/14604842-cyber-verification-program
- Cyber Verification Program Security Requirements (help article): https://support.claude.com/en/articles/17202708-cyber-verification-program-security-requirements
- Introducing the Life Sciences Verification Program (announcement): https://anthropic.com/news/life-sciences-verification-program
- Life Sciences Verification Program (help article): https://support.claude.com/en/articles/16975617
- Data retention practices for Mythos-class models (help article): https://support.claude.com/articles/15425996-data-retention-practices-for-mythos-class-models
- Claude Fable 5.2 launch offers (help article): https://support.claude.com/en/articles/17506494
- Introducing Claude Fable 5.2 and Claude Mythos 5.2 (announcement): https://www.anthropic.com/claude-fable-and-mythos-5-2
- Covered Models (help article): https://support.claude.com/en/articles/15425695-covered-models
- BAA coverage and Covered Models (help article): https://support.claude.com/en/articles/15455031
- Amazon Bedrock: data retention (AWS documentation): https://docs.aws.amazon.com/bedrock/latest/userguide/data-retention.html
- Amazon Bedrock: abuse detection (AWS documentation): https://docs.aws.amazon.com/bedrock/latest/userguide/abuse-detection.html
- Introducing Claude Fable 5.2 on AWS (AWS blog): https://aws.amazon.com/blogs/machine-learning/introducing-claude-fable-5-2-on-aws/

---

MADE BY MYTHOS 5.2. Compiled in the Mythos 5.2 Gatekeeper simulation workbench from the decisions recorded above.
