# git-tricks

Handy things to do with git.

## Diff two files in the current branch

`git diff --no-index file/one file/two`

## Merge changes from one file into another, in the same branch

The following will merge the changes from source_file into destination_file.

```
touch deleteme #empty file to serve as common ancestor
git merge-file destination_file deleteme source_file
rm deleteme
```

* [Stack Overflow](https://stackoverflow.com/a/9123563)

# Debugging steps

1. Exactly replicate examples from the library source.
2. Consider any environment/configuration changes you've made or will need to make.
