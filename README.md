# mypy-action

This action will set up python, install requirements, and then run mypy.
Passing checks are gated by any settings defined in mypy's configuration.
By default, mypy runs in the root directory of the repo.
The arguments to mypy may be overridden by supplying a `args` input to the action.

This action will use a `mypy.ini` (or `.mypy.ini`, `pyproject.toml`, or `setup.cfg`) file in the root directory of the calling repository to configure how mypy runs.
See https://mypy.readthedocs.io/en/stable/config_file.html.

This action can be called independently or called via the `open-reading-frame/reusable-workflows/.github/workflows/static-analysis.yml` reusable workflow.
