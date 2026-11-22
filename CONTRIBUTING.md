# Contributing to Mosgird client

The contribution process for this repository is the same as for the protocol repository. See [CONTRIBUTING.md](https://github.com/mosgird/protocols/blob/main/CONTRIBUTING.md).

This repository adds two requirements: the `contribution-policy` and `actions-lock` checks must pass before a pull request can merge. `actions-lock` checks that `.github/workflows/actions.lock` locks every action the workflows use; after changing a `uses:` line, run `gh actions-lock` (the GitHub CLI extension `github/gh-actions-lock`) and commit the updated lockfile.

Implementation details for client belong in this repository, in its own documentation. Protocol behavior belongs in the protocol repository.
