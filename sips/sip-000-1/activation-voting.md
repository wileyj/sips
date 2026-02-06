# SIP Activation 

## Voting Requirements

| SIP Type              | Vote Type             | Participants | Minimum Voting Period | Approval Threshold                   | Additional Requirements |
| :---------------------| :-------------------- | :----------- | :-------------------- | :----------------------------------- | :---------------------- |
| Meta                  | Mandatory CAB vote    | CAB Members  | N/A                   | Voting criteria defined by CAB       | None |
| Informational         | Mandatory CAB vote    | Cab Members  | N/A                   | Voting criteria defined by CAB       | None |
| Consensus (Soft Fork) | Mandatory CAB vote    | CAB Members  | N/A                   | Voting criteria defined by CAB       | None |
| Consensus (hard fork) | Mandatory public vote (See the exceptions section below) | Token holders and/or a designated voting mechanism defined by the Steering Committee | 1 Stacking cycle (~ 2 weeks) | Supermajority (e.g., ≥ 80% approval) | <ul><li>CAB approval is required before the vote may begin</li><li>A clear activation height must be specified</li><li>A post-vote buffer period must exist before activation</li></ul> |

### Exceptions to the Consensus (hard fork) public vote requirement

In some cases, there may be an applicable exception to the mandatory public vote requirement for a Consensus (hard fork) SIP type. These exceptions should be clearly identified in the Activation section of the SIP (see [sip-000-1-stacks-improvement-proposal-process.md](./sip-000-1-stacks-improvement-proposal-process.md#activation)).  
Some examples to this exception include:

- A hard fork that adds a new feature, but the feature is _opt in_ and only affects users who choose to use it. For example, a new Clarity function that does not affect existing functionality. 
- Bug fixes to modify incorrectly implemented behaviour should only require a CAB vote under the following conditions:
    - The SIP proposing the correction identifies an existing required SIP in the preamble. i.e. `Requires: SIP-xyz`, where `SIP-xyz` contains the implementation that needs to be corrected. 


## SIP Activation Requirements

ALL SIPs are required to have a clearly defined activation criteria. 

Example:
- SIP is considered ratified if `n+1` wallet providers implement this proposal)

_Failure to meet the approval threshhold_ results in the SIP being rejected and shall require re-submission as a new SIP
