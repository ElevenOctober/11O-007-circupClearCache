# 11O-008: Circup clear-cache

Private contribution record for [adafruit/circup issue #221](https://github.com/adafruit/circup/issues/221).

**Status:** [PR #292](https://github.com/adafruit/circup/pull/292) is open. Its `Build CI / test` job passed; it is awaiting maintainer review and merge.

## Problem

A broken bundle download can leave Circup's saved data in a bad state. Issue #221 asks for a command to remove all saved state.

## Change

Adds the boardless `circup clear-cache` command. It asks for confirmation before deleting Circup's data directory, which contains downloaded bundles and local bundle settings, and reports when there is nothing to clear.

## Validation

See [validation.md](validation.md) for local and CI results. The upstream change is preserved in [`patches/circup-clear-cache.patch`](patches/circup-clear-cache.patch).
