

# Preamble

SIP: 000-1  
Title: Stacks Improvement Proposal Process  
Author: Claire Gadd <claire@stacks.org>, HeroGamer, Jesse Wiley <jwiley@stacks.org>
Contributors: Jude Nelson jude@stacks.org, Ken Liao yukanliao@gmail.com
Status: Draft  
Consideration: Governance  
Type: Meta  
Created: 2025-10-22  
License: BSD-2-Clause  
Discussions-To: https://github.com/stacksgov/sips/issues/228  
Replaces: SIP-000  


# Abstract

A Stacks Improvement Proposal (SIP) is a design document that provides information to Stacks ecosystem participants concerning the design and ongoing operation of the Stacks blockchain. Each SIP must provide a clear and concise description of features, processes, and/or standards for the Stacks blockchain and its operators to adopt, with sufficient detail for a reasonable practitioner to create an independent but compatible implementation of the proposed improvement.

SIPs are the primary mechanism by which new features are proposed and described, and by which input from Stacks participants is collected. A SIP is expected to document *what* change is being proposed, *why* it is needed, and *how* it should be activated or implemented, so that the evolution of Stacks remains transparent, reviewable, and grounded in verifiable consensus.

Because SIPs are maintained as text files in a version-controlled repository, their revision history forms the canonical record of protocol and governance design decisions.

# License and Copyright

This SIP is made available under the terms of the BSD-2-Clause license, available at https://opensource.org/licenses/BSD-2-Clause. This SIP’s copyright is held by the Stacks Open Internet Foundation.

# What is a SIP?

A Stacks Improvement Proposal (SIP) is the standard process for proposing changes to the Stacks blockchain and its surrounding processes.

SIPs exist to ensure that changes to Stacks are:

- **Transparent**: proposals, rationale, and dissent are visible to the ecosystem.
- **Reviewable**: proposals can be discussed, critiqued, and iterated on in public.
- **Technically sound**: proposals meet minimum standards for clarity, completeness, and safety.

SIPs are required for any change that affects:

- Consensus rules or protocol behavior.
- Core standards or interoperability guarantees.
- Governance processes, decision-making structures, or SIP workflow itself.
- Other cross-ecosystem processes that need durable documentation and
  predictable activation.

Routine engineering work (bug fixes, minor refactors, non-standardized feature ) does not require a SIP and should be handled via the relevant repository’s issue tracker and contribution workflow.

This specification also defines the roles involved in SIP governance—including SIP Editors, Consideration Advisory Boards (CABs), and the Steering Committee—and the responsibilities those groups hold in maintaining fairness, consistency, and transparency.

Once ratified, a SIP becomes part of Stacks’ canonical technical and governance documentation and may guide future upgrades and design decisions.

---

# What belongs in a successful SIP?

Each SIP should contain the following parts, in the approximate order:

## Preamble

Structured metadata describing the SIP (number, title, authors, status, consideration, type, created date, license, sign-off, dependencies, etc.).

## Abstract

A short ( `~100–200` word) overview of the problem and proposed solution.

## Copyright / Licensing

