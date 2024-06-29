# Toan Nguyen Homepage [http://www.toaninfo.com](http://www.toaninfo.com)

Generated by Jekyll

## Install Jekyll (MacOS)

https://jekyllrb.com/docs/installation/macos/

```
brew install chruby ruby-install

ruby-install 3.1.2 -- --enable-shared

echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
echo "chruby ruby-3.1.2" >> ~/.zshrc # run 'chruby' to see actual version

gem install github-pages
gem install jekyll
gem install jekyll-feed
bundle update
```

## Install
```
cd toaninfo
sudo bundle install
```

## Run on localhost to test**
```
bundle exec jekyll serve
```

## Build to docs**
```
JEKYLL_ENV=production bundle exec jekyll build -d docs
cp CNAME docs
```
