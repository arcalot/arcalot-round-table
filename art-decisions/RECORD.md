# Record of ART Decisions

This file keeps a record of all decisions made by the Arcalot Round Table and might be split over time as the ART continues.

## Promotion Jared O'Connell to Chair

**Date: 2023-04-17**

Janos Bonic has stepped down as an Arcalot chair, and Jared O'Connel has been nominated and approved to replace him.

- Pull request: [#32](https://github.com/arcalot/arcalot-round-table/pull/32)
- Proposal: [proposals/2023-03-20-janos-chair-election.md](proposals/2023-03-20-janos-chair-election.md)

### Voted in favor:

* [@sandrobonazzola](https://github.com/sandrobonazzola)
* [@dustinblack](https://github.com/dustinblack)
* [@tsebastiani](https://github.com/tsebastiani)
* [@AvlWx2014](https://github.com/AvlWx2014)
* [@engelmi](https://github.com/engelmi)
* [@HubertStefanski](https://github.com/HubertStefanski)
* [@Harshith-umesh](https://github.com/Harshith-umesh)
* [@jaredoconnell](https://github.com/jaredoconnell)
* [@jdowni000](https://github.com/jdowni000)
* [@mfleader](https://github.com/mfleader)

### Voted against:

* *None*

## Expansion of Workflow Expression Language

**Date: 2023-04-03**

The current state of the expression language allows users to retrieve values from inputs and step output. That is enough for usable workloads, but is insuffient for many use cases. This proposal will make it so less manual work is required to get a workflow working.

- Pull request: [#31](https://github.com/arcalot/arcalot-round-table/pull/31)
- Proposal: [proposals/2023-03-14-expressions-expansion.md](proposals/2023-03-14-expressions-expansion.md)

### Voted in favor:

* [@sandrobonazzola](https://github.com/sandrobonazzola)
* [@lmilbaum](https://github.com/lmilbaum)
* [@dustinblack](https://github.com/dustinblack)
* [@tsebastiani](https://github.com/tsebastiani)
* [@HubertStefanski](https://github.com/HubertStefanski)
* [@Harshith-umesh](https://github.com/Harshith-umesh)
* [@jdowni000](https://github.com/jdowni000)
* [@mfleader](https://github.com/mfleader)
* [@janosdebugs](https://github.com/janosdebugs)

### Voted against:

* *None*

## Rename Carpenters repository to `arcalot/arcaflow-container-toolkit`

**Date: 2023-03-21**

This change will separate the tool from the plugins and pave way for a much clearer readme.md file. This will simplify the entrypoint for new users to the tool and cause less confusion in the documentation with naming convention as well as usage.

Also I believe it would be a good time to move the reusable workflow file from [arcaflow-reusable-workflows](https://github.com/arcalot/arcaflow-reusable-workflows/blob/main/.github/workflows/carpenter.yaml), into the carpenter project itself. This will centralize the project and keep everything carpenter, with carpenter.

- Pull request: [#30](https://github.com/arcalot/arcalot-round-table/pull/30)
- Proposal: [proposals/2023-03-09-carpenter-repository-rename.md](proposals/2023-03-09-carpenter-repository-rename.md)

### Voted in favor:

* [@sandrobonazzola](https://github.com/sandrobonazzola)
* [@lmilbaum](https://github.com/lmilbaum)
* [@dustinblack](https://github.com/dustinblack)
* [@tsebastiani](https://github.com/tsebastiani)
* [@HubertStefanski](https://github.com/HubertStefanski)
* [@Harshith-umesh](https://github.com/Harshith-umesh)
* [@jaredoconnell](https://github.com/jaredoconnell)
* [@mfleader](https://github.com/mfleader)
* [@janosdebugs](https://github.com/janosdebugs)

### Voted against:

* *None*

## Adding signals to the Arcaflow execution model

**Date: 2023-01-23**

In this proposal, we transform the execution of Arcaflow by adding the ability to send and receive signals via signal channels. Each signal channel will have a schema and is declared by a plugin. Workflow authors can take these signals and pipe them into other plugins that have declared they can receive signals.

- Pull request: [#24](https://github.com/arcalot/arcalot-round-table/pull/24)
- Proposal: [proposals/2022-11-20-arcaflow-signals.md](proposals/2022-11-20-arcaflow-signals.md)

### Voted in favor:

* [@dustinblack](https://github.com/dustinblack)
* [@jaredoconnell](https://github.com/jaredoconnell)
* [@sandrobonazzola](https://github.com/sandrobonazzola)
* [@tsebastiani](https://github.com/tsebastiani)
* [@AvlWx2014](https://github.com/AvlWx2014)
* [@HubertStefanski](https://github.com/HubertStefanski)
* [@Harshith-umesh](https://github.com/Harshith-umesh)
* [@jdowni000](https://github.com/jdowni000)

### Voted against:

* *None*

## Standardize on python code formatting requirements

**Date: 2022-11-04**

Standardize on python code formatting requirements for official Arcaflow contributions.

- Pull request: [#16](https://github.com/arcalot/arcalot-round-table/pull/16)
- Proposal: [proposals/2022-10-26-standardize-python-formatting.md](proposals/2022-10-26-standardize-python-formatting.md)

### Voted in favor:

* [@jaredoconnell](https://github.com/jaredoconnell)
* [@sandrobonazzola](https://github.com/sandrobonazzola)
* [@portante](https://github.com/portante)
* [@mkarg75](https://github.com/mkarg75)
* [@Harshith-umesh](https://github.com/Harshith-umesh)
* [@jdowni000](https://github.com/jdowni000)
* [@mfleader](https://github.com/mfleader)

### Voted against:

* *None*

## Standardize python projects on poetry

**Date: 2022-11-04**

Standardize on the use of [poetry](https://python-poetry.org/) for dependency management a packaging for all python projects.

- Pull request: [#15](https://github.com/arcalot/arcalot-round-table/pull/15)
- Proposal: [proposals/2022-10-26-standardize-on-poetry.md](proposals/2022-10-26-standardize-on-poetry.md)

### Voted in favor:

* [@dustinblack](https://github.com/dustinblack)
* [@sandrobonazzola](https://github.com/sandrobonazzola)
* [@portante](https://github.com/portante)
* [@mkarg75](https://github.com/mkarg75)
* [@Harshith-umesh](https://github.com/Harshith-umesh)
* [@jaredoconnell](https://github.com/jaredoconnell)
* [@jdowni000](https://github.com/jdowni000)
* [@mfleader](https://github.com/mfleader)
* [@janosdebugs](https://github.com/janosdebugs)

### Voted against:

* *None*

## Nomination of Peter Portante as chair

**Date: 2022-10-11**

Nomination of [Peter Portante](https://github.com/portante) as a Chair of Arcalot to replace [Sanja Bonic](https://github.com/sanjacodes).
- 
- Pull request: [#9](https://github.com/arcalot/arcalot-round-table/pull/9)
- Proposal: [proposals/2022-10-05-chair-nomination-peter-portante.md](proposals/2022-10-05-chair-nomination-peter-portante.md)

### Voted in favor:

* [@sanjacodes](https://github.com/sanjacodes)
* [@sandrobonazzola](https://github.com/sandrobonazzola)
* [@janosdebugs](https://github.com/janosdebugs)
* [@mkarg75](https://github.com/mkarg75)
* [@jaredoconnell](https://github.com/jaredoconnell)
* [@Harshith-umesh](https://github.com/Harshith-umesh)
* [@dustinblack](https://github.com/dustinblack)
* [@jdowni000](https://github.com/jdowni000)

### Voted against:

* *None*

## Propose exception for early chair nominations

**Date: 2022-10-05**

> The [Arcalot Charter](https://github.com/arcalot/arcalot-round-table/blob/main/CHARTER.md#chair-elections) mandates a 6 months minimum membership for chair nominations, but the Arcalot organization is less than 6 months old, therefore this proposal is making **any Arcalot member as of the 4th of October 2022 eligible to become an Arcalot Chair** for this election only. In light of the rule change for chair voting, this proposal is open for voting using pull request reviews **until the 12th of October**.

- Pull request: [#7](https://github.com/arcalot/arcalot-round-table/pull/7)
- Proposal: [proposals/2022-10-05-chair-election-exception.md](proposals/2022-10-05-chair-election-exception.md)

### Voted in favor:

* [@sanjacodes](https://github.com/sanjacodes)
* [@sandrobonazzola](https://github.com/sandrobonazzola)
* [@jaredoconnell](https://github.com/jaredoconnell)
* [@jdowni000](https://github.com/jdowni000)
* [@mfleader](https://github.com/mfleader)
* [@janosdebugs](https://github.com/janosdebugs)
* [@dustinblack](https://github.com/dustinblack)
* [@Harshith-umesh](https://github.com/Harshith-umesh)

### Voted against:

* *None*

