# Safari MediaTrack Clone Bug Reproduction

This experiment shows an issue in Safari 18 on iOS and macOS: Cloning a disabled `MediaStreamTrack` does not retain the `enabled` state.
It shows that the cloned track incorrectly has `enabled` set to `true` instead of mirroring the original `false` state.
