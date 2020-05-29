# git_subtree_example

# Add subtree
```
git subtree add --prefix lib/OpenBLAS https://github.com/xianyi/OpenBLAS master --squash
git log
```

# Update subtree
```
git subtree add --prefix lib/OpenBLAS https://github.com/xianyi/OpenBLAS master --squash
```

# Pushing to a subtree
tricky and slow

subtree repository has no knowledge of the original repository.

# Conclusion
Is the external repository something you own yourself and are likely to push
code back to? **submodule** (dont forget to run a git submodule update.)

Is the external repository third party code that you are unlikely to push
anything back to? **subtree**
