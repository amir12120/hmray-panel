# NOTICE

**HMray Panel** is an independent project maintained by
[amir12120](https://github.com/amir12120) at
<https://github.com/amir12120/hmray-panel>. That repository is the canonical
source: releases, container images, the installer, the updater and in-app update
checks all resolve there, and development continues there.

## Where the code came from

- Upstream project: HMPanel — <https://github.com/neoauroraproject/hmpanel>
- Upstream author: the HMPanel Team (© neoauroraproject)
- Last sync: **upstream v3.0.1**. This build is versioned `3.0.1-hmray.N` so
  fork builds stay distinguishable from upstream releases while remaining
  semver-comparable for the panel's update check.
- Earlier work: the fork started from upstream **v2.5.20**, which upstream had
  published under the MIT License, and which the fork rebranded as HMray Panel.

Code imported from upstream v2.5.21 through v3.0.1 ships upstream without a
LICENSE file and with `backend/package.json` marked `"UNLICENSED"`. It is
redistributed and rebranded here **with the upstream author's written
permission**; that permission covers this repository and its container image
under the `amir12120/hmray-panel` name. Copyright in the imported files remains
with the upstream author — see `LICENSE` for the exact scope, which part is MIT
and which part is not.

## What is not included

The upstream product sells a separate **Premium** edition. Premium feature code
is not part of this repository: it is delivered at runtime as a downloadable
bundle by the vendor's license server and is guarded in the code by
`backend/src/common/guards/premium.guard.ts`. No premium material from the
vendor is redistributed here, and the license/entitlement checks are kept
intact.

## Building on this repository

Keep this notice and the upstream attribution. Copyright in the imported work
remains with the upstream author; the HMray Panel work on top of it is released
under the MIT License as described in `LICENSE`.
