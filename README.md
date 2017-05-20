# dirbuster-ng

This is a fork of dirbuster-ng with a one line patch to change the logic for what 'found' means. Rather than saying found is `(response_code == 200)` it now is `(response_code && response_code != 404)`

## Stability notes

I've experienced a lot of crashes when running dirbuster-ng. However, when run in GDB, it seems to work just fine. This is probably due to some NULL ptr dereference being ignored in a thread, or maybe more likely some race condition not getting triggered.

## This file

Also added this file, original project has no README

