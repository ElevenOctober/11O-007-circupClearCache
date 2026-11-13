# Validation

## Local checks

- The clear-cache confirmation and cancellation tests passed.
- The README CLI-help synchronization test passed.
- Changed-file pre-commit hooks passed (Black, Pylint, REUSE, end-of-file, whitespace).
- Full Windows suite with Python 3.12: 67 passed, 5 failed. Four failures compare POSIX paths with Windows paths; one `install --auto-file` test expects a different exit code. These failures are outside the changed behavior.
- No hardware is needed for these CLI and documentation changes.

## Upstream CI

- The `Build CI / test` job passed on [PR #292](https://github.com/adafruit/circup/pull/292).
- Run: [43494225707](https://github.com/adafruit/circup/actions/runs/43494225707).
- PR #292 remains open and is awaiting maintainer review and merge.
