Here are all the alias creation commands in a single bash snippet that you can paste into your bash profile:

```
alias gs='git status'
alias gb='git branch'
alias gco='git checkout'
alias gcb='git checkout -b'
alias gl='git log'

```

Copy and paste this code into your bash profile, and the Git aliases will be available to you the next time you open a terminal window.

To add these Git aliases to both your bash profile and zshrc files in the terminal, you can use the following command:

```
echo -e "alias gs='git status'\\nalias gb='git branch'\\nalias gco='git checkout'\\nalias gcb='git checkout -b'\\nalias gl='git log'" >> ~/.bash_profile && echo -e "alias gs='git status'\\nalias gb='git branch'\\nalias gco='git checkout'\\nalias gcb='git checkout -b'\\nalias gl='git log'" >> ~/.zshrc && source ~/.bash_profile && source ~/.zshrc

```

This command will append the Git aliases to both your `.bash_profile` and `.zshrc` files, and then source both files so that the aliases are immediately available in your terminal session.