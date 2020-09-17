# useful-shortcuts
Ctrl + Shift + T : reopen tabs closed in history

# useful-commands
Useful commands

### To rename all file.txt in children folder to super-file.txt
rename 's/finish-flag/finish_flag/' drawable*/finish-flag.png

# Bash aliases
alias appbifup='cd ~/projects/bifup-mobile/'

### To add in .bashrc for loading at startup
if [ -f ~/.bash_aliases ]; then
    . ~/.bash_aliases
fi

# Git aliases

git config --global alias.df diff

# Pycharm

Command + 1: Go to left panel

Control + Alt + H: Open Call Hierarchy view

Command + B: Find usages

Ctrl + Shit + Test: Generate a new test for selected method

Shift + Alt + Command + T: Refactor this

Shit + Command + Test: Go to test for the class test where the cursor is.

Command + K: Commit change

Shift + Command + K:  Push changes

Alt + Command + A: Add file to changes

Alr + Command + O: Optimize imports

# Mac OS

Go to app windows: Command + Tab + Key up

Screenshot (all screen) Shift + Command + 3

Screenshot (selected area) Shift + Command + 4

Change tab in terminal: Fn + Command + Left/Right

Type : Shift + Alt + K

Restart postgresql: brew services restart postgres

# VIM

Ctrl + V : Visual Block

# Shell

grep -rnw '/path/to/somewhere/' -e 'pattern': Find string in files
printf '.idea\n__pycache__/*.pyc\n*/__pycache__/*.pyc\n/venv/*\ndb.sqlite3' > .gitignore

pg_ctl -D /usr/local/var/postgres start
pg_ctl -D /usr/local/var/postgres stop
