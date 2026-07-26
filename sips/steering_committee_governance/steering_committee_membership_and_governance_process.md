# Preamble

SIP Number: XXX

Title: Steering Committee Membership and Governance Process

Author: Jesse Wiley <jesse@stacks.org>

Consideration: Governance

Type: Meta

Status: Draft

Created: [2026-04-06]

License: BSD-2-Clause

Sign-off:

Discussions-To: https://github.com/stacksgov/sips

Requires: 000

# Abstract

This SIP defines a formal governance process for the Stacks Improvement
Proposal (SIP) Steering Committee (SC). Specifically, it establishes rules
governing the composition of the SC, including the number of active and
alternate members, term limits for all members, qualifications for membership, 
the process by which new members may be nominated and seated, the conduct of all
SC correspondence, and the framework by which SC members may be compensated for
their service. The intent of this SIP is to ensure that the SC
remains accountable, adequately staffed, and capable of fulfilling its duties as
described in SIP-000, while maintaining continuity of governance across member
transitions.

# License and Copyright

This SIP is made available under the terms of the BSD-2-Clause license,
available at https://opensource.org/licenses/BSD-2-Clause. This SIP's copyright
is held by the Stacks Open Internet Foundation.

# Introduction

SIP-000 established the Steering Committee (SC), but does not fully specify many of the operational details that govern how the SC itself is constituted and maintained over time. In particular, SIP-000 leaves open questions regarding how many members should comprise the SC, how vacancies are filled, how nominations are made, what communication channels govern SC business, and whether or how members may receive compensation.

This SIP attempts to address some of these gaps in SIP-000. The proposed process: 
- Prioritizes transparency (by requiring all correspondence to be conducted via a public mailing list).
- Accountability (through a restricted but clearly defined nomination process)
- Continuity (through the provision of alternate members who may vote in the absence of active members).  
This SIP does not (and shall not be construed to) grant new powers to the SC over and above those defined in SIP-000.

# Specification

## Steering Committee Composition

### Active Members

The Steering Committee (SC) shall at all times consist of exactly three (3) active, voting members. Active members bear the full duties and responsibilities of the SC as described in SIP-000, including attending public meetings, voting on SIPs, recognizing Consideration Advisory Boards, and overseeing SIP activation and
ratification.

A quorum for the purpose of conducting official SC business shall be any two (2) of the three (3) active members, or any combination of active and alternate members that results in at least two (2) eligible voters being present, subject to the rules governing alternate member voting described below.

### Alternate Members

The Steering Committee shall maintain a roster of exactly two (2) alternate
members. Alternate members are non-voting participants in SC proceedings under
normal circumstances, but are empowered to vote in place of an active member
under any of the following conditions:

- An active member provides advance written notice to the SC mailing list that
  they will be absent from a scheduled meeting or vote AND fails to provide (or explicitly yields to the alternate) a written vote for the meeting
- An active member is unresponsive for a period of fourteen (14) or more
  consecutive calendar days during an active deliberation or vote
- An active member has formally vacated their seat, and a successor has not yet
  been seated.
- An active member is under review for failing to adhere to the SIP Code of Conduct.

When an alternate member votes in place of an active member, this shall be
recorded in the meeting minutes and published to the SC's public mailing list.
In no case shall there be more than three (3) total votes cast in any SC deliberation. The method by which an alternate may be required to cast a vote shall be chosen by the active SC members on a case by case basis, e.g. the first alternate who affirms their willingness to participate. 

Alternate members are expected to remain informed of all ongoing SC business,
attend public meetings as observers, and be prepared to assume an active
membership seat when one becomes vacant.

## Qualifications

The qualifications for SC membership shall remain as defined in SIP-000. For
reference, all candidates for active or alternate SC membership:

- Must possess deep domain expertise pertinent to blockchain development;
- Must possess excellent written communication skills; and
- Should  have authored at least one ratified
  technical-consideration SIP prior to joining the committee.

All SC members must abide by the SIP Code of Conduct at all times. Failure to
adhere to the Code of Conduct shall be grounds for immediate removal from the
SC, with no eligibility to rejoin any SC seat until the matter has been formally
reviewed and resolved per the relevant Ethics-consideration SIP or, in the
absence of such a SIP, at the SC's unanimous discretion (excluding the affected
member).

