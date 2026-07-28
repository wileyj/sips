# Consideration Advisory Board Voting Procedures

## Purpose

This document establishes standardized voting procedures for all Consideration Advisory Boards (CABs) when evaluating SIPs under their respective expertise areas. These procedures ensure consistent, transparent, and fair decision-making across all CABs, regardless of size or specialization.

---

## 1. Voting Authority and Scope

### 1.1 CAB Voting Mandate
Each Consideration Advisory Board has the authority to vote on SIPs that fall within their designated consideration track. CAB votes determine whether a SIP advances from **Accepted** status to:
- **Recommended** status (CAB approval), or
- **Rejected** status (CAB disapproval)

### 1.2 Prerequisites for CAB Voting
A CAB may only vote on a SIP when all of the following conditions are met:

1. The SIP has completed the **minimum review periods** as defined in the CAB Voting & Ratification Clarity document:
   - Draft Open Comment Period: minimum 2 weeks
   - CAB Review Period: minimum 1 week
   - Final Comment Resolution Period: minimum 1 week

2. The SIP text is **stable and review-complete** with no substantive changes pending

3. All outstanding substantive comments have been addressed or formally acknowledged

4. The SIP has been formally submitted to the CAB by the SIP author or Steering Committee

### 1.3 Stable Text Enforcement
- Once a CAB vote begins, **no substantive changes** may be made to the SIP
- Only editorial corrections (typos, formatting) may be accepted, and only with explicit CAB awareness
- Any substantive change requires immediate suspension of the vote and triggers a mandatory re-vote after the change is finalized

---

## 2. CAB Voting Thresholds

To accommodate CABs of varying sizes while maintaining legitimacy and fairness, voting thresholds are structured based on board membership size.

### 2.1 Standard CAB (5+ Members)

**Quorum:**
- Minimum 60% of current CAB members must participate in the vote
- For a 5-member CAB: minimum 3 members
- For a 7-member CAB: minimum 5 members

**Approval Threshold:**
- Simple majority of votes cast (50% + 1)
- Abstentions count toward quorum but not toward majority calculation

**Example:** 5-member CAB with 4 members voting (quorum met)
- 3 Yes, 1 No = **Approved**
- 2 Yes, 2 No = **Rejected** (tie defaults to rejection)

### 2.2 Small CAB (4 Members)

Small CABs present unique challenges where traditional quorum (60% = 2.4, rounds to 3) could create voting deadlocks. The following adapted rules apply:

**Quorum:**
- Minimum 3 of 4 members must participate
- If only 2 members are available after good-faith outreach, the vote may proceed with Steering Committee approval and must be documented as "reduced quorum"

**Approval Threshold - Affirmative Vote Requirement:**
- Minimum **3 affirmative votes** required for approval
- This ensures meaningful support even in a 4-member body

**Voting Outcomes:**
- 4 members voting: 3+ Yes = Approved; 2 or fewer Yes = Rejected
- 3 members voting: 3 Yes = Approved; 2 or fewer Yes = Rejected
- 2 members voting (reduced quorum): Both must vote Yes = Approved; otherwise Rejected

**Rationale:** Requiring 3 affirmative votes ensures that approval represents majority support (75%) rather than a simple coin-flip, while still allowing the small CAB to function.

### 2.3 Very Small CAB (3 Members)

**Quorum:**
- All 3 members should participate
- Minimum 2 members may constitute quorum in exceptional circumstances with SC approval

**Approval Threshold:**
- Minimum **2 affirmative votes** required for approval

**Voting Outcomes:**
- 3 members voting: 2+ Yes = Approved; otherwise Rejected
- 2 members voting (reduced quorum): Both must vote Yes = Approved; otherwise Rejected

### 2.4 Tie-Breaking and Default Positions

- In all cases where the required affirmative vote threshold is not met, the proposal is **Rejected**
- CAB Chairs do not have tie-breaking authority; ties default to rejection
- A rejected SIP may be revised and re-submitted for future consideration

---

## 3. Voting Process

### 3.1 Vote Initiation

The CAB Chair shall initiate a vote by:

1. Confirming all voting prerequisites are met (Section 1.2)
2. Posting a **formal vote announcement** in the CAB's public communication channel (GitHub issue, forum, mailing list, etc.)
3. Including in the announcement:
   - SIP number and title
   - Link to the stable SIP text being voted on
   - Voting period start and end dates (minimum 7 calendar days)
   - Instructions for casting votes
   - Quorum and approval threshold requirements

### 3.2 Voting Period

**Duration:**
- Minimum 7 calendar days
- May be extended at the Chair's discretion for complex proposals or to accommodate member schedules

**Voting Methods:**
- Votes must be cast publicly in a verifiable manner
- Acceptable methods include:
  - GitHub issue comments with clear vote format (e.g., "Vote: Approve" or "Vote: Reject")
  - Dedicated voting platform with public results
  - Email to a public mailing list archive
  - CAB meeting minutes with recorded votes

