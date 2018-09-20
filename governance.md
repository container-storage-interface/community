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

Voting on a motion must happen on the [community mailing list](https://groups.google.com/forum/#!forum/container-storage-interface-community).

A motion can be one of the following:
* Package releases
* Procedural issues

### Voting Window

Voting on each motion must specify a time window when voters can vote, starting from the time when the motion is posted on the [mailing list](https://groups.google.com/forum/#!forum/container-storage-interface-community).
Any vote made outside the time window will not be considered.
Votes should be permitted to run for at least 72 hours to provide an opportunity for all concerned persons to participate regardless of their geographic locations.
Votes must not run more than 1 week.

### Expressing Votes

Votes are represented as numbers:
* `+1` means 'yes'
* `-1` means 'no'

Any `-1` vote must include a list of concerns or links to written documentation for those concerns (e.g. GitHub issues or mailing-list threads).

### Binding Votes

Votes from [approvers](#community-membership) are binding.
Other members are encouraged to vote, even if their votes are only advisory.

### Passing Criteria

A proposed motion is considered adopted when it receives `+1` from more than half of the voters that have binding vote privilege and receives no `-1` binding vote.

If there is any `-1` binding vote, the proposed motion is considered adopted only if it receives `+1` from more than 2/3 of the voters that have binding vote privilege.

### Subject Templates

Each proposed motion should use the following subject templates.

#### Proposing a motion

`[VOTE] {Motion Description} (closes {the End of the Voting Window})`

The end of the voting window should be in YYYY-MM-DD hh:mm (ISO 8601) with UTC timezone to avoid ambiguity.

#### Tallying results

`[VOTE RESULT]: {Motion Description}`

## Pull Request Rot

| Term | Definition | Synopsis |
| ---- | ---------- | -------- |
| Stale | PR has been inactive for 90+ days. | PRs will be labeled as "stale". An inactive, stale PR may be marked "rotten" after 30 days. |
| Rotten | Stale PR has been inactive for 30+ days. | PRs will be labeled as "rotten". An inactive, rotten PR may be closed after 30 days of being marked "rotten". |

The process of marking PRs as *stale* or *rotten* is currently a manual one.
In the future this process will be automated.
