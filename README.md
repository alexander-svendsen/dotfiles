# Alexander's dotfiles

Dotfiles are how you personalize your system. It contains the prefs and settings for your toolbox. Your dotfiles might be the most important files on your machine. These are mine.

Fore more info about dotfiles read: https://dotfiles.github.io/

## Installation

Clone the repository and run the install.sh script. The install script will pull in the latest version and copy the dotfile to your home folder.

```bash
git clone https://github.com/alexander-svendsen/dotfiles.git && cd dotfiles && source bootstrap.sh
```

To update, run the last command again inside your `dotfiles` repository:

```bash
source bootstrap.sh
```

You need to have set up **git** to get started:

## Initial Git setup

```bash
# Generate ssh key
ssh-keygen -t rsa -C "your.email@xxx.yy"

# Add ssh key to ssh-agent
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa

# Copy ssh key to github.com
subl ~/.ssh/id_rsa.pub

# Test connection
ssh -T git@github.com

# Set git config values
git config --global user.name # <NAME>
git config --global user.email # <EMAIL>
```


## Thanks to
- [Mathias Bynen's dotfiles](https://github.com/mathiasbynens/dotfiles)
- And other random repos found on Github
