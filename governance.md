# Governance

The Container Storage Interface is an independently run open-source project (independent of any single cluster orchestration system, any single storage vendor, etc).
It is proposed and maintained by members representing all major cluster orchestration (CO) systems (Kubernetes, Mesos, Docker, and Cloud Foundry).
Contributions from the community are are welcome and accepted via pull requests.

## Community Membership

| Role | Responsibilities | Requirements | Defined by |
| -----| ---------------- | ------------ | -----------|
| member | Active contributor in the community. | Sponsored by 2 reviewers.  Multiple contributions to the project. | CSI GitHub org member. |
| reviewer | Review contribution from other members. | History of review and authorship. | OWNERS file reviewer entry. |
| approver | Approve contributions for merge. | Core group of CO representatives. | OWNERS file approver entry. |
| janitor | Org and repo maintenance. | Minimal subset of approvers required for maintenance. | GitHub repo write access. |

While contributions are accepted from the community at large, to maintain impartiality and the benefit of end users, approvers for CSI are limited to just this core group of CO representatives.

## Voting

Voting on a motion must happen on the mailing list.

A motion can be one of the following:
* Package releases
* Procedural issues

### Voting Window

Voting on each motion must specifiy a time window when voters can vote.
Any vote made outside the time window will not be considered.
Votes should be permitted to run for at least 72 hours to provide an opportunity for all concerned persons to participate regardless of their geographic locations.

### Expressing Votes

Votes are represented as numbers:
* `+1` means 'yes'
* `-1` means 'no'

Any `-1` vote must include a list of concerns or links to written documentation for those concerns (e.g. GitHub issues or mailing-list threads).

### Binding Votes

Votes from [approvers](#community-membership) are binding.
Other members are encouraged to vote, even if their votes are only advisory.

### Passing Criteria

A proposed motion is adopted if:
* It receives `+1` from more than half of voters that have binding vote privilege.
* It receives no `-1` binding vote.

A proposed motion is considered rejected if any of the above condition is not met.

Any `-1` binding vote constitutes a veto and it cannot be overruled nor overridden by anyone. The veto stands until and unless withdrawn by their casters.

### Subject Templates

Each proposed motion should use the following subject templates.

#### Proposing a motion

`[VOTE] {Motion Description} (closes {the End of the Voting Window})`

#### Tallying results

`[VOTE RESULT]: {Motion Description}`