**Vote Options:**
- **Approve (Yes)**: CAB member believes the SIP is feasible, practical, and beneficial
- **Reject (No)**: CAB member believes the SIP has significant concerns or should not advance
- **Abstain**: CAB member declines to vote (counts toward quorum only)

### 3.3 Vote Closure

The CAB Chair shall:

1. Close the vote at the announced end time
2. Tally all votes cast during the voting period
3. Determine if quorum was met
4. Determine if the approval threshold was met
5. Publish the **official vote results** within 48 hours, including:
   - Total members eligible to vote
   - Number of votes cast (quorum status)
   - Breakdown of Approve/Reject/Abstain
   - Final outcome (Recommended or Rejected)
   - Link to vote record

### 3.4 Documentation and Transparency

All vote records must be:
- Publicly accessible
- Permanently archived
- Linked from the SIP itself
- Included in CAB meeting minutes or equivalent public record

---

## 4. Special Circumstances

### 4.1 Emergency or Time-Sensitive Votes

For urgent security fixes or time-critical proposals, CABs may use an **expedited voting procedure**:

- Minimum voting period: 48 hours (instead of 7 days)
- Requires 100% of CAB members to acknowledge the expedited timeline
- Quorum requirements remain unchanged
- Must be approved by Steering Committee before initiation
- Final results must document the emergency justification

### 4.2 Unavailable Members

If a CAB member is unavailable (on leave, unresponsive, etc.):

- The Chair should make good-faith efforts to contact the member
- If unavailable beyond 72 hours and the voting period is ending, proceed without that member
- Document the outreach attempts in the vote record
- For small CABs (4 or fewer members), consider requesting SC approval for reduced quorum

### 4.3 Member Recusal and Conflicts of Interest

CAB members should recuse themselves from voting when they have a conflict of interest:

- Direct financial interest in the SIP outcome
- Significant involvement in authoring the SIP
- Personal relationship that could compromise objectivity

**Recusal Process:**
1. Member publicly declares recusal with brief explanation
2. Recused member is excluded from quorum calculation for that vote only
3. Remaining members vote according to the adjusted quorum threshold

**Example:** 5-member CAB with 1 recusal = 4 members eligible
- New quorum: 60% of 4 = 2.4, rounds to 3 members
- Approval requires majority of votes cast

### 4.4 Vote Invalidation and Re-Votes

A vote must be invalidated and re-held if:

1. **Substantive SIP changes** occur during the voting period
2. **Procedural violations** are discovered (e.g., quorum miscalculated, vote manipulated)
3. **New material information** emerges that significantly impacts the evaluation

**Re-Vote Requirements:**
- The Chair or any CAB member may call for vote invalidation with justification
- SC must approve vote invalidation if challenged
- New vote follows standard procedures with minimum 7-day voting period
- Original vote is marked invalid in the record

---

## 5. CAB Approval and Public Voting

### 5.1 CAB Approval as Prerequisite

Per the CAB Voting & Ratification Clarity document:
- A SIP cannot proceed to public or ecosystem-wide voting until the relevant CAB(s) have formally approved it (voted Recommended)
- CAB approval must be documented via public vote records
- Multiple CABs may need to approve if the SIP spans multiple consideration tracks

### 5.2 Post-CAB Vote SIP Updates

Once a CAB vote concludes with approval:

**Minor Updates Permitted:**
- Editorial corrections (typos, formatting)
- Implementation detail clarifications that don't alter intent
- Must be shared in CAB communication channels
- Must be visible in the SIP's pull request for auditability

**CAB Re-Vote Required If:**
- Any CAB member believes the change alters the SIP's meaning, intent, semantics, or functional behavior
- The determination is made jointly by the CAB Chair and a SIP Deputy

**Documentation:**
- The Chair should note all post-vote updates in meeting minutes and/or SIP PR discussion

### 5.3 Rider SIP Determinations

When a CAB votes on a Rider SIP (see [rider-sip.md](./rider-sip.md)), the CAB's vote record must
additionally state whether the Rider requires the parent SIP's public vote to be re-done,
or done jointly with the Rider (see [rider-sip.md](./rider-sip.md) for the underlying rules on when this
applies). This determination and its rationale must be documented in the CAB's meeting
minutes and posted as a response on the Rider SIP's own pull request.

---

## 6. Appeal and Dispute Resolution

### 6.1 Appeal Process

If a SIP author or community member believes a CAB vote was conducted improperly, they may appeal to the Steering Committee:

**Grounds for Appeal:**
- Procedural violations (quorum not met, improper notice, etc.)
- Conflict of interest not disclosed
- Vote occurred on unstable or changing SIP text
- CAB acted outside its designated consideration track

