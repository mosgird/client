# Agent rules

The rules for AI agents and contributors are kept once, in the protocol repository:

- [AGENTS.md](https://github.com/mosgird/protocols/blob/main/AGENTS.md)
- [AI_POLICY.md](https://github.com/mosgird/protocols/blob/main/AI_POLICY.md)
- [CONTRIBUTING.md](https://github.com/mosgird/protocols/blob/main/CONTRIBUTING.md)

Read them before making changes. This file only points to them.

## Protocol details

The protocol is specified in [mosgird/protocols](https://github.com/mosgird/protocols). Before implementing, changing, or documenting protocol behavior, read the specification there, starting with `spec/v0.1/overview.md` and the decision records in `spec/decisions/`. Wire formats, cryptographic procedures, and test vectors are defined there, not in this repository. If this repository and the specification disagree, the specification is correct. Propose a specification change in the protocol repository before changing behavior here.

## Test-driven development

Work test first: write a failing test, then the least code that passes it, then refactor. Keep at least 3 lines of test code per line of production code, counted without blank lines and comments, for this repository, for each unit (crate or module), and for each production file. Fuzz targets, Kani harnesses, hax annotations and test tools count as tests. Whole test files name what they test in a `covers:` comment.

The full rule is in the protocol repository's [AGENTS.md](https://github.com/mosgird/protocols/blob/main/AGENTS.md#test-driven-development). The required `test-ratio` check enforces it. To run it locally, with the protocol repository checked out beside this one:

```sh
python3 ../protocols/scripts/check_test_ratio.py .
```
