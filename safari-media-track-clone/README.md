# Safari MediaTrack Clone Bug Reproduction

This experiment shows an issue in Safari 18 on iOS and macOS: Cloning a disabled `MediaStreamTrack` does not retain the `enabled` state.
It shows that the cloned track incorrectly has `enabled` set to `true` instead of mirroring the original `false` state.

| Test on Safari 18           | Test on Chrome 130         |
|-----------------------------|-----------------------------|
| <img width="700" alt="Screenshot from Safari 18" src="https://github.com/user-attachments/assets/457aff57-42a7-4854-937e-bade35a4df5a"> | <img width="700" alt="Screenshot from Chrome 130" src="https://github.com/user-attachments/assets/61e8aef5-9612-4340-ac39-9f07775f7213"> |

Bug report: https://bugs.webkit.org/show_bug.cgi?id=282465

