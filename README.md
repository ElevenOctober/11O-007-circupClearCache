# 11O-008: Circup clear-cache and README help

Private contribution record for [adafruit/circup issues #221](https://github.com/adafruit/circup/issues/221) and [#170](https://github.com/adafruit/circup/issues/170).

**Status:** [PR #292](https://github.com/adafruit/circup/pull/292) is open. Its `Build CI / test` job passed; it is awaiting maintainer review and merge.

## Problems

Issue #221 requests a command to remove Circup's saved state after problems such as a broken bundle download. Issue #170 reports that the README's CLI help output had fallen behind the current command and options.

## Changes

- Adds the boardless `circup clear-cache` command. It asks for confirmation before deleting Circup's data directory, which contains downloaded bundles and local bundle settings, and reports when there is nothing to clear.
- Refreshes the README's complete `circup --help` example and adds a test that checks the documented output against the Click command.

## Validation

See [validation.md](validation.md) for local and CI results. The upstream change is preserved in [`patches/circup-clear-cache.patch`](patches/circup-clear-cache.patch).
