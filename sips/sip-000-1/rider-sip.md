# Rider SIPs

## Definition

A **Rider SIP** is a secondary proposal that bundles additional, related changes into a
parent SIP that has not yet been Ratified — allowing closely related changes discovered
after the parent SIP's drafting to be voted on together, rather than requiring an
entirely separate SIP process (and, for hard-fork SIPs, an entirely separate public vote).

A Rider SIP must receive its own SIP number and must undergo the full standard pipeline (Draft →
Accepted → Recommended, including full CAB review) like any other SIP — it is not a
shortcut around review, only around running a second full public vote where one can
reasonably cover both.

## When Rider SIPs Are Used

Riders are typically used for **Consensus-Hard-Fork** parent SIPs, where the barrier to
ratification (a full public/token-holder vote per [activation-voting.md](activation-voting.md)) is highest, and
re-running that vote for a small follow-on change is disproportionate. Common cases:

- Additional, closely related consensus changes discovered after the parent SIP was
  drafted (e.g. A function related to the parent SIP requires additional change).
- Correcting an activation condition that was missed or needs updating (e.g., a specified
  activation block height that passed before the SIP's implementation criteria were met).

## Constraints

- **A Rider may only attach to a parent SIP that has not yet reached Ratified status.**
  Once a parent SIP is Ratified, no Rider may be attached to it — any further change must
  be submitted as an entirely new, independent SIP. This prevents a Rider from being used
  to bypass the vote requirements a Ratified SIP already satisfied.
- A Rider may attach at any point before Ratification, including while the parent is in
  Activation-In-Progress status.

## Process

1. **Submission.** The Rider is submitted as its own SIP, and must reference the parent SIP it rides on.
2. **Full review.** The Rider goes through the standard pipeline in full: Deputy review to
   assign a SIP number and move to Accepted status, then full CAB review by the relevant Consideration Advisory Board(s), per
   [procedure.md](procedure.md).
3. **Parent SIP update.** Once the Rider exists, a SIP Deputy or the Steering Committee updates the parent
   SIP via pull request to add a `Requires:` field referencing the Rider SIP.
4. **CAB determination on public re-vote.** As part of its vote on the Rider (per
   [procedure.md](procedure.md)), the reviewing CAB(s) must determine whether the Rider's content is
   substantive enough to require the parent SIP's public vote to be re-done (or, if the
   parent hasn't yet had its public vote, to be done jointly with the Rider). A narrow,
   limited-scope Rider (e.g., a block-height correction alone) may not require a public
   re-vote; a Rider that changes implementation details beyond the narrow scope of the
   correction (e.g., also altering a token emission schedule) would.
   - This determination, and the CAB's reasoning for it, must be recorded in the CAB's
     meeting minutes (submitted via PR to the repository's `minutes` directory, per
     standard CAB documentation practice) **and** posted directly as a response on the
     Rider SIP's own pull request, so the requirement is visible to the SIP's authors and
     the community without needing to locate the minutes separately.
5. **Type escalation.** If the Rider's own Type would independently require a public vote
   that the parent's Type did not (e.g., a Hard-Fork Rider attached to a Soft-Fork
   parent), the parent is included in the public vote regardless of the CAB's
   determination in step 4.
6. **Joint vote, if triggered.** Where a public vote is required per step 4 or step 5, the
   parent and Rider are voted on together, as a single bundled vote — not two separate
   votes.
