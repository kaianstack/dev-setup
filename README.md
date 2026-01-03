I am using Windows 10.


# GitHub
In GitHub to keep your email private, go to https://github.com/settings/emails and turn on "Keep my email addresses private". 

*After that your every git action to GitHub repos with your email will be hided by a GitHub email.*

Copy your private email address that looks like this 12345678+username@users.noreply.github.com
to use it in git config.

# VS Code
Sign on in VS Code with the GitHub account.


I am using VS Code built-in Git controller (Ctrl+Shift+G G) to do most of git actions.

But in setting up you need to do some actions in cmd.



# Git
1. Install Git
2. Make Sure you have your name and email in git config.

Check it like that in cmd:

`git config --global user.name`

`git config --global user.email`

You can change it like that:

`git config --global user.name "Your Name"`

Then set-up email. Your real one if "Keep my email addresses private" is off. And private one that you copied previously in GitHub if "Keep my email addresses private" is on.

`git config --global user.email "email"`

If you tried to push with real one and "Keep my email addresses private" is on and gets the error, you need to set the correct email using the command above and then execute `git commit --amend --reset-author` and try to push again.



