---
title: 'Terminal Setup'
date: 2019-11-12 00:00:00
featured_image: '/images/2019-11-12/featured_terminal.jpg'
excerpt: I get asked all of the time how I setup my terminal to look the way that it does. In this post I share my secret sauce with the world. Hint, its not a secret as a matter of a fact there is a pretty sizable community behind what I use.
---

![](/images/2019-11-12/terminal.png)

To begin, let's give credit where credit is due. The colors and magic could not be possible without the Dracula Theme. Credit goes to that awesome community. 

You can find them [HERE](https://draculatheme.com/).

I use the Dracula Theme on everything:
* VSCode
* Slack
* Terminal

> "Lets get your terminal looking amazing!"

Well it's really simple: 

The following instructions are aplicable to mac users. 
1. Download zip file from the following [link](https://github.com/dracula/terminal-app/archive/master.zip).
2. Unzip the file. 
3. Terminal > Settings Tab
4. Click "Gear" icon
5. Click Import...
6. Select the Dracula.terminal file
7. Click Default


Run the following command to change shells and install oh-my-zsh. 
```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

Finally:

Add the following plugins to your ```~/.zshrc``` config. 

```
plugins=(
 docker
 docker-compose
 git
 doctl
 kubectl
 zsh-autosuggestions
 zsh-syntax-highlighting
 helm
 golang
 vscode
 kube-ps1
)
```

There are hundreds of plugins to choose from. These currently work for my needs. 
zsh-autosuggestions and zsh-syntax-highlighting do not come by default. 
You can refer to [zsh-users](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md) on installation instructions.

Click here to read more on [oh my zsh](https://github.com/robbyrussell/oh-my-zsh).

---

## Pretty cool, huh?

Do not forget to folllow me on [twitter](https://twitter.com/_areyesjr) for updates and extras. 

<a href="../" class="button button--large">Back</a>