# Arcalot Round Table Charter

Arcalot is a **free and open source collection of projects and will remain so**. Our
main mission is to improve the way workloads are run, how their data is consumed and
forwarded, and to simplify analyzing the output of workloads.

This charter covers **important processes and decisions that impact the whole
organization, its direction, and its goals**. Small decisions like coding style per
repository or similar details can be decided among the repository maintainers.

## Arcalot Round Table

The Arcalot Round Table (ART) consists of:
* Four chairs with equal rights who
  - Enforce the [Code of
    Conduct](https://github.com/arcalot/.github/blob/main/CODE_OF_CONDUCT.md)
  - Have administrative rights over the [GitHub org](https://github.com/arcalot),
    communication channels, and other community-owned resources
  - Publicly record decisions made by the ART in the [`art-decisions`](art-decisions)
    folder
* Individuals who
  - Contribute with code, documentation, artwork, articles, videos, talks, or similar
    additions to the Arcalot community
  - Are users of Arcalot projects (end users, product builders, researchers, etc.)
  - Help community members on any of the official Arcalot channels

### ART Participation

If you wish to join the ART, please submit a pull request adding yourself to the
[`ART_MEMBERS.md`](ART_MEMBERS.md) file. Please describe your use case in the pull
request comments; you do not need to mention any company names or details. Joining is
finalized upon two pull request approvals by the chairs and the merging of the pull
request.

Community meetings are not compulsory as we want to include people in all stages of life
and across all timezones. We therefore refrain from any synchronous or undocumented
decision making.

As stated in the [Arcalot Code of
Conduct](https://github.com/arcalot/.github/blob/main/CODE_OF_CONDUCT.md), chairs can
remove any ART member if their behavior is clearly disruptive to the community.


### Chair Participation

Chairs are expected to remain actively involved in the community. A chair who does not
participate in ART voting *without reason and notice* three times in a row forfeits the
position and becomes a regular ART member automatically.


## Proposals

Proposals may only be made asychronously by submitting a pull request to this repository
with a new file in the [`art-decisions/proposals`](art-decisions/proposals) directory.
The provided [template file](art-decisions/proposals/template.md) may be used as a
guideline for new proposals. The proposal file name should start with the date of the
initial draft of the proposal in YYYY-MM-DD format, followed by the proposal title in
all-lowercase with dashes substituting spaces (i.e., `2024-07-17-my-proposal-title.md`).
Proposals may only be submitted by current ART members. If you would like to encourage
discussion around a proposal before any voting starts, please submit a draft pull
request instead. Once the discussion is complete and you are comfortable that you will
not make any changes to your proposal, mark the pull request ready for review. Open pull
requests can be viewed at the [ART repository pull
requests](https://github.com/arcalot/arcalot-round-table/pulls) page.

## Voting

Each member of the ART is eligible to vote if they have been a member for at least 30
days. For any proposal that impacts the whole project or processes, **approval requires
a minimum of four votes with 75% approval among those voting**.

Any vote must be open for at least 7 calendar days to account for different time zones
and other obligations and must be open no longer than 30 days. The voting period must be
stated in the proposal in calendar days. The voting period begins on the day the pull
request is opened for review and ends at midnight after the last day of the voting
period, with all dates and times considered in UTC. Proposals can be extended for no
longer than 30 days total. Extensions can be made before the end of the current voting
period by the original submitter or one of the ART chairs by updating the pull request
with a note stating the number of calendar days for the extension. **If approval is not
reached within the voting period deadline, the proposal is rejected.**

Once rejected, a proposal may not be submitted again for 30 days.

ART members cast their votes by reviewing the pull request. An approval vote is cast by
approving the pull request, and a rejection vote is cast by using the *Request changes*
function and providing feedback in the comment regarding the reason for the rejection
and the changes they would like to see made. Once the voting period is over or all ART
members have voted, the pull request is merged into the `main` branch (always, whether
approved or rejected). The chairs then record the decision, dissenting comments, and
other relevant information in the [`RECORD.md`](art-decisions/RECORD.md) file via
another pull request that is reviewed and approved by at least 50% of the chairs to
ensure accuracy.

## Chair Elections

If a chair leaves through non-participation, through their own resignation, or due to an
incapacity to carry out their duties, elections for a new chair take place.

After the announcement of a chair leaving, there is a period of 30 days for nominations
(from the date of the announcement). Any ART member can nominate another ART member or
themselves, while a second member has to sponsor the nomination. Only members that have
been part of the ART for at least six months are eligible to become a chair or sponsor a
nomination.

After the nomination period, elections take place asynchronously through the same
process as standard proposals.

A proposal to remove a chair from their position for any reason other than those stated
at the beginning of this section follows the normal proposal process.

## Code of Conduct Enforcement

Removing or disciplining an ART member due to a violation of the [Arcalot Code of
Conduct](https://github.com/arcalot/.github/blob/main/CODE_OF_CONDUCT.md) is initiated
by any chair as a pull request to the ART. Only the chairs vote on these matters, with
an approval by a majority of the chairs voting in favor with none voting against. In the
case of a dissenting vote, consent is not achieved, and the matter moves to the normal
proposal process. An appeal may be made by any ART member or by the affected party via
the normal proposal process.

## Changing the Charter

This charter can be changed by a pull request passing the same threshold of voting as
any other proposal with the additional requirement of having no more than one rejection
vote from a chair.
