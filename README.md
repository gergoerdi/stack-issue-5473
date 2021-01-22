To reproduce https://github.com/commercialhaskell/stack/issues/5473, follow these steps:

```
$ stack build                            # Works as expected
$ cp clash-HEAD2.yaml clash-HEAD.yaml    # Changes the Git commit hash of Clash dependency
$ stack build                            # Rebuild fails at link time 
```
