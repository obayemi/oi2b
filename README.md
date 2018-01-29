oi2b
====

obayemi interface to blih, because blih sucks, because you allways forget
someone of your team, because you often forget ramassage-tek, because you
don't want to use the command 'rendu' (if you do, trust me, you don't, just
read it's code and and you won't want much longer), because you
want to be able to clone your repos everywhere but in ~/rendu, because you
want to clone easily your repos on whatever linux distribution, or even
windows accurding you got it a POSIX shell.


# Installation (for zsh)
```bash
mkdir -p $HOME/.local/lib/
git clone https://github.com/obayemi/oi2b ~/.local/lib/oi2n
ln -s $HOME/.local/lib/oi2b/oi2b $HOME/.local/bin/oi2b
echo 'export OI2B_HOME=$HOME/.local/lib/oi2b/'
echo 'export PATH=$HOME/.local/bin:$PATH' >> $HOME/.zshrc
```


# Usage
to create a repo:
```bash
oi2b create_repo repo_name
```
> note: when asked for new users, add a list of user's names separated by
> spaces

to clone a repo
```bash
oi2b get_repo [user/]repo_name
```

# TODO:
Maybe one day, if I'm not that lazy:
- key uploading utility
- bash argparse --short and --help in module
- module template to source to provide basic args recognition
- bash / zsh completion
