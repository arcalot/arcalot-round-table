# Use upstream renovate in replacement of Red Hat hosted version

As an amendment to proposal
[2023-03-08-automated-dependency-updates](2023-03-08-automated-dependency-updates.md),
the Arcalot organization will use the upstream
[Mend Renovate GitHub App](https://github.com/marketplace/renovate) service as the
primary means of automated dependency management and resolution rather than the
Renovate bot service hosted internally by Red Hat.

Implementing this change involves configuring the Renovate GitHub App to access all
repositories, and then removing the redhat-renovate-bot as a member of the Arcalot
organization. All other existing Renovate-related configurations can remain unchanged.
Some additional one-time maintenance of repos will also likely be required to remove
any unmerged changes from the existing Red Hat Renovate bot.

## Voting Period

The voting period for this proposal will be open for 7 days from its submission.

## Benefits

The upstream Renovate GitHub App is actively maintained by the community, it has proven
in testing to create more user-friendly PRs, and it may alleviate some troubles we have
seen with Go version compatibility. This change also provides more ongoing maintenance
reliability as we are currently unsure of the future support and maintenance of the
internally-hosted Renovate, and our goal is to minimize Arcalot maintenance efforts as
much as possible.

## Drawbacks

Our line of support may not be as direct as with the internally hosted version of
Renovate.
