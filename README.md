DESCRIPTION
===========
Git version individual files without being in a (visible) git repository.

USAGE
=====
`ver <filename> <anything git can do>`

EXAMPLE
=======
You've got a quick script, `doit.bash`, that you want to version control so you can move faster.
```
ver doit.bash init
```
creates a git repo associated with `doit.bash`.  Then
```
ver doit.bash add doit.bash
ver doit.bash commit -m "Add doit.bash"
```
makes your first commit.  If you'd added `eval $(ver --bashrc-amendments)` to your `$HOME/.bashrc`, then you could use the `vir` shorthand which uses the most recent `<filename>`.  That would look like
```
ver doit.bash init
vir add doit.bash
vir commit -m "Add doit.bash"
```

INSTALL
=======
```
mkdir -p $HOME/bin && cd $HOME/bin && ln -s /path/to/this/repository/ver
```
