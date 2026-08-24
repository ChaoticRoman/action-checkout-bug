# Checkout action submodules bug

When we have submodule introduced on top of the default branch, checkout action
for any branch created before the submodule is introduced will contain directory
for this submodule instead of having the branch in clean state.

This repo aims to reproduce this.

**Result:** Negative, not reproduced on GitHub runners, the problem seems to be
caused by some misconfiguration of our runners.
