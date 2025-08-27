How to run blog on a windows machine:

wsl
->
(if not added earlier) add aliases
alias startblog='rsync -avh --delete /mnt/c/Users/kosel/dev/github/nikitakoselev.github.io/ ~/blog/ && cd ~/blog && bundle exec jekyll serve'
alias syncblog='rsync -avh --delete /mnt/c/Users/kosel/dev/github/nikitakoselev.github.io/ ~/blog/'
->
startblog


=======
# Tech Edge Intrapreneur Blog

This repository contains the source code for the Tech Edge Intrapreneur blog powered by [Jekyll](https://jekyllrb.com/) and GitHub Pages.

## Running locally on Windows

The recommended way to run the site locally on a Windows machine is to use the [Windows Subsystem for Linux (WSL)](https://learn.microsoft.com/windows/wsl/).

1. Install WSL and a Linux distribution (Ubuntu is recommended).
2. Install Ruby and Bundler:
   ```bash
   sudo apt update
   sudo apt install ruby-full build-essential zlib1g-dev
   gem install bundler
   ```
3. Clone the repository and enter it:
   ```bash
   git clone https://github.com/nikitakoselev/nikitakoselev.github.io.git
   cd nikitakoselev.github.io
   ```
4. Install dependencies into a local path to keep them isolated:
   ```bash
   bundle install --path vendor/bundle
   ```
5. Build and serve the site:
   ```bash
   bundle exec jekyll serve
   ```
6. Open [http://localhost:4000](http://localhost:4000) in your browser to view the blog.

The site will rebuild automatically as you edit files.

For other Windows setups, you can use [RubyInstaller](https://rubyinstaller.org/) and run the same `bundle` and `jekyll` commands in a command prompt with Ruby available.

## License

[Creative Commons Attribution-NonCommercial 4.0 International](LICENSE)