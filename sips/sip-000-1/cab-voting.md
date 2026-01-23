# CAB Voting & Ratification Clarity

To ensure transparency, predictability, and consistency across all SIPs, the following rules define what constitutes a valid vote, which version of a SIP may be voted on, and how proposals advance through the ratification pipeline.

These rules ensure that votes occur on stable, well-reviewed content; that changes during voting do not invalidate outcomes; and that the entire community can rely on a predictable, transparent pipeline from Draft to final ratification.


### Stable Text Requirement
    - All votes —CAB votes or public on-chain votes—must be held on a stable, review-complete 
      version of the SIP text.
    - No substantive changes may be made to a SIP once a vote has begun. Editorial corrections 
      (typos, formatting fixes) may be accepted only with CAB awareness and must not alter intent.

### Re-Vote Requirement
    - If the SIP’s intent, semantics, functional behavior, or implementation requirements change 
      after a vote has started, a re-vote is mandatory.
    - The determination of whether a change is “substantive” shall be made jointly by the 
      relevant CAB Chair and a SIP Editor.

### Defined Lifecycle Phases
    - SIPs must progress through the following standardized phases:
        1. **Draft** – SIP is open for early feedback, incomplete, or undergoing revisions.
        2. **Proposed** – SIP has undergone initial cleanup and is structurally complete.
        3. **CAB Review** – SIP is under active subject-matter review and comment resolution.
        4. **Public Vote (if applicable)** – Only after CAB approval and final sign-off.
        5. **Accepted / Rejected** – Determined by the vote outcome and activation rules.

### Minimum Timeline Requirements
    - To ensure sufficient review and prevent rushed governance:
        - **Draft Open Comment Period:** minimum **2 weeks**
        - **CAB Review Period:** minimum **1 week**
        - **Final Comment Resolution Period:** minimum **1 week**
    - Longer durations are strongly encouraged for complex or consensus-impacting proposals.

### Standardized Voting Procedure
    - All public votes must follow a documented, standardized procedure that includes:
        - minimum quorum thresholds  
        - required participation levels  
        - verification steps  
        - clear closing criteria  
    - Each SIP must link to the vote record and verification method.

### CAB Approval Prerequisite
    - A public or ecosystem-wide vote cannot begin until:
        - the relevant CAB(s) have formally approved the SIP for voting, **and**
        - all outstanding comments have been resolved.
    - CAB approvals must be documented via public minutes, GitHub comments, or a similar open venue.



## Caveats

### Post-CAB Vote SIP Updates

Once a CAB vote concludes, the SIP is considered approved in its voted form.

- Minor updates may still be made after the CAB vote and before merge under the following conditions:
    - The changes are editorial or implementation-detail only — i.e. they do not alter the SIP’s intent, semantics, or functional behavior as approved.
    - Any such change must be shared in the relevant CAB communication channel(s), and the diff must be visible in the PR for auditability.

- If any CAB member believes the change alters meaning, a CAB re-vote must be called.
- The CAB Chair should note such updates in the meeting Minutes and/or SIP PR discussion for record-keeping.

