# Title

Standardize on python code formatting requirements

All Python code must conform to [PEP 8](https://peps.python.org/pep-0008), and
will be checked via the use of [`flake8`](https://github.com/PyCQA/flake8).

All Python imports will be required to be sorted and grouped according to [PEP
8](https://peps.python.org/pep-0008/#imports) using
[`isort`](https://github.com/PyCQA/isort).

All Python code (Python 3 assumed) will be required to be auto-formatted via
[`black`](https://github.com/psf/black).

A pre-commit hook will be offered for use to help verify the above
requirements before they go through the CI job.

The CI environment will include a series of checks to ensure the above
requirements are met using the following commands:

```
$ black --check .
$ isort --profile=black --check .
$ flake8 .
```

## Recommendation

We should set one standard and adhere to it judiciously without exception. I
recommend that we simply adopt the standards already established by the
[pbench](https://github.com/distributed-system-analysis/pbench) repository and
eliminate further debate on the topic. This formatting standard should also be
applied wherever possible with automation and CI.

References:

[pbench .pre-commit-config.yaml](https://github.com/distributed-system-analysis/pbench/blob/main/.pre-commit-config.yaml)
[pbench pyproject.yaml](https://github.com/distributed-system-analysis/pbench/blob/main/pyproject.toml)
[pbench CI](https://github.com/distributed-system-analysis/pbench/blob/64364eeb2d027ce562da4861af9a588cc18a6d8d/build.sh#L27)

## Benefits

All python projects within Arcalot will follow an expected norm for formatting
standards, simplifying readability, and code reviews.  This eliminates coding
style preference changes and formatting debates.

## Drawbacks

It's impossible to define one perfect standard the everyone loves. There will
inevetibly be quirks to the formatting and disagreements from the community
with the chosen approach.
