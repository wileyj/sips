# SIP Editor

By far the largest committee in the SIP process is the SIP Editor Committee. The SIP Editors are responsible for maintaining the "inbound funnel" for SIPs from the greater Stacks community. SIP Editors ensure that all inbound SIPs are well-formed, relevant, and do not duplicate prior work (including rejected SIPs).

## Membership

Anyone may become a SIP Editor by recommendation from an existing SIP Editor, subject to the “Recruitment” section below.

## Qualifications

A SIP Editor must demonstrate proficiency in the SIP process and formatting requirements. A candidate SIP Editor must demonstrate to an existing SIP Editor that they can independently vet SIPs.

## Responsibilities

SIP Editors are concerned with shepherding SIPs from Draft status to Accepted status, and for mentoring community members who want to get involved with the SIP processes (as applicable).

### Edit Rights by Status

| SIP Status | Who Can Edit | Process |
|------------|--------------|---------|
| **Draft / Proposed** | Authors | May open PRs and make minor updates, subject to review |
| **Accepted / Ratified** | SIP Editors, CAB members, Steering Committee | Authors may suggest corrections via new PRs but cannot directly commit |

### Post-Merge Changes

Once a SIP is merged, modifications are strictly limited:
- **Permitted  changes:** Procedural, non-substantive corrections only
  - Typo fixes
  - Adding vote results
  - Updating broken links
  - Formatting corrections

- **Required approval:** All post-merge edits must be reviewed and approved by a SIP Editor before merge

This ensures finalized SIPs remain auditable, properly attributed, and maintain their original intent.



### Getting Users Started

SIP Editors should be open and welcoming towards enthusiastic users who want to help improve the greater Stacks ecosystem. As such, SIP Editors should encourage users to submit SIPs if they have good ideas that may be worth implementing.

In addition, SIP Editors should respond to public requests for help from community members who want to submit a SIP. They may point them towards this document, or towards other supplemental documents and tools to help them get started.

### Feedback

When a SIP is submitted in Draft status, a SIP Editor that takes the SIP into consideration should provide fair and full feedback on how to make the SIP ready for its transition to Accepted status. 

To do this, the SIP Editor should:

- Verify that the SIP is well-formed according to the criteria defined in the SIP process
- Verify that the SIP has not been proposed before
- Verify as best that they can that the SIP is original work
- Verify that the SIP is appropriate for its type and consideration
- Recommend additional Considerations if appropriate
- Ensure that the text is clear, concise, and grammatically-correct English
- Ensure that there are appropriate avenues for discussion of the SIP listed in
  the preamble.

The SIP Editor does not need to provide public feedback to the SIP authors, but
should add their name(s) to the Signed-off field in the SIP preamble once the SIP is ready to be Accepted.

### Acceptance

Once a SIP is moved to Accepted, the SIP Editor shall assign it the smallest positive number not currently used to identify any other SIP. Once that number is known, the SIP Editor shall set the SIP's status to Accepted, set the number, and commit the SIP to the SIP repository in order to make it visible to other SIP Editors and to the Consideration Advisory Boards. Additionally, once a SIP is accepted, it shall be added to the table of SIPs in the repository `README.md` document.

### Recruitment

Each SIP Editor must list their name and contact information in an easy-to-find location in the SIP repository, as well as a list of each SIP Editor they have recommended.  In so doing, the SIP Editors shall curate an “invite tree” that shows which Editors recommended which other Editors.

A SIP Editor may recommend another user to be a SIP Editor no more than once per month, and only if they have faithfully moved at least one SIP to Accepted status in the last quarter.  If a SIP Editor does not participate in editing a SIP for a full year and a day, then they may be removed from the SIP Editor list.  The SC may remove a SIP Editor (and some or all of the users he or she recommended) if they find that the SIP Editor has violated the SIP Code of Conduct.

Newly-Accepted SIPs, new SIP Editor recruitment, and SIP Editor retirement shall be submitted as pull requests by SIP Editors to the SIP repository.
