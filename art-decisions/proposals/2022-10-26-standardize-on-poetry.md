# Title

All python projects in Arcalot should standardize on the use of
[poetry](https://python-poetry.org/) for dependency management and packaging.
This standard should be built into documentation and contribution guidelines,
included in any templates, and should be checked automatically by CI.

Voting period for this proposal will end 14 days after its original submission.

## Benefits

From @mfleader:

`requirements.txt` in no way defines how a python project can be built and
published as a package. From [PyPA](https://www.pypa.io/en/latest/) on python
project configuration, the `pyproject.toml` is equivalent to `requirements.txt
&& setup.py`. If we're requiring plugins to be publishable, and `setup.py`
is deprecated, then we have to require `pyproject.toml`, and `requirements.txt`
is redundant.

One of the main issues is that `pip` cannot ingest a `pyproject.toml` to install
dependencies for local development. To maintain exactly one set of software
dependencies (instead of a `pyproject.toml` and a `requirements.txt`) for your
project, and to be able to publish that project, then you need a software tool
that can programmatically interact with a `pyproject.toml` (i.e. add and remove
software dependencies). If that software tool can also export the software
dependencies defined in a `pyproject.toml` as a `requirements.txt`, then that's
a bonus, so that other developers do not need to use the exact same software
dependency manager. There just aren't many options for python software
dependency management and/or python package publishing.

An example with `poetry`:

```bash
poetry export --without-hashes --format=requirements.txt > requirements.txt
```

Exporting the `pyproject.toml` to a `requirements.txt` also means we do not need
`poetry` in our python image build environment, but it is unclear how much that
matters.


## Drawbacks

This imposes more process and compliance requirements on contributors, forcing
the integration of `poetry` into their workflows.
