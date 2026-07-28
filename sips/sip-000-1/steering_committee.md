# Steering Committee

## Steering Committee Duties

The Steering Committee's (SC) overarching duty is to oversee the evolution of the Stacks blockchain’s design, operation, and governance in a way that is technically sound and feasible according to the rules and procedures described in this document. The SC shall be guided by and held accountable by the greater community of users, and shall make all decisions with the advice of the relevant Consideration Advisory Boards. 

The SC’s role is that of a steward. The SC shall select SIPs for ratification based on how well they serve the greater good of the Stacks users. Given the nature of blockchains, the SC's particular responsibilities pertaining to upgrading the blockchain network are meant to ensure that upgrades happen in a backwards-compatible fashion if at all possible. While this means that more radical SIPs may be rejected or may spend a long amount of time in Recommended status, it also minimizes the chances of an upgrade leading to widespread disruption (the minimization of which itself serves the greater good).

### Steering Committee Selection

Members of the Steering Committee are selected to ensure continuity, legitimacy, and accountability in Stacks governance.

- **Foundation Appointment**
  - All Steering Committee members must be approved by the Stacks Open Internet Foundation Board.
  - The Foundation Board is responsible for appointing initial and replacement members to the Steering Committee.

- **Community Representation**
  - At least one Steering Committee seat is reserved for a representative from the broader Stacks community, independent of the Stacks Foundation.
  - The process for selecting or ratifying community representatives may be defined through a separate SIP and informed by community input.

- **Selection Criteria**
  - Candidates should demonstrate relevant domain expertise, a history of constructive participation in the Stacks ecosystem, and the ability to act in the best interest of the network.
  - Prior involvement in SIP authorship, review, or governance processes is strongly preferred.

- **Changes and Succession**
  - Steering Committee membership may change over time due to resignation, replacement, or expansion of the committee.
  - Any changes to membership must be publicly documented.
  - Significant changes to Steering Committee composition should be communicated to the community in advance whenever feasible.

This selection process ensures that the Steering Committee remains trusted, capable, and accountable, while retaining a clear approval role for the Stacks Open Internet Foundation Board.


### Qualifications

Members of this committee must have deep domain expertise pertinent to blockchain development, and must have excellent written communication skills. It is highly recommended that members should have authored at least one ratified technical-consideration SIP before joining this committee.

### Responsibilities

#### Recognizing Consideration Advisory Boards.

The members of the Steering Committee must bear in mind that they are not infallible, and that they do not know everything there is to know about what is best for the broader user community. To the greatest extent practical, the SC shall create and foster the development of Consideration Advisory Boards in order to make informed decisions on subjects in which they may not be experts.

Any group of users can form an unofficial working group to help provide feedback to SIPs, but the SC shall have the power to recognize such groups formally as a Consideration Advisory Board via at least a two-thirds majority vote. The SC shall simultaneously recognize one of its members to serve as the interim chairperson while the Advisory Board forms. A SC member cannot normally serve on a Consideration Advisory Board concurrently with serving on the SC, unless granted a limited exception by a unanimous vote by the SC (e.g. in order to address the Board’s business while a suitable chairperson is found). Formally recognizing Consideration Advisory Boards shall occur in Public Meetings (see below) no more than once per quarter.

Once recognized, Consideration Advisory Boards may not be dissolved or dismissed, unless there are no Accepted or Recommended SIPs that request their consideration. If this is the case, then the SC may vote to rescind recognition of a Consideration Advisory Board with a two-thirds majority at one of its Public Meetings.

_If a recognized Consideration Advisory Board has no current members_ — whether because all members resigned, were removed, or the Board was never fully seated — the SC is responsible for seating initial members and a chairperson to restore the Board to active status, following the same recognition process described above. This is distinct from formally rescinding a Board's recognition, which requires that there be no Accepted or Recommended SIPs requesting its consideration, per the preceding paragraph.

