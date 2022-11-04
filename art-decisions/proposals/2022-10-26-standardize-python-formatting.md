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
$ isort --profile black --check .
$ black --check .
$ flake8 .
```

Acceptance of this proposal would require applying the formatting first to all
existing code at the same time as adding the `pre-commit` hooks.

Voting period for this proposal will end 14 days after its original submission.

## Recommendation

It is important that we adhere to one standard judiciously and eliminate further
debate on the topic. The standards documented above match the standards already
adopted by the [pbench](https://github.com/distributed-system-analysis/pbench)
repository. This formatting standard should also be applied wherever possible to
automation and CI.

Locally, one would first run `isort --profile black` to get the imports
sorted, then run `black` to fix up the formatting, then verify the remainder
of PEP 8 using `flake8`.

Here is an example set of scripts one can use locally for any changed Python
file.

`apply-pep-8`:
```
#!/bin/bash
function gitpyfiles {
    git status -s --ignored=no --untracked-files=no | awk '{print $2}' | while read line; do
        file ${line} 2> /dev/null | grep -F "Python script" | awk -F ':' '{print $1}'
    done
}

pyfs=$(gitpyfiles)
isort --profile black ${pyfs} && black ${pyfs} && flake8 ${pyfs}
```

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
