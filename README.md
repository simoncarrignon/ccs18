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

From easychair abstract to web:
With a bunch of vim subistitue commande it' s easy to modify the output given by easy chair export into a better one:  
then add the :s
```vim
%s#span class="title">#div class="title"></br><b>Title: </b>#g
```
Then one can the convert it with pandoc:
pandoc -s asbtract.html -o abstract.tex

And we some adjustment get a good latex output:

```vim
%s/^{/{\\textbf/g ''put the name of authors in bold
%s/^{\\bf/\\rule{4cm}{.4pt}\r\r{\\bf/g ''add a line betwee all abstrac
```
