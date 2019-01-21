## Mac Core Setup

Although I work 100% on linux systems I must say that my favorite operating system to work on is MacOS. I get the benefit of a unix based operating system with the bonus of a beautiful system. Now, MacOS is not perfect so here are some minor tweeks that I implement on my mac to get it up and running. 

Fist thing first, I need a package manager. I prefer to use brew since it's really the only one that I have tested and have grown to love the system. [here](https://brew.sh/) you can find the link to the official site. 

### Brew

Installing brew is quite easy just open the terminal and run the following.

```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Once installed I trypicall install the following right away. 

```
brew install wget git tmux doctl bash-completion terraform watch
```

### tmux config

```
# remap prefix from 'C-b' to 'C-a'
unbind C-b
set-option -g prefix C-a
bind-key C-a send-prefix

# split panes using | and -
bind | split-window -h
bind - split-window -v
unbind '"'
unbind %
```

### bashprofile config

```
# profile
export PS1="\W \$ "

# bash completion (brew)
source <(kubectl completion bash)
if [ -f $(brew --prefix)/etc/bash_completion ]; then 
. $(brew --prefix)/etc/bash_completion
fi

# Add Visual Studio Code (code)
export PATH="$PATH:/Applications/Visual Studio Code.app/Contents/Resources/app/bin"

# Powerline
powerline-daemon -q
POWERLINE_BASH_CONTINUATION=1
POWERLINE_BASH_SELECT=1
source /usr/local/lib/python3.7/site-packages/powerline/bindings/bash/powerline.sh

# Alias
alias t='tmux'
```

[back](../)
