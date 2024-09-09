# 31279

Reproduction for https://github.com/renovatebot/renovate/discussions/31279

## Current behavior

Version range for changelogs is calculated from the value in `Cargo.toml`,
even though that's actually a semver range, and the installed version in `Cargo.lock`
is newer.

## Expected behavior

Use the locked/installed version from `Cargo.lock` to calculate the version range that
changelog entries should cover.

## Link to the Renovate issue or Discussion

https://github.com/renovatebot/renovate/discussions/31279
