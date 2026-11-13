# Validation

## Local checks

- Both clear-cache CLI tests passed, covering confirmation and cancellation.
- Changed-file pre-commit hooks passed (Black, Pylint, REUSE, end-of-file, whitespace).
- Full Windows suite with Python 3.12: 66 passed, 5 failed. Four failures compare POSIX paths with Windows paths; one `install --auto-file` test expects a different exit code. These are outside the clear-cache command and tests.
- No hardware is needed for this CLI command.

## Upstream CI

- The `Build CI / test` job passed on [PR #292](https://github.com/adafruit/circup/pull/292).
- PR #292 remains open and is awaiting maintainer review and merge.
