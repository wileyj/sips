# SIP Status & Workflow

This document defines the statuses a SIP may have throughout its lifecycle and summarizes the workflow for authors, reviewers, and contributors. Each SIP has exactly **one** status at any given time.


## SIP Lifecycle

|Status	|What Happens	|Governing Vote|
|------------|--------------|---------|
| **Draft**	| SIP is open for early feedback, incomplete, or undergoing revisions.	| None |
| **Accepted**	| SIP Deputies confirm the SIP is well-formed, licensed, and ready for CAB review. The SIP receives its official number.	| None (Deputy consensus, not a vote)|
| **Recommended** | The relevant CAB(s) complete subject-matter review and vote to approve.	| CAB vote, per [procedure.md](procedure.md)|
| **Public Vote** (if required)	| For SIP types requiring one, a public/token-holder vote follows CAB approval. Status remains Recommended pending the outcome.	| Public vote, per [activation-voting.md](./activation-voting.md)|
| **Activation-In-Progress**	| The SIP awaits fulfillment of the criteria in its Activation section.	| None (monitoring only)|
| **Ratified**	| Once Activation-section criteria are met, the SC's certification vote confirms this.	| SC certification vote, per [steering_committee.md](steering_committee.md)|

A SIP may move to Rejected, Withdrawn, or Superseded at any point in this pipeline — see status definitions above. A failed CAB vote or public vote moves the SIP to Rejected rather than advancing it.


All non-final SIPs remain permanently in the repository for historical reference.


## SIP Statuses

### Draft
The SIP is being written and refined. It may or may not yet have an assigned SIP Number (provided by the SIP Deputies CAB). Public feedback is encouraged, but formal evaluation by Consideration Advisory Boards (CABs) has not started.

### Accepted
SIP Deputies have reviewed the document and confirmed that:
- It meets all SIP formatting and licensing requirements
- It represents a coherent and reviewable proposal

The SIP receives its official SIP number at this stage and becomes eligible for CAB review.

### Recommended
_Note_: A SIP must be **Accepted** before it becomes **Recommended**.

Relevant CABs have completed their subject-matter review and agree that the SIP:
- Is technically and/or procedurally sound
- Should proceed toward activation criteria


### Activation-In-Progress
_The Steering Committee CAB has approved the SIP for activation. However, some or all conditions in the SIP’s **Activation** section have not yet been met._

Examples include:
- Miner signaling thresholds
- Governance votes
- Activation at a specific block height
- Required infrastructure readiness

### Ratified (Final)
The SIP has met all activation criteria and is fully adopted.

Once Ratified:
- It becomes the authoritative specification
- Only non-substantive errata may be edited
- Substantive changes require a new SIP

### Rejected
_The SIP will not move forward in its current form._

A rejected SIP remains in the repository for historical reference and may be submitted again as a new Draft after major revision. 

### Withdrawn
_The author(s) have stopped work on the SIP._

A withdrawn SIP cannot be revived as-is; it must receive a new SIP number if
re-submitted.

### Superseded
_The SIP has been replaced by a newer SIP._

The superseded SIP must include a `Superseded-By:` field, and the new SIP must include `Replaces:`. This header shall be added by the SIP Deputies CAB, and added to any ratified SIP as appropriate, following the contributing guidelines for merging a PR. 

---

## SIP Workflow (Contributor Overview)

### 1. Idea Vetting
The author(s) publicly vet whether or not a proposal warrants a SIP.
Discussion helps determine:
- Novelty
- Scope
- Alignment with Stacks design and security goals
- Whether a simpler repo-level change is more appropriate

### 2. Drafting the SIP
The author prepares a SIP in Markdown using the official template and specifies:
- SIP Type
- Relevant Consideration(s)

Next, a pull request is opened in the SIP repository with links to any discussions and a brief description in the pull request body. 

### 3. Early Review & SIP Number Assignment
SIP Deputies ensure the draft is:
- Coherent and well scoped
- Properly formatted and licensed
- Suitable as a standalone proposal

If approved, Deputies shall:
- Assign a SIP number
- Set status to **Accepted**
- Merge the SIP
- Add it to the SIP index

_Authors **shall not** self-assign SIP numbers._

### 4. Public Review & CAB Evaluation
Once Accepted, the SIP:
- Enters a public comment period
- Undergoes various CAB review
- Accumulates formal feedback and revision requests

Expected timelines:
- Public comment window: ~2 weeks
- CAB review: 1-2 weeks depending on complexity
- Final comment resolution: ~1 week or more

Emergency SIPs may use accelerated processes.

### 5. Sign-off & Advancement
When CAB(s) approve the SIP:
- CAB chairs and SIP Deputies update the **Sign-off** section
- The SIP status is changed to _Recommended_

If the SIP's Type requires a public vote (see [activation-voting.md](./activation-voting.md)):
- The public vote is conducted per the requirements in [activation-voting.md](./activation-voting.md)
- Upon approval, the SIP status shall be updated to _Activation-In-Progress_

If no public vote is required for the SIP's Type, the SIP status is updated directly to Activation-In-Progress once Recommended.

### 6. Activation & Finalization
When all activation criteria are fulfilled:
- The SIP status shall be updated to _Ratified_
- Only errata may be added thereafter in a new trailing section as _Addendum_


# Summary for Contributors

To successfully advance a SIP, authors must:

- Write a clear, well-scoped and falsifiable proposal using the SIP template
- Identify the correct SIP Type and Consideration(s)
- Actively engage with both public and CAB feedback in good faith
- Provide precise activation conditions
- Expect iterative review before approval
