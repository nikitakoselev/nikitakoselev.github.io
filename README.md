How to run blog on a windows machine

wsl
->
(if not added earlier) add aliases
alias startblog='rsync -avh --delete /mnt/c/Users/kosel/dev/github/nikitakoselev.github.io/ ~/blog/ && cd ~/blog && bundle exec jekyll serve'
alias syncblog='rsync -avh --delete /mnt/c/Users/kosel/dev/github/nikitakoselev.github.io/ ~/blog/'
->
startblog