In order to identify users who would form a Consideration Advisory Board, users should organize into an unofficial working group and submit a SIP to petition that SC recognizes the working group as a Consideration Advisory Board. This petition must take the form of a Meta-type SIP, and may be used to select the initial chairperson and define the Board's domain(s) of expertise, bylaws, membership, meeting procedures, communication channels, and so on, independent of the SC. The SC would only be able to ratify or reject the SIP.

The SC shall maintain a public index of all Consideration Advisory Boards that are active, including contact information for the Board and a summary of what kinds of expertise the Board can offer. This index is meant to be used by SIP authors to help route their SIPs towards the appropriate reviewers before being taken up by the SC.

#### Steering Committee Certification

The Steering Committee does not vote on the merits of a SIP. A SIP's approval is
determined entirely by its required CAB vote(s) (per [procedure.md](procedure.md)) and, where
applicable, a public vote (per [activation-voting.md](activation-voting.md)). These votes govern the
transition from Recommended to Activation-In-Progress, and require no separate SC vote.

#### Monitoring Activation-In-Progress SIPs

While a SIP is in Activation-In-Progress status, the SC is responsible for tracking
progress against the criteria in its Activation section — for example, monitoring miner
signaling thresholds, block-height targets, or other conditions the Activation section
specifies. The Activation section functions as an instruction manual the SC follows
faithfully; the SC does not have discretion to substitute its own judgment for what the
Activation section requires.

If, in the course of this monitoring, the SC determines that the Activation section's
criteria cannot be objectively verified as met or not met — for example, due to
ambiguous instructions, missing measurement criteria, or the absence of a prescribed
activation timeout — the SC may return the SIP to _Recommended_ status by unanimous
agreement of all currently seated SC members, with a detailed public explanation of
the deficiency. This is distinct from CAB review, which occurs before a SIP
reaches Activation-In-Progress and does not evaluate whether activation has actually
occurred. A SIP returned in this way must have its Activation section revised and
resubmitted for CAB approval before it can re-enter _Activation-In-Progress_.

#### Certification vote

Once a SIP in Activation-In-Progress status has satisfied all criteria in its Activation
section, the Steering Committee shall hold a single certification vote to confirm that:

- The correct CAB(s) for the SIP's consideration(s) voted, with proper quorum, per
[procedure.md](procedure.md).
- Any required public vote met its own quorum, threshold, and procedural requirements
per [activation-voting.md](activation-voting.md).
- All conditions in the SIP's Activation section have been objectively satisfied.

This certification vote requires unanimous agreement of all currently seated SC
members.

If certification fails because a requirement above was not met, the SC shall provide a
detailed public explanation of which requirement failed. The SIP remains in
Activation-In-Progress status pending correction — a failed certification is a
procedural finding, not a rejection of the SIP's merits, and does not move the SIP to
Rejected status.

Upon successful certification, the SC shall update the SIP's Status field to Ratified.


#### Feedback on Recommended SIPs

The Steering Committee shall give a full, fair, public, and timely evaluation to each SIP transitioned to Recommended status by Consideration Advisory Boards. A SIP shall only be considered by the SC if the Consideration Advisory Board chairperson for each of the SIP's considerations has signed-off on the SIP (by indicating as such on the SIP's preamble). 

If a SIP is moved to a Rejected status, the SIP authors may appeal the process by re-submitting it in Draft status once the feedback has been addressed. The appealed SIP must cite the SC’s feedback as supplemental material, so that SIP Deputies and Consideration Advisory Boards are able to verify that the feedback has, in fact, been addressed.


#### Public Coordination

The Steering Committee shall conduct SIP-related coordination and decision-making through public, observable channels, such as GitHub issues, pull requests, or the Stacks forum.

The Steering Committee may hold and record public meetings at its discretion. Meetings, when held, should focus on SIP ratification, committee coordination, or other active governance matters.

Any decisions or outcomes must be documented in a public venue. The absence of meetings does not prevent governance actions, provided public records are maintained.
