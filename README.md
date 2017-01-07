# git_jira_hooks

* prepare-commit-msg: Takes jira ticker number from branch name and puts that into your prepared commit message

Works with branch names like:

```
abc/proj-123
def/proj-123_new_feature1
```
and is [easy to extend](hooks/prepare-commit-msg)

## How to use it?

* Clone this repo as your .git_template
```
git clone https://github.com/codesurf42/git_jira_hooks.git ~/.git_template
```

* Add lines below to your ```~/.gitconfig```

```
[init]
  templatedir = ~/.git_template
```

* Reinitialise your current git repository with:
```
cd your_repo
git init
```

* When you commit something, just don't use ```-m``` so the message will be prepared by git itself:

```git commit``` or ```git commit -a```

* Thank you for using. Please contribute your automation ideas!
