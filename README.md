# orca-build

Unsigned macOS builds of [Orca](https://github.com/stablyai/orca) for HarnessOS.

Each commit that replaces `inputs/` is one build: the patch series, the build manifest and lock, and the build script it was dispatched with. A run of `build.yml` on GitHub's `macos-15` runner checks out `stablyai/orca` at the selected release tag, refuses a tag that no longer names the selected commit, applies the series, builds and tests it, and uploads the unsigned zip with its receipt. The zips here are not signed and are not meant to be installed.

This repository holds no secret, and its workflow reads none.