## Correspondence and Public Communication

### Public Mailing List

All official SC correspondence shall be conducted via a designated public mailing
list. This includes, but is not limited to:

- Deliberations and votes on SIPs in Recommended status;
- Discussions regarding the recognition or rescission of Consideration Advisory
  Boards
- Nomination and seating of new SC members (active or alternate)
- Notices of member absences and alternate member substitutions
- Announcements of public meeting schedules and agendas
- Publication of meeting minutes
- Any formal communications between the SC and Consideration Advisory Boards,
  SIP Editors, or the Stacks Open Internet Foundation.

The Stacks Open Internet Foundation shall provision and maintain the public
mailing list infrastructure:
- The mailing list archive shall be accessible to the public in read-only form. 
- Any member of the public may  subscribe to the mailing list as an observer. 
- Posting rights shall be limited to SC members (active and alternate), the SC's designated moderators and note-takers, and, at the SC's
discretion, other formally recognized parties (e.g., Consideration Advisory
Board chairpersons).

### Prohibition on Private Deliberation

No binding SC vote or formal decision may be made via private or semi-private communication channels. Any deliberation that begins in a private channel must be re-initiated and concluded on the public mailing list before a binding vote may take place. This requirement does not preclude informal pre-deliberation discussions among members, but such discussions shall not substitute for the required public process.

### Meeting Minutes

The SC's appointed note-taker shall publish complete meeting minutes to the
SIPs public repository within five (5) business days following each public meeting. Minutes shall include a record of attendance (including any alternate member substitutions), all motions raised, votes cast (including individual member
votes), and any action items assigned.

## Nomination Process

### Eligibility to Nominate

Nominations for active or alternate SC membership may be submitted only by the
following parties:

- Any current SC member (excluding alternates)
- The Stacks Open Internet Foundation Board (acting by unaminous vote of its own membership).

To prevent conflicts of interest and to adhere to existing governance standards, self-nominations are not permitted. No individual may be nominated by more than
one nominating party per vacancy. If multiple nominations are received for the
same vacancy, the SC shall evaluate all nominees and select the most qualified
candidate by a two-thirds majority vote.

### Nomination Procedure

When a SC seat becomes vacant, the SC shall notify the public mailing list within seven (7) calendar days of the vacancy arising. The notification shall describe the nature of the vacancy (active or alternate), the anticipated timeline for filling it, and an invitation for eligible nominators to submit candidates.

Nominations shall be submitted to the public mailing list and shall include:

- The full name and contact information of the nominee
- A statement of the nominee's qualifications relative to those defined in
  SIP-000 and reiterated in this SIP
- A brief description of why the nominating party believes the nominee is suited
  to serve on the SC
- Written confirmation from the nominee that they accept the nomination, are
  aware of the responsibilities of the role, and agree to abide by the SIP Code
  of Conduct.

The nomination window shall remain open for no fewer than fourteen (14) calendar days, and will remain open until the vacancy is filled.  Each nomination will be voted upon by the active SC members within thirty (30) days of the nomination being received.  If there are no nominations after thirty (30) days, then the SC shall re-post the vacancy on the public mailing list in a bid to continue to solicit nominations.

### Evaluation and Seating

Following the close of the nomination window, the SC shall deliberate publicly
on the mailing list and vote to seat one nominee per vacancy. Active SC members
shall vote; alternate members may participate in deliberation but may not vote
on seating decisions unless substituting for an absent active member per the
rules described above. The vote to seat a nominee shall require a two-thirds
majority of eligible voters, with alternates potentally included (per the rules in this document) to reach quorum in the case of multiple nominees being voted on. 

Once a nominee is voted into a seat, the SC shall announce the seating decision
on the public mailing list and update the SC's public member roster accordingly.
The newly seated member's term shall begin on the date of the seating
announcement.

### Promotion of Alternate Members

