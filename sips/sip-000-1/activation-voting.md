# SIP Activation 

## Voting Requirements

The types of votes should align with types of SIPs. 

| SIP Type              | Vote Type             | Participants | Minimum Voting Period | Approval Threshold                   | Additional Requirements |
| :---------------------| :-------------------- | :----------- | :-------------------- | :----------------------------------- | :---------------------- |
| Meta                  | Mandatory CAB vote    | CAB Members  | N/A                   | Voting criteria defined by CAB       | None |
| Informational         | Mandatory CAB vote    | Cab Members  | N/A                   | Voting criteria defined by CAB       | None |
| Consensus (Soft Fork) | Mandatory CAB vote    | CAB Members  | N/A                   | Voting criteria defined by CAB       | None |
| Consensus (hard fork) | Mandatory public vote | Token holders and/or a designated voting mechanism defined by the Steering Committee | 1 Stacking cycle (~ 2 weeks) | Supermajority (e.g., ≥ 80% approval) | <ul><li>CAB approval is required before the vote may begin</li><li>A clear activation height must be specified</li><li>A post-vote buffer period must exist before activation</li></ul> |

## SIP Activation Requirements

ALL SIPs are required to have a clearly defined activation criteria. 

Example:
- SIP is considered ratified if `n+1` wallet providers implement this proposal)

_Failure to meet the approval threshhold_ results in the SIP being rejected and shall require re-submission as a new SIP
