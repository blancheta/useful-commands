# Tools

```
pip install ipython
```

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

# AWS

aws s3 sync s3://memshumedia/audio/ . --size-only

# Mac OS
brew services info nginx

Go to app windows: Command + Tab + Key up

Screenshot (all screen) Shift + Command + 3

Screenshot (selected area) Shift + Command + 4

Change tab in terminal: Fn + Command + Left/Right

mdfind "youtube" | grep '\.py$'

Type : Shift + Alt + K

Restart postgresql: brew services restart postgres

sudo  grep CRON /var/log/syslog

# VIM

Ctrl + V : Visual Block

V + SHIFT + > OR < to indent/unindent code

# Shell

grep -rnw '/path/to/somewhere/' -e 'pattern': Find string in files
du -cha --max-depth=1 /var/lib | grep -E "M|G Find what is taking up in a folder
printf '.idea\n__pycache__/*.pyc\n*/__pycache__/*.pyc\n/venv/*\ndb.sqlite3' > .gitignore

pg_ctl -D /usr/local/var/postgres start
pg_ctl -D /usr/local/var/postgres stop

sudo dscacheutil -flushcache; sudo killall -HUP mDNSResponder

# Django

Export DB to file: ./manage.py dumpdata --exclude contenttypes > dump_02_11_2020.json

# PostgreSQL

 GRANT ALL PRIVILEGES ON DATABASE pickmylaptop TO admin;
 
 # Kill process on port
 kill -9 $(lsof -ti:8000)

# Wordpress

Installation
```
mysql_installation
CREATE DATABASE db;
CREATE USER "user"@"host" IDENTIFIED BY "password";
GRANT ALL PRIVILEGES ON db.* TO "user"@"host";
nano /opt/homebrew/etc/php/8.4/php-fpm.d/www.conf
```

UPDATE wp_options SET option_value = replace(option_value, 'oldurl.com', 'newurl.com') WHERE option_name = 'home' OR option_name = 'siteurl';UPDATE wp_posts SET guid = replace(guid, 'oldurl.com','newurl.com');UPDATE wp_posts SET post_content = replace(post_content, 'oldurl.com', 'newurl.com'); UPDATE wp_postmeta SET meta_value = replace(meta_value,'oldurl.com','newurl.com');

Permissions
```
chmod a+w wp-content/uploads
chmod a+w wp-content/
chmod a+w wp-content/plugins/
chmod a+w wp-content/themes/
chmod a+w wp-content/upgrade/
chmod a+w wp-content/upgrade-temp-backup/
sudo chown -R www-data:www-data wordpress
```

# Docker
```
docker build . --tag backend --no-cache
docker run -it -p 80:8080 --name app-backend backend
```

SHELL

```
files=()
for file in "${files[@]}"; do
  ffmpeg -i "old_audio/$file" "audio/${file%.wav}.ogg"
done

netstat -tupn | grep -E ":(22|80|8000) .*"
sudo iptables -A INPUT -p tcp --dport 22 -s ip -j DROP
```
