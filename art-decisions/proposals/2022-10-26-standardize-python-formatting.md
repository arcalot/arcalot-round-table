# Title

We should standardize on python formatting expectations. We should set one standard and adhere to it judiciously without exception. I recommend that we simply adopt the standards already established by the pbench organization and eliminate further debate on the topic. This formatting standard should also be applied wherever possible with automation and CI.

References:

[pbench .pre-commit-config.yaml](https://github.com/distributed-system-analysis/pbench/blob/main/.pre-commit-config.yaml)
[pbench pyproject.yaml](https://github.com/distributed-system-analysis/pbench/blob/main/pyproject.toml)
[pbench CI](https://github.com/distributed-system-analysis/pbench/blob/64364eeb2d027ce562da4861af9a588cc18a6d8d/build.sh#L27)

## Benefits

All python projects within Arcalot will follow an expected norm for formatting standards, simplifying readability and code reviews.

## Drawbacks

It's impossible to define one perfect standard the everyone loves. There will inevetibly be quirks to the formatting and disagreements from the community with the chosen approach.
