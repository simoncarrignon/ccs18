#CCS 2018
this jekyll template is a fork of alembic, see her:
# [Alembic](https://alembic.darn.es/)
[![Gem Version](https://badge.fury.io/rb/alembic-jekyll-theme.svg)](https://badge.fury.io/rb/alembic-jekyll-theme)

⚗ A Jekyll boilerplate theme designed to be a starting point for any Jekyll website.

### Random notes
Reminder to compile and watch the changes:

```bash
bundle exec jekyll build --watch --source . --destination /var/www/ccs18/
```

and simple bash loop to check if the github repo has changed:
```bash
while true ; do git pull darnes master ; sleep 5 ; done 
```

Migrate to new year:
```bash
sed -i "s/ccs18/ccs18/g" *.md      
sed -i "s/Cancun/Thessaloniki/g" *.md 
```


