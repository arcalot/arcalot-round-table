# Arcalot Round Table Charter

Arcalot is a **free, open source collection of projects, and will remain so**. Our main mission is to improve the way workloads are run, how their data is consumed and forwarded, and to simplify analyzing the output of workloads, debugging where necessary.

This charter covers **important processes and decisions that impact the whole organization, direction, and goals**. Small decisions like coding style per repository or similar details can be decided among the repository maintainers.

## Arcalot Round Table

The Arcalot Round Table *(ART)* consists of:
* 4 chairs with equal rights who
  - Enforce the [Code of Conduct](https://github.com/arcalot/.github/blob/main/CODE_OF_CONDUCT.md)
  - Have administrative rights over the [GitHub org](https://github.com/arcalot), communication channels, and other community-owned resources
  - Publicly record decisions made by the ART in the [`art-decisions`](art-decisions) folder
* Individuals who want to join the ART and pass a review of their PR sent to [ART_MEMBERS.md](ART_MEMBERS.md), with approval depending on any one or more of the below requirements:
  - They contribute with code, documentation, artwork, articles, videos, talks, or similar additions to the Arcalot ecosystem
  - They are an active user of Arcalot projects (end user, product builder, researcher, etc. - please describe your use case in the PR, you do not have to mention any company names or details)
  - They are actively helping community members on any of the official Arcalot channels

### ART Participation

Meetings do not count as necessary round table matters as we want to include people in all stages of life and across all timezones. We therefore refrain from any synchronous or undocumented decision making.

Additionally, as stated in the [Arcalot Code of Conduct](https://github.com/arcalot/.github/blob/main/CODE_OF_CONDUCT.md), chairs can remove an ART member if their behavior is clearly disruptive to the community.


### Chair Participation

Chairs are expected to remain actively involved in the community. An Arcalot Round Table chair that does not participate in round table matters (voting) *without reason and notice* for 3 times in a row leaves the chairs automatically as we can assume they are not interested in the responsibilities of the chair position anymore.


## Decision Proposals

Decisions can be started *only asychronously* in the [ART repository pull requests](https://github.com/arcalot/arcalot-round-table/pulls) via submitting a pull request with a new file to [`art-decisions/proposals`](art-decisions/proposals). You can use the included [template file](art-decisions/proposals/template.md) as a guideline. Decision proposals can only be submitted by ART members. If you would like to encourage discussion around a decision before any voting starts, please submit a draft PR instead and mark it ready for review once you are comfortable that you will not add any changes to your proposal.

## Voting

Each member of the Arcalot Round Table is eligible for voting if they have been a member of the ART for at least 30 days. For any decision that impacts the whole project or processes, a vote is started where a minimum of 4 votes is required with 75% approval majority among the voters.

If the majority cannot be reached, the proposal is considered rejected and can be brought to the ART again 1 month after the rejection at the earliest. If the same decision has been rejected twice, it cannot be brought to the ART again.

Any voting period must last at least 7 calendar days to account for different time zones and other obligations and should last no longer than 30 days. The voting period should be stated in the proposal. Proposals can be extended no more than twice and for no longer than 30 days total. Extensions can be made by the original submitter, their direct representative, or one of the ART chairs by updating the PR with a note stating the number of calendar days for the extension.

ART members cast their votes by starting a review that either approves or rejects the decision suggested via a pull request. A reject vote is recorded by using the *Request changes* function of the PR review. Once the voting period is over or all ART members have voted, the chairs record the decision, objections, and other relevant information in the [`art-decisions` folder](art-decisions). Silence equals abstaining from a vote.

## Chair Elections

If a chair leaves through non-participation or through their own announcement, elections for a new chair take place.

After the announcement of a chair leaving, there is a period of 30 days for nominations (from the date of the announcement). Any ART member can nominate another ART member or themselves, while a second member has to sponsor the nomination. Only members that have been part of the ART for 6+ months are eligible to become a chair or sponsor a nomination.

After the nomination period, elections take place asynchronously through the same process as standard decision proposals.

## Code of Conduct Enforcement

Removing or disciplining an ART member due to a violation of the [Arcalot Code of Conduct](https://github.com/arcalot/.github/blob/main/CODE_OF_CONDUCT.md) is performed by the chairs as a pull request to the ART. Only the the chairs vote on these matters, with an approval by 75% of the active chairs required for the matter to pass.

## Changing the Charter

This charter can be changed by a pull request passing the same threshold of voting as any other proposal and additionally can have no more than 1 dissenting vote from an active chair.
