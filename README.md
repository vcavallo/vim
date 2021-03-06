## To update this repo on another machine (after updates elsewhere):

may need to `git submodule update --init` if submodule directories are empty

## To add a new plugin:

```
git submodule add git@github... bundle/submodule-name
git commit
git push
```

## To 'install' this vim environment on another machine:

```
git clone git@github.com:vcavallo/vim ~/.vim
cd ~/.vim
git submodule init # [maybe add --init]
git submodule update
```

_Make sure to update the machine's dotfiles as well [git@github.com:vcavallo/dotfiles]_

ctags or exuberent ctags will likely need tobe installed as well

## reminders

- if you're getting issues with `submodule update` or `submodule init`:
  - `git rm --cached bundle/the-problematic-submodule` and try again (repeat).
    I think this means the local machine you're on has directories for
    submodules but the `.gitmodules` file doesn't contain them anymore.
  - make sure the machine you're
    using has an ssh key on github. then make sure that no submodules have local
    changes (not sure what this is about, but it seemed to happen once.)
