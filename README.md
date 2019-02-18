<p align="center"><img src="https://github.com/amiremohamadi/bash-mardom-azar/blob/master/screen-shot.png"></p>

# What's this?!
**bash-mardom-azar** (Persian: بشِ مردم آزار) is a persian fork of [bash-insulter](https://github.com/hkbakke/bash-insulter)

Randomly insults the user when typing wrong command.

Change insults as needed :)

**Note**: Use a terminal with rtl support like [konsole](https://github.com/KDE/konsole)

```bash
amir@qwerty:~ $ sl

  تلاشت قابل تحسین بود! (:

-bash: sl: command not found
amir@qwerty:~ $ gti status

  این چیه نوشتی آخه؟!!!! :|

-bash: gti: command not found
amir@qwerty:~ $ sp aux

 اسکار تایپیست سال میرسه به... amir!

-bash: sp: command not found
```

# Installation

    git clone https://github.com/amiremohamadi/bash-mardom-azar.git
    sudo cp bash-mardom-azar/src/bash.command-not-found /etc/

Then source the file automatically for new logins by adding the following to `/etc/bash.bashrc` or any of the other locations where you can configure your shell automatically during login (zsh have different config files):
```
if [ -f /etc/bash.command-not-found ]; then
    . /etc/bash.command-not-found
fi
```
Login again and type some invalid commands for the effects to be visible.
