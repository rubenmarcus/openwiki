---
"openwiki": patch
---

Fix a crash that aborted repository runs when skipping a page whose parent directory was never written: the filesystem backend surfaces a raw ENOENT delete error, which the not-found guard now tolerates.
