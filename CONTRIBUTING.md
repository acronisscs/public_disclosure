# How to contribute

This repository is managed by @AcronisSCS. Please make a pull request if you
spot any typos or other errors.

## pre-commit

[`pre-commit`][pre-commit] is a Python project for maintaing git pre-commit
hooks. This repository uses `pre-commit` to enforce a number of commit-time
checks. The checks to run are specified in a rules file at the base of this
repository called [`.pre-commit-config.yaml`](.pre-commit-config.yaml).

To get started with it:

1. Install the latest version of Python
2. Install `pre-commit` with `pip install pre-commit`
3. Run `pre-commit install` in the project root
4. Run `pre-commit install --hook-type commit-msg`

When adding new hooks to the config file, use `pre-commit run --all-files` to
check everything with the new hooks.

### Commit style

Commits should be formatted as one of the [Conventional Commits][conventional-commits]
types followed by a colon and a brief description.

<!-- Links -->
[pre-commit]: <https://pre-commit.com/>
[conventional-commits]: <https://www.conventionalcommits.org/en/v1.0.0/>
