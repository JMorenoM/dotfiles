Dotfiles
========

This repository includes some of my custom dotfiles. 

Installation Vundle
-------------------
Install vundle for vim plugins

	$ git clone https://github.com/gmarik/Vundle.vim.git ~/.vim/bundle/Vundle.vim
	

Installation Prezto — Instantly Awesome Zsh
---------------------------------------------


Prezto will work with any recent release of Zsh, but the minimum required
version is 4.3.17.

  1. Launch Zsh:

        zsh

  2. Clone the repository:

        git clone --recursive https://github.com/sorin-ionescu/prezto.git "${ZDOTDIR:-$HOME}/.zprezto"

  3. Create a new Zsh configuration by copying the Zsh configuration files
     provided:

        setopt EXTENDED_GLOB
        for rcfile in "${ZDOTDIR:-$HOME}"/.zprezto/runcoms/^README.md(.N); do
          ln -s "$rcfile" "${ZDOTDIR:-$HOME}/.${rcfile:t}"
        done

  4. Set Zsh as your default shell:

        chsh -s /bin/zsh

  5. Open a new Zsh terminal window or tab.

### Troubleshooting

If you are not able to find certain commands after switching to *Prezto*,
modify the `PATH` variable in *~/.zprofile* then open a new Zsh terminal
window or tab.

### Note
For more info about Prezto: <https://github.com/sorin-ionescu/prezto>

Create links
------------
	
	cd ~
	git clone https://github.com/JMorenoM/dotfiles.git ~/dotfiles
	ls -s dotfiles/vimrc .vimrc
	ls -s dotfiles/zshrc .zshrc
	ls -s dotfiles/tmux.conf .tmux.conf

Then the prompt looks like:

![MacDown Screenshot](http://mikebuss.com/images/posts/a-beautiful-productive-terminal-experience/cover.png)