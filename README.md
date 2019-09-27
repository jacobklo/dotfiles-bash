# configs for bash

This store all the configs for bash, also all the plugins and themes.


# clone this repo
clone this repo into the $HOME directory, using following command
```
git clone --bare https://github.com/jljacoblo/dotfiles-bash.git $HOME/.gitdotbash
```


# checkout
checkout the repo for all the configs
```
git --git-dir=$HOME/.gitdotbash/ --work-tree=$HOME checkout
```


# update bashrc
Now, need to add custom commands for bashrc to load, just link bashrc_bash to bashrc
```
echo "source ~/.bashrc_bash" >> ~/.bashrc
```


# pull all the git submodules
Now, pull all the git submodules inside this repo, especially all the vim plugins
```
gitdotbash submodule update --init --recursive
```


# Commit changes
Now, you can use a special git command: gitdotvim.

All the changes required stage manually.
```
gitdotbash status
gitdotbash add new_changes
gitdotbash add new_unstage_files_that_not_shown
```

Then commit and push
```
gitdotbash commit -m "commit message"
gitdotbash push
```

# Reference and More Info:
[The best way to store your dotfiles: A bare Git repository](https://www.atlassian.com/git/tutorials/dotfiles)
