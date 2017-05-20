# dirbuster-ng

This is a fork of dirbuster-ng with a one line patch to change the logic for what 'found' means. Rather than saying found is `(response_code == 200)` it now is `(response_code && response_code != 404)`

## This file

Also added this file, original project has no README
