# Basic Bylaws for a Consideration Advisory Board
_Note_: the original source of this document is here: https://gist.github.com/jcnelson/3fcc635ede20ce98d1eae60941eb127a

This document provides an initial set of bylaws for starting a Consideration Advisory Board.  It can serve as the bylaws for the CAB indefinitely, or it can be replaced later if the CAB's members devise better ones.

## Overview

Per [SIP-000](https://github.com/stacksgov/sips/blob/main/sips/sip-000/sip-000-stacks-improvement-proposal-process.md), each consideration advisory board (CAB) has a lot of leeway in deciding how it conducts its business.  In particular, SIP-000 only imposes the following responsibilities on the CAB:

* The CAB needs a **chairperson** that the SIP Steering Committee (SC) can reach to coordinate SIP ratification.

* The CAB needs a **description** of its consideration, which needs to be detailed enough that it's clear to a SIP author wether or not their SIP falls within their purview.

* The CAB needs to **review Accepted SIPs** in a timely fashion, ultimately providing a recommendation to advance or reject the SIP.  This review needs to be public, and must provide actionable feedback to the SIP authors so that they can get their SIP ready for activation or resubmission.

## Picking the First Chairperson

There are two ways a CAB can be instantiated:

* It was instantiated by a SIP submitted by an unofficial working group, or

* It was instantiated by SIP-000

In the first case, the chairperson needs to be chosen prior to the CAB-creation SIP being activated -- the SC can require that a choice be made as part of its activation criteria, for example.  The second case was left unspecified in SIP-000.

To pick the first chairperson for a CAB instantiated by SIP-000 (which today includes all CABs), members of the CAB whose names are listed in the CABs' respective CAB definition file (found [here](https://github.com/stacksgov/sips/tree/main/considerations)) will attempt the following selection procedures, in this order:

1. The chairperson is the first person who volunteers for the job within 10 days of this document being adopted, with the acquiescence of the other members.  For example, the governance CAB has used this procedure to pick its chairperson.

2. If the above fails, then the CAB members will vote amongst themselves to pick a chairperson.  They will do so within 10 days of accepting this document.  The chairperson shall be the person who receives a majority vote from of all members.  Members may abstain from voting, or may be absent.

3. If the above fails, then the chairperson will be the person whose listed email address, when SHA256-hashed with the filename of the CAB definition file, is alphanumerically the lowest such hash.  For example:

```bash
$ echo -n 'jude@stacks.org technical.md' | sha256sum
617c226866d78e54db531252c5979bc9d15505e5c3f4a67f2a76b99b02c5b071 -
```

The SC will use option #3 to pick the first chairperson after 10 days of this document being adopted by the CAB, if a chairperson cannot be found with options #1 and #2.

## Chairperson Duties

The chairperson only needs to do the following:

* Sign off on the CAB's official review of a SIP.  They don't need to write it themselves; they just need to approve it.  It will be uploaded to the [minutes](https://github.com/stacksgov/sips/tree/main/considerations/minutes) directory.

* Help resolve any review conflicts within the CAB.  If they cannot do so, then they need to bring them to the attention to the SC.  A Github comment on the SIP pull request is sufficient for doing this, as long as it @-mentions one of the SC members.

* Attend the weekly SIP call (Fridays at 11am US Eastern), or make sure a substitute CAB member will do so, or inform the SC that no one can come.

The chairperson can assume more responsibilities if they wish.  The SC will otherwise handle the SIP shepharding processes, including reaching out to CAB members to get their reviews, drafting the official review response, and moving SIPs from Accepted to Recommended.

## Chairperson Tenure

A CAB chairperson will only serve for one quarter.  A new chairperson will be selected at the start of each quarter, via chairperson selection rules #1 or #2 above.

If the CAB does not choose a new chairperson by the time the next quarter starts, then the SC will select the chairperson by choosing the CAB member whose email and CAB definition filename hash alphanumerically follows the last chairperson's hash.  If the current chairperson's hash is the last hash in alphanumeric order, then the next chairperson will be the person whose hash is alphanumerically first.  In this manner, each CAB member would take turns acting as the chairperson in a round-robin fashion, in hash-order, with wrap-around.

For example:

```bash
$ echo -n 'alice@stacks.org technical.md' | sha256sum
e47a11ebae09424bc866ace5b006448d792e454a2739ef1e480aab2a589d84e1 -
$ echo -n 'bob@stacks.org technical.md' | sha256sum
ccc0207d2a40cbd9b3a30e9779c8802b2799250fcd7c9bd490b71451de5b377d -
$ echo -n 'charlie@stacks.org technical.md' | sha256sum
f4ef64ded7c5dea061d421073ef994d023d73ac637276b9742d91b39454574d5 -
```

If the CAB does not ever choose a chairperson, then `bob@stacks.org` would be the first chairperson.  He would be succeeded by `alice@stacks.org`, and she would be succeeded by `charlie@stacks.org`.  After he finishes his tenure, `bob@stacks.org` would be the chairperson again.

## CAB Member Duties

A CAB member only needs to comment on a SIP under review, via Github comments on the SIP pull request.  If they cannot do so in a timely fashion, the SC will move to have their review dropped so as to unblock a SIP that has otherwise received adequate feedback.  The SC will declare this decision publicly as a Github comment on the SIP pull request.  Unless informed otherwise by the CAB chairperson, or stated in the CAB bylaws, the SC shall decide what "timely fashion" and "adequate feedback" mean for a SIP on a case-by-case basis.

## CAB Member Tenure

Beyond abiding by the rules in SIP-000, a CAB member is a member of the CAB until they explicitly resign.  They can do so by informing the SC via email.

If a CAB member becomes unresponsive, then per the preceding section, the SC shall declare that their review on an in-scope SIP will not be required or considered.

## Amending or Replacing these Bylaws

The CAB can ammend these bylaws by a majority vote.  Any new sections will be added to the `Amendments` section at the end of this document, submitted via a pull request.  Amendments may supercede any part of this document, or even replace it entirely.

The individuals who voted to amend or replace this document must be publicly recorded as part of the proposed amendment.  The SC will reach out to these individuals to confirm their vote to make the change.

## Amendments

This section will contain a CAB's amendments.
