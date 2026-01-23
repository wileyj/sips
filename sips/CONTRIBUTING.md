# Contributing to SIPs

Thank you for your interest in contributing to the Stacks Improvement Proposals (SIPs) repository. This guide outlines the standards, procedures, and requirements for submitting and maintaining SIPs.

## Table of Contents

- [Submission Requirements](#submission-requirements)
- [Quality Standards](#quality-standards)
- [Review Process](#review-process)
- [Merge Requirements](#merge-requirements)
- [Finding SIPs](#finding-sips)
- [Version Control & Technical Guidelines](#version-control--technical-guidelines)
- [SIP Versioning and Replacements](#sip-versioning-and-replacements)

---

## Submission Requirements

### Fork-Based Workflow

**All SIP submissions must originate from a fork of the SIPs repository.** Direct branches in the main repository are prohibited.

**To submit a SIP:**

1. [Fork the SIPs repository to your GitHub account](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)
2. [Create a new branch in your fork for your SIP](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository)
3. Write your SIP following the template at https://github.com/stacksgov/sips/blob/main/sips/SIP_TEMPLATE.md
4. Submit a pull request from your fork to the main repository
5. Address reviewer feedback through additional commits to your PR

### Author Responsibilities

- **SIP authors may not resolve review comments** on their own submissions unless providing substantive changes or clear justification
- Comment resolution should remain visible to reviewers and Consideration Advisory Boards (CABs)
- Authors should respond to feedback promptly and professionally

---

## Quality Standards

All SIP submissions must meet high quality standards before being eligible for CAB review or merge.

### Polished State Requirement

- SIPs must reach a **highly polished, internally reviewed state** before moving to Proposed status
- Drafts with structural issues, missing sections, or formatting inconsistencies may be closed or deferred by Editors

### Formatting & Structure

- **Must adhere to SIP-000-1 document standards** including:
  - Required headers and sections
  - Proper ordering of content
  - Complete metadata in preamble
- Use the official SIP template as your baseline format
- Ensure consistent formatting throughout

### Plain-Language Writing

- Write in **clear, technically verifiable language**
- Avoid unnecessary jargon
- Support major claims with:
  - Implementation references
  - Data and metrics
  - Citations to research or prior work

### Prohibited Content

**Marketing language or promotional content is not permitted** in the main SIP text. This includes:

- Unsupported claims about benefits
- Promotional language
- Advocacy or commentary

Such material may be included in supplementary reference documents only.

---

## Review Process

### Reviewer Guidelines

- Provide constructive, specific feedback
- Focus on technical accuracy, completeness, and clarity
- Consider ecosystem impact and implementation feasibility

### Status Labels

All merged SIPs must include an accurate status:

- **Draft** - Work in progress, not yet ready for formal review
- **Proposed** - Ready for CAB consideration
- **Pending Vote** - Awaiting community vote
- **Accepted** - Approved and ready for implementation
- **Rejected** - Formally declined
- **Withdrawn** - Removed by author

**Only SIP Editors, CAB Chairs, or Steering Committee delegates may update the Status field** of a merged SIP.

---

## Merge Requirements

### Prerequisites for Merging

A SIP can only be merged into Main when **all** of the following conditions are met:

1. The SIP has received all relevant CAB sign-offs
2. Relevant CAB meeting minutes have been submitted and merged
3. Sign-off from a Steering Committee member has been added
4. For SIPs requiring public vote: An "Activation Status / Voting Results" section has been added with:
   - Verified vote tallies
   - Verification scripts
   - Audit links

### Merge Timing & Visibility

#### Pre-Vote vs Post-Vote Merging

- SIPs **may be merged before a public vote** if clearly labeled as "Proposed" or "Pending Vote"
- **Merging a SIP PR does not imply ratification**
- A SIP becomes ratified only after meeting activation criteria and Steering Committee verification

#### Visibility Requirements

- All SIPs referenced in release notes or upgrade documentation **must be merged** before publication
- Release notes shall not link to unmerged pull requests
- SIPs must be publicly accessible before being referenced in mainnet releases

#### Release Timing Buffer

A **minimum time buffer** must exist between:
1. Merging a SIP
2. Including it in a mainnet release

This allows for:
- Quality assurance testing
- Ecosystem review
- Developer verification
- Implementation alignment

The Steering Committee may set or request additional buffer requirements for hard fork SIPs.

---

## Finding SIPs

### SIP Index

The repository maintains an up-to-date index of all SIPs in BIP-style format, including:

- SIP Number
- Title
- Author(s)
- Status
- Consideration / Layer
- Relevant links (PR, Discussion, Merged File)

**SIP Editors are responsible for:**
- Maintaining this index
- Assigning SIP numbers early in the process
- Ensuring historical SIPs (including rejected/withdrawn) remain accessible

### Discoverability

- Release notes and announcements should link directly to merged SIPs
- All SIPs remain in the repository for historical context and version continuity

---

## Version Control & Technical Guidelines

### Repository Branch Restrictions

- **Contributors may not create branches** in the main SIP repository
- All submissions must originate from contributor forks
- Only authorized maintainers designated by the Steering Committee may create or maintain branches

### Hyperlink Formatting

All SIPs must use full, explicit URLs** for references and citations.

**Example:** "See https://github.com/stacksgov/sips/blob/main/sips/sip-000.md for more details`

This ensures long-term readability, prevents link rot, and maintains clarity for offline readers and archival tools.

### Activation Height Changes

If an approved activation height requires modification due to testing, security review, or implementation constraints:

1. A SIP Editor must open a PR documenting the change
2. Relevant CAB(s) must explicitly approve the update
3. A Steering Committee member must provide final sign-off

**The PR must include:**
- Rationale for the change
- Links to testing evidence or engineering constraints
- Updated activation criteria
- References to the parent SIP

**No activation-height modification is valid** unless recorded through this process.

### Hard Fork Release Branches

For SIPs introducing consensus changes or hard forks:

- A **dedicated release branch** must be created and maintained
- Only milestone-relevant changes may be merged into this branch
- Unrelated modifications or opportunistic changes must not be included
- A **code-freeze date** shall be established prior to activation

---

## SIP Versioning and Replacements

### Replacement Model

All SIPs (except SIP-000) adopt a **Replacement Model**:

- When a SIP is superseded, add to the old SIP's preamble: `Superseded-By: SIP-XYZ`
- The new SIP must include in its preamble: `Replaces: SIP-XYZ`
- The replacing SIP must contain the **complete, definitive text** (not just a list of changes)

### SIP-000 Special Case

SIP-000 (the process document) uses **version increments** instead:
- SIP-000-1, SIP-000-2, etc.
- Each version shall contain the complete text

---

## Questions?

If you have questions about the SIP process:

- Review existing SIPs and discussions for examples
- Open a discussion in the repository
- Reach out to SIP Editors for guidance
- Visit the SIP forum category https://forum.stacks.org/c/sip/65

---

## Compensation

Compensation for committee participation is outside the scope of this document. This document neither creates provisions for nor forbids compensation for SIP-related work.

