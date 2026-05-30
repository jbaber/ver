DESCRIPTION
===========
Git version individual files without being in a (visible) git repository.

USAGE
=====
- `ver <filename> <anything git can do>`
- `vir <anything git can do>`

`vir` calls ver with the most recent <filename>.

Put

```
eval "$(ver --bashrc-amendments)"
```

in `$HOME/.bashrc` (or your shell's equivalent) to make `vir` available
