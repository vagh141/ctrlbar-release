# ctrlbar-release

Release buttons for Greenmission Ctrl firmware. Every run waits for the owner's approval in GitHub before anything
reaches beta testers or customers. No code and no secrets live in this repository; the upload key is an encrypted
environment secret with a no-overwrite, no-delete AWS policy.

- `firmware-release`: beta = dev bucket -> stage (environment `release`); prod = stage -> production (environment
  `release-prod`, only a file already in beta, same sha256).