When an active member seat becomes vacant, the SC should, as a matter of first
recourse, consider whether one of the existing alternate members is qualified and willing to be promoted to the active seat. If so, the SC may vote to promote an alternate member to the active seat without opening a full nomination window, provided that the promotion vote satisfies the two-thirds majority threshold. The resulting vacancy in the alternate roster shall then be filled through the standard nomination process. Only a single alternate may be promoted during any  six (6) month timeframe from the last alternate member promotion, with the requirement that the promoted SC member has remained active since being promoted. 

## Compensation

### Scope

This SIP establishes a framework for SC member compensation but does not itself
prescribe specific compensation amounts or funding sources. Specific
compensation arrangements shall be documented in supplemental materials ratified
alongside or subsequent to this SIP, and may be revised by a subsequent
Governance-consideration SIP or by agreement of the Stacks Open Internet
Foundation Board.

### Eligibility

All active SC members are eligible for compensation for the time they dedicate to carrying out their SC duties. Alternate members are eligible for compensation
when actively substituting for an absent active member, and for their ongoing
participation in SC business as observers and in preparation for potential
activation. Moderators and note-takers appointed by the SC are separately
eligible for fixed, regular bounties as described in SIP-000.

### Principles

Any compensation structure adopted under this SIP shall adhere to the following
principles:

- **Transparency.** All compensation arrangements, including amounts, payment
  schedules, and funding sources, shall be published on the SC's public mailing
  list and maintained as supplemental documentation to this SIP.
- **Consistency.** All active members serving concurrently shall receive equal
  compensation for equivalent duties, unless a member has voluntarily declined
  compensation in writing to the public mailing list.
- **Non-conflicting.** Compensation arrangements shall not create financial
  incentives that conflict with the SC's duty to act in the best interests of the broader Stacks user community. SC members who identify a potential compensation-related conflict of interest in relation to a particular SIP vote shall recuse themselves from that vote and notify the public mailing list.
- **Foundation-backed.** Compensation shall be sourced from the Stacks Open
  Internet Foundation or from a funding mechanism ratified by the SC under a
  separate Economic-consideration SIP. No SC member shall accept compensation
  from any external party in connection with their SC duties without the unanimous written consent of the other active SC members, published to the public mailing list.

Failure to adhere to the above may be grounds for immediate termination from the SC and a lifetime ban from participating in the SIP process..

# Related Work

This SIP builds directly upon SIP-000, which established the Steering Committee
and defined its duties, voting thresholds, and relationship to other governance
bodies in the Stacks ecosystem. 
https://github.com/stacksgov/sips/blob/main/sips/sip-000/sip-000-stacks-improvement-proposal-process.md#related-work


# Backwards Compatibility

This SIP modifies the governance structure of the Steering Committee as
established by SIP-000 and is therefore backwards-incompatible with any SC
compositions or practices that do not conform to the rules herein. Upon
activation, any current SC members whose terms exceed the limits specified in
this SIP shall be grandfathered in for their current term only and shall not be
eligible for re-appointment until the cooling-off period described in this SIP
has elapsed. The SC shall take steps to achieve the composition defined in this
SIP (three active, two alternate members) within ninety (90) days of activation.

# Activation

This SIP shall be considered activated once all of the following criteria have
been met:

1. The SC has voted to move this SIP from Recommended status to
   Activation-In-Progress status, by the two-thirds majority threshold applicable
   to non-technical SIPs as defined in SIP-000.
2. The Stacks Open Internet Foundation has provisioned a public mailing list for
   SC correspondence and confirmed its availability in writing on that mailing
   list.
3. The SC has published a public notice on the mailing list acknowledging the
   activation of this SIP and describing the steps it will take to achieve the
   required membership composition within the ninety (90) day transition window.
4. The SC has published an updated public member roster reflecting the current
   composition of the SC (active and alternate members), including each member's
   seat start date.

Upon activation, the SC shall have ninety (90) days to achieve full compliance
with the membership composition requirements of this SIP (three active members,
two alternate members), using the nomination process defined herein. Progress
shall be reported on the public mailing list no less than once per month during
the transition period.

If the SC is unable to achieve full compliance within ninety (90) days, it shall
publish a detailed explanation on the public mailing list and request guidance
from the Stacks Open Internet Foundation Board, which may grant a one-time
extension of up to sixty (60) additional days.

# Reference Implementations

Not applicable.