**Appeal Procedure:**
1. Submit written appeal to SC within 14 days of vote closure
2. Include specific procedural violations and evidence
3. SC reviews appeal and may:
   - Uphold the CAB vote
   - Order a re-vote with corrected procedures
   - Reassign the SIP to a different CAB if appropriate

### 6.2 Steering Committee Oversight

The Steering Committee reserves the right to:
- Review any CAB vote record for compliance
- Request clarification on voting outcomes
- Intervene in cases of repeated procedural violations
- Modify these voting procedures with community input

---

## 7. Multi-CAB Coordination

### 7.1 When Multiple CABs Review a SIP

Some SIPs may require review and approval from multiple CABs (e.g., a proposal affecting both security and network consensus):

**Coordination Process:**
1. SIP author identifies all relevant consideration tracks in the SIP preamble
2. Each CAB conducts its own independent vote
3. All relevant CABs must vote Recommended for the SIP to advance
4. If any CAB votes Rejected, the SIP does not advance (author may revise and resubmit)

**Timing:**
- CAB votes may occur sequentially or in parallel
- Recommended approach: sequential, so each CAB can consider prior CABs' feedback
- Total timeline should respect the cumulative minimum review periods

### 7.2 CAB Disagreements

If CABs provide conflicting recommendations:
- The Steering Committee may facilitate discussion between CABs
- CABs may jointly agree to defer to one CAB's expertise
- If unresolvable, the Steering Committee makes the final determination on advancement

---

## 8. Voting Records and Reporting

### 8.1 Required Vote Documentation

For each vote, the CAB Chair must maintain a public record containing:

- SIP number and title
- Vote initiation date and announcement link
- Voting period dates
- Stable SIP text version/commit hash voted on
- List of eligible voters
- Individual vote records (member name + vote)
- Quorum calculation and status
- Approval threshold calculation and status
- Final outcome (Recommended/Rejected)
- Any special circumstances or notes

### 8.2 Transparency Requirement

Vote records must be:
- Posted in the same public venue as the vote announcement
- Linked from the SIP's GitHub PR or tracking issue
- Archived in the CAB's permanent records
- Accessible to the entire community indefinitely

### 8.3 Annual Reporting

Each CAB Chair should provide an annual summary to the Steering Committee:
- Total SIPs reviewed
- Vote outcomes (Recommended/Rejected counts)
- Average review timeline
- Any procedural issues encountered

---

## 9. Amendments to Voting Procedures

### 9.1 Modification Process

These voting procedures may be amended through:

1. Proposal by any CAB Chair, SC member, or community member
2. Review period of minimum 30 days with public comment
3. Approval by the Steering Committee
4. Notification to all CAB Chairs
5. Grace period of 14 days before new procedures take effect

### 9.2 Backwards Compatibility

Votes in progress when amendments take effect:
- Continue under the procedures in place when the vote started
- New procedures apply only to votes initiated after the effective date

---

## Appendix A: Quick Reference - Voting Thresholds by CAB Size

| CAB Size | Quorum Required | Approval Threshold | Example Outcome |
|----------|----------------|-------------------|-----------------|
| 3 members | 3 (or 2 with SC approval) | 2 affirmative votes | 2 Yes = Approved |
| 4 members | 3 (or 2 with SC approval) | 3 affirmative votes | 3 Yes of 4 voting = Approved |
| 5 members | 3 members | Majority of votes cast | 2 Yes, 1 No = Approved |
| 6 members | 4 members | Majority of votes cast | 3 Yes, 2 No = Approved |
| 7 members | 5 members | Majority of votes cast | 3 Yes, 2 No = Approved |
| 8+ members | 60% of members | Majority of votes cast | Scales proportionally |

---

## Appendix B: Sample Vote Announcement Template

```markdown
# CAB Vote: SIP-XXX [Title]

**Status:** Vote Open  
**SIP:** [SIP-XXX: Title](link-to-stable-version)  
**CAB:** [Consideration Advisory Board Name]  
**Vote Period:** [Start Date] to [End Date] (7 days)

## Summary
[Brief 2-3 sentence summary of what this SIP proposes]

## Voting Instructions

Please cast your vote by replying to this issue with one of:
- **Vote: Approve** - I believe this SIP is feasible, practical, and beneficial
- **Vote: Reject** - I have concerns about this SIP advancing
- **Vote: Abstain** - I decline to vote but wish to be counted for quorum

## Requirements
- **Quorum:** [X] of [Y] members must vote
- **Approval:** [Threshold description]

## Current Status
- Eligible voters: [X]
- Votes cast: [X]
- Quorum met: [Yes/No]

---

## Notes
_This section shall contain applicable notes as a SIP is being considered_

```

---

## Document History

- **Version 1.0** - [Date] - Initial voting procedures established
- Integrates with CAB Voting & Ratification Clarity requirements
- Addresses small CAB quorum challenges
- Establishes transparent, predictable voting pipeline
