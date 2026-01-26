# SIP Activation Voting
TODO - fill in details on how votes are to happen in a standardized way for each type of SIP (as a minimum - a sup may choose to be more restrictive or longer etc). 

The types of votes should align with types of SIPs. 

### Consensus (Hard Fork) SIPs

Consensus (hard fork) SIPs introduce backward-incompatible changes and require explicit ecosystem coordination.

- **Vote Type:** Mandatory public vote
- **Participants:** Token holders and/or a designated voting mechanism defined by the Steering Committee
- **Minimum Voting Period:** 2 weeks
- **Approval Threshold:** Supermajority (e.g., ≥ 80% approval)
- **Additional Requirements:**
  - CAB approval is required before the vote may begin
  - A clear activation height must be specified
  - A post-vote buffer period must exist before activation

Failure to meet the approval threshold results in rejection and shall require resubmission as a new SIP.


### Consensus (Soft Fork) SIPs

- **Vote Type:** Mandatory CAB vote
- **Approval Threshold:** Voting criteria defined by CAB
- **Additional Requirements:**
  - Clearly defined SIP activation criteria (ex: SIP is considered ratified if `n+1` wallet providers implement this proposal)

### Informational SIPs
- **Vote Type:** Mandatory CAB vote
- **Approval Threshold:** Voting criteria defined by CAB
- **Additional Requirements:**
  - Clearly defined SIP activation criteria

### Meta SIPs
- **Vote Type:** Mandatory CAB vote
- **Approval Threshold:** Voting criteria defined by CAB
- **Additional Requirements:**
  - Clearly defined SIP activation criteria
