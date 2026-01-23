# SIP Status & Workflow

This document defines the statuses a SIP may have throughout its lifecycle and
summarizes the workflow for authors, reviewers, and contributors. Each SIP has
exactly **one** status at any given time.


A typical SIP progression:
```
Draft → Accepted → Recommended → Activation-In-Progress → Ratified (Final)
```

A SIP may transition into the following terminal states at any time:
- Rejected
- Withdrawn
- Superseded

All non-final SIPs remain permanently in the repository for historical
Reference.

## SIP Statuses

### Draft
The SIP is being written and refined. It may or may not yet have an assigned SIP
Number (provided by the SIP Editors CAB). Public feedback is encouraged, but formal evaluation by Consideration Advisory Boards (CABs) has not started.

### Accepted
SIP Editors have reviewed the document and confirmed that:
- It meets all SIP formatting and licensing requirements
- It represents a coherent and reviewable proposal

The SIP receives its official SIP number at this stage and becomes eligible for
CAB review.

### Recommended
_Note:_: A SIP must be **Accepted** before it becomes **Recommended**.

Relevant CABs have completed their subject-matter review and agree that the SIP:
- Is technically and/or procedurally sound  
- Should move proceed toward activation criteria  


### Activation-In-Progress
The Steering Committee CAB has approved the SIP for activation. However, some or all conditions in the SIP’s **Activation** section have not yet been met.

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
The SIP will not move forward in its current form.  
A rejected SIP remains in the repository for historical reference and may be
submitted again as a new Draft after major revision, but may not be reconsidered unless re-submitted. 

### Withdrawn
The author(s) have stopped work on the SIP.  
A withdrawn SIP cannot be revived as-is; it must receive a new SIP number if
re-submitted.

### Superseded
The SIP has been replaced by a newer SIP.  
The superseded SIP must include a `Superseded-By:` field, and the new SIP must
include `Replaces:`. This header shall be added by the SIP Editors CAB, and added to any ratified SIP as appropriate, following the contributing guidelines for merging a PR. 


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

Next, a pull request  is opened in the SIP repository with links to any discussions and a brief description in the pull request body. 

### 3. Early Review & SIP Number Assignment
SIP Editors ensure the draft is:
- Coherent and well scoped  
- Properly formatted and licensed  
- Suitable as a standalone proposal  

If approved, Editors shall:
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
- CAB chairs and SIP Editors update the **Sign-off** section  
- The SIP status is changed  to _Recommended_


If activation requires governance action:
- The Steering Committee reviews and votes  
- Upon approval, the SIP status shall be updated to _Activation-In-Progress_

## 6. Activation & Finalization
When all activation criteria are fulfilled:
- The SIP status shall be updated to _Ratified_
- Only errata may be added thereafter as an _Addendum_


# Summary for Contributors

To successfully advance a SIP, authors must:

- Write a clear, well-scoped and falsifiable proposal using the SIP template  
- Identify the correct SIP Type and Consideration(s)  
- Actively engage with both public and CAB feedback in good faith  
- Provide precise activation conditions  
- Expect iterative review before approval  



