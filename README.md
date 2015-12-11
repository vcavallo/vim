## To add a new plugin:

```
git submodule add git://github.com/thoughtbot/vim-rspec
```

## To 'install' this vim environment on another machine:

```
git clone git@github.com:vcavallo/vim ~/.vim
cd ~/.vim
git submodule init
git submodule update
```

_Make sure to update the machine's dotfiles as well [git@github.com:vcavallo/dotfiles]_

ctags or exuberent ctags will likely need tobe installed as well
