## Mac Core Setup

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

[back](./)
