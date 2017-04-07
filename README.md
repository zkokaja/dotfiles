# dotfiles

My UNIX dot files.

## Structure

Based on [GNU Stow](https://www.gnu.org/software/stow/):

```shell
.
├── .gitignore
├── README.md
├── bash
y   ├── .bash_aliases
│   ├── .bash_exports
│   ├── .bash_functions
│   ├── .bash_profile
│   └── .bashrc
├── git
│   └── .gitconfig
├── readline
│   └── .inputrc
├── tmux
│   └── .tmux.conf
├── vim
│   ├── .vimrc
│   └── .vim
│       └── autoload
│           └── plug.vim
└── x11
    ├── .Xresources
    └── .Xresources.d
        ├── urxvt
        └── xft
```

## Usage

```shell
$ git clone https://github.com/zkokaja/dotfiles.git
$ cd dotfiles
$ stow bash
$ stow tmux
$ stow vim
```

Install vim plugins with `:PlugInstall!` and update with `:PlugUpdate!`.

Use `stow -t ~` if parent directory is not home.
