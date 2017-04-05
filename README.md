# npm-superls

Basically, I want to upgrade `npm ls` to list builtin module dependencies. The idea would be that I can run `npm superls` and get the same output as `npm ls`, but with builtin modules included, such as `fs`, `path`, `crypto`, etc.

This `grep` command gives the list of all files that require the `crypto` module:

```shell
grep -RnisI "require('crypto')" *
```
