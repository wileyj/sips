# SIP Committees

The act of deciding the status of a SIP is handled by a set of designated committees. These committees are composed of users who dedicate their time and expertise to curate the blockchain, ratifying SIPs on behalf of the rest of the ecosystem’s users.

There are two categories of committee in the SIP process: the **Steering Committee (SC)**,
and **Consideration Advisory Boards (CABs)**. CABs come in two kinds — subject-matter CABs
and the SIP Deputies CAB — described below.

### Steering Committee (SC)
- Select _Recommended_ status SIPs to be activated
- Determine whether or not a SIP has been activated and thus ratified
- Formally recognize [Consideration Advisory Boards](cab.md) 

### Consideration Advisory Boards (Subject-Matter CABs)
One per Consideration (Technical, Economic, Governance, Ethics, Diversity):
- Provide expert feedback on SIPs that have been moved to Accepted status in a timely manner - Transition SIPs to Recommended status if they have met the Board's consideration criteria, or set to a Rejected status otherwise. 

### SIP Deputies (the Deputies CAB)
A CAB responsible for the inbound funnel rather than subject-matter review. Unlike
subject-matter CABs, the Deputies CAB does not hold a formal vote to advance a SIP;
Deputies work by consensus to confirm formatting and numbering.
- Identify SIPs in the Draft status that can be transitioned to Accepted status. 
- Vet a SIP to ensure that it is well-formed, that it follows the ratification workflow faithfully
- Ensures that a proposal does not overlap with any already-Accepted SIPs or SIPs that have since become Recommended or Ratified.

### Committee Membership Limits
A user may serve on at most three (3) CABs concurrently, counting both subject-matter and
Deputies CAB membership toward that limit. An SC member may not normally serve concurrently
on any CAB (subject-matter or Deputies), absent a unanimous SC exception, per Steering
Committee Duties.

Any user may serve on a committee. However, all Stacks committee members must abide by the SIP Code of Conduct and must have a history of adhering to it. Failure to adhere to the Code of Conduct shall be grounds for immediate removal from a committee, with a potential prohibition against serving on any future committees.

---

## Committee Improvements

To strengthen accountability, transparency, and the effectiveness of the SIP review, the following standards apply to all Consideration Advisory Boards (CABs) and committee participants.

### Clear Review Workflow
- Each CAB must follow a consistent and publicly observable workflow when evaluating SIPs. This workflow may include GitHub comments, forum threads, a mailing list, or published meeting minutes.
- CAB deliberations should be documented in a publicly accessible location for long-term reference and transparency.

### Advance Notice Requirements
- SIP authors must provide adequate notice to the relevant CAB(s) before a SIP enters the CAB Review phase. 
- CABs should be given sufficient time to prepare, gather expertise, and schedule discussion as needed.

### Comment Resolution Prior to Vote
- All CAB comments must be fully addressed before a SIP may advance to a public vote. 
    - Unresolved comments or substantive open questions prevent the SIP from moving forward.
- CAB Chairs and SIP Deputies share responsibility for confirming that comments are resolved.

### CAB Quorum and Participation
- CABs must establish minimum participation or quorum expectations so that a small minority cannot advance or block SIPs without broad engagement.
- CABs may designate deputies or alternates who can vote or comment on behalf of absent members, provided they follow the same Code of Conduct and disclosure requirements.

### Non-Compliance and Replacement
- If CAB members fail to participate consistently, violate process expectations, or demonstrate chronic non-responsiveness, the Steering Committee may replace them.
- A public record of CAB membership, attendance expectations, and replacement criteria shall be maintained.

### Steering Committee Refresh
- Before implementing governance-impacting SIPs, the Steering Committee should be refreshed or reconfirmed where feasible, to support legitimacy and broad community trust. This is a recommended practice, not a precondition for a SIP's activation or certification.

### Communication Expectations
- CAB members and SIP authors are expected to maintain clear, timely communication during all review phases.
- CAB Chairs should provide short summaries of decisions or review outcomes so authors and the community can track progress.

These improvements ensure that CABs operate predictably, transparently, and in alignment with the community’s expectations for responsible governance.

---

## Governance Definition & Ownership

This section formalizes how decision-making authority and repository control are distributed among the primary SIP governance bodies.

### Authority Boundaries
- The Steering Committee (SC) retains final decision authority over SIP ratification and can delegate merge permissions to Deputies after CAB approval.
- Consideration Advisory Boards (CABs) provide review and recommendations but do not hold merge or ratification authority.
- SIP Deputies enforce standards, manage formatting and numbering, and maintain the SIP index, but may only merge procedural or editorial updates unless authorized by the SC.

### Repository Scope
- The SIP repository serves as a public bulletin board for both ratified and non-ratified SIPs (Draft, Accepted, Recommended, Activation-In-Progress, Withdrawn, and Rejected). All must remain accessible for transparency.

### What Qualifies as a SIP
- A SIP must propose a change, standard, or process affecting the design, governance, or operation of the Stacks blockchain. General discussions or implementation tasks should remain GitHub issues, not SIPs.

### Governance Maintenance
- Where feasible, the Steering Committee should be refreshed or re-confirmed before enacting new governance SIPs. This is aspirational guidance; a SIP's Activation section is the sole authoritative checklist for its own activation and certification (see [Steering Committee Certification](./steering_committee.md#steering-committee-certification)).

### Compensation

Compensation for carrying out committee duties is outside of the scope of this document. This document does not create a provision for compensation for committee participation, but it does not forbid it either.