A concise statement of the SIP’s license that references an approved license.(See [SIP Copyright and Licensing](#sip-copyright-and-licensing)).

## Summary / Motivation  

A clear description of:
- The problem(s) the SIP aims to solve.
- Why existing specifications or processes are insufficient.
- High-level goals and non-goals.

## Specification

The normative technical or process description. This section must be detailed enough to:
- Enable interoperable implementations, and/or
- Provide a clear, testable governance/process change.

## Rationale
Explanation of key design decisions, tradeoffs, and rejected alternatives. This section should reference Related Work where applicable and reflect community feedback and concerns.

## Backwards Compatibility
Discussion of incompatibilities or migration concerns, including:
- Impact on existing nodes, contracts, tools, or governance processes.
- Mitigations or migration paths.
- An explicit statement if no backwards compatibility concerns exist.

## Activation
A precise description of activation conditions, including:
- Timeline and phases, if any.
- Off-chain and/or on-chain signals required.
- How acceptance or rejection is objectively determined.

## Reference Implementation(s)
Links to production-quality implementations, where applicable. This may be added or updated after the SIP is ratified.

## Security Considerations (_if applicable_)
A discussion of relevant threat models, risks, and mitigations.

## Related Work / References
See “Related Work” section below.

Additional sections may be included as needed, provided the main structure remains recognizable and consistent.

# SIP Formats and Templates

All SIPs MUST be written in Markdown. Sections should use second-level headers (`##`) and deeper headers for subsections.

To encourage consistency:

- New SIPs should follow the official SIP template file (https://github.com/stacksgov/sips/blob/main/sips/SIP_TEMPLATE.md).
- Code blocks, diagrams, and tables should use standard Markdown constructs.
- External references (papers, repos, specifications) should be included in a "Related Work" or "References" section and, where possible, mirrored or backed up in the SIP repository if licensing allows.

# SIP Header Preamble

Each SIP begins with an RFC 822 style header preamble. The headers MUST appear in the following general order.
Required:

- SIP: SIP number will be assigned later by SIP Editors
- Title: Short descriptive title
- Author: List of SIP authors
- Status: Draft
- Consideration: One or more considerations, e.g. Governance, Consensus, Economics
- Type: One of: Consensus-Hard-Fork | Consensus-Soft-Fork | Meta | Informational
- Created: Date in ISO 8601 format (`YYYY-MM-DD`)
- License: One or more approved licenses (see [SIP Copyright and Licensing](#sip-copyright-and-licensing))

_Optional but recommended:_
- Contributor: Comma separated list of authors’ real names and optionally email addresses
- Discussions-To: Link(s) to any relevant external discussion
- Requires: Comma-separated list of SIP numbers this SIP depends on
- Replaces: SIP number(s) that this SIP replaces
- Superseded-By: SIP number(s) that supersede this SIP
- License-Code: License for code snippets if different from text

Authors should include an email address if they are willing to receive direct feedback. The format of an Author line **with** an email address is:

```text
Random J. User <address@domain.tld>
```


## SIP Considerations

A SIP's consideration determines the particular steps needed to ratify the SIP and incorporate it into the Stacks blockchain. Different SIP considerations have
different criteria for ratification. A SIP can have more than one consideration,
since a SIP may need to be vetted by different users with different domains of
Expertise ([committees.md](./committees.md))


## SIP Types

Consensus change SIPs will typically require reference implementations and carefully specified activation procedures. _Meta_ and _Informational_ SIPs focus more on process clarity and guidance.

There are several kinds of SIPs, analogous to BIP types but tailored to Stacks:

### Consensus – Hard Fork 

Proposes changes to consensus rules that require all Stacks full nodes and implementations to upgrade in order to remain compatible. These SIPs must clearly specify the affected layer(s) and activation criteria.

### Consensus – Soft Fork 

Proposes changes that restrict or refine consensus behavior in a way that is forward-compatible for upgraded nodes, but may impose new validity constraints. These SIPs also specify the affected layer(s) and activation conditions.

### Meta

Describes processes around Stacks rather than protocol rules themselves. This includes changes to the SIP process, governance workflows, committee structures, or tooling. Meta SIPs often require broad community consensus and are not purely advisory.

### Informational

Documents best practices, design notes, or general information relevant to the Stacks ecosystem, but does not mandate changes. Informational SIPs do not necessarily represent consensus and may be ignored or superseded by practice.


## Public Venues for Conducting Business

The canonical set of SIPs in any state shall be recorded in the same medium where the canonical copy of this SIP is.  Presently, this is in the Github repository `https://github.com/stacksgov/sips` but may be changed in the future.

In addition, individual committees may set up and use public mailing lists or other for conducting business.  The Stacks Open Internet Foundation shall provide a means for doing so, and any discussion thereof that lead to non-trivial contributions to a SIP should be referenced by the SIP as supplemental Material

## SIP Copyright and Licensing
Each SIP must identify at least one acceptable license in its preamble. Source code in the SIP  may be licensed differently than the text. SIPs whose reference implementation(s) touch existing  reference implementation(s) must use the same license as the existing implementation(s) in order  to be considered. Below is a list of recommended licenses.
- BSD-2-Clause: OSI-approved BSD 2-clause license
- BSD-3-Clause: OSI-approved BSD 3-clause license
- CC0-1.0: Creative Commons CC0 1.0 Universal
- GNU-All-Permissive: GNU All-Permissive License
- GPL-2.0+: GNU General Public License (GPL), version 2 or newer
- LGPL-2.1+: GNU Lesser General Public License (LGPL), version 2.1 or newer


# Related Work

The governance process proposed in this SIP is inspired by the Python PEP
process [1], the Bitcoin BIP2 process [2], the Ethereum Improvement Proposal [3]
processes, the Zcash governance process [4], and the Debian GNU/Linux
distribution governance process [5].  This SIP describes a governance process
where top-level decision-making power is vested in a committee of elected
representatives, which distinguishes it from Debian (which has a single elected
project leader), Python (which has a benevolent dictator for life), and Bitcoin
and ZCash (which vest all decision ratification power solely in the blockchain
miners).  The reason for a top-level steering committee is to ensure that
decision-making power is not vested in a single individual, but also to ensure
that the individuals responsible for decisions are accountable to the community
that elects them (as opposed to only those who have the means to participate
in mining).  This SIP differs from Ethereum's governance
process in that the top-level decision-making body (the "Core Devs" in Ethereum,
and the Steering Committee in Stacks) is not only technically proficient to evaluate
SIPs, but also held accountable through an official governance
process.

[1] https://www.python.org/dev/peps/pep-0001/

[2] https://github.com/bitcoin/bips/blob/master/bip-0002.mediawiki

[3] https://eips.ethereum.org/

[4] https://www.zfnd.org/governance/

[5] https://debian-handbook.info/browse/stable/sect.debian-internals.html

# Backwards Compatibility

Not Applicable.

# Activation

This SIP activates once following tasks have been carried out:
- All existing CABs have approved the changes herein

# Reference Implementation

Not applicable.
