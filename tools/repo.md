####Repo Tool Basics
====================

Switching to new branch after repo sync
======================================

repo init by default fetches everything (If you didn't fetch just that branch explicitly). -b is just checkout
Just repo init with new branch and repo sync again

```
repo init -u https://android.googlesource.com/platform/manifest android-5.1.1_r36
repo sync -j8
```



