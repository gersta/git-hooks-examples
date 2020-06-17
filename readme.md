# Git Hook Examples
This is a collection of githooks, which is a standard feature of git. Usually, the hooks are located under .git/hooks of your project and they all carry the file ending `.sample`, which
deactivates them. Simply removing the file ending, actives them. You can hook into various lifecycle events of your typical git workflow, like:

* commit-msg
* pre-commit
* pre-push

This allows for a bunch of options, incl.:

* linting your code
* checking for specific ids in the commit message
* preventing unformatted commit messages

The files in this repository each contain multiple examples and you can just remove/comment those that you don't want to use.

## Configure the hooks directory
You can easily re-configure the directory that your hooks live in, by running the following command:

```
git config --local core.hooksPath .githooks/
```

This moves the hooks directory to .githooks (same level as your .git folder) only for this very repository.
