See:
- https://github.com/mmistakes/minimal-mistakes
- https://jekyllrb.com/docs/installation/
- https://github.com/mmistakes/minimal-mistakes
- https://bundler.io/

## Preparataion
- Install Ruby
  - Need the one with devkit
  - Need to select MSYS2 dev toolchain
  - Windows RubyInstaller
    - https://rubyinstaller.org/downloads/
- Install bundler

gem install bundler

- Install jekyll

gem install jekyll bundler

## Installing barebone site
- Open git

cd /d/GitHub/nrt-impacts.github.io/
jekyll _3.8.5_ new .
bundle install
bundle update
bundle install
bundle exec jekyll serve

- Modified Gemfile
  - remove the "gem "jekyll"" above 
  - uncomment the line below and add "~> 202"
  - Run bundle update
  
bundle update github-pages

bundle exec jekyll serve

## Install theme
- Replace the current theme in your Gemfile with gem "jekyll-theme-clean-blog".
- Install the theme: 

bundle install

- Replace the current theme in your _config.yml file with theme: jekyll-theme-clean-blog.
- Build your site: 

bundle exec jekyll serve

## Convert gem-based theme into regular theme
- https://jekyllrb.com/docs/themes/

cp -r /c/Ruby26-x64/lib/ruby/gems/2.6.0/gems/minimal-mistakes-jekyll-4.16.5/* ./

- Based on gemespec, include these references in the Gemfile
  gem "jekyll", ">= 3.6", "< 5.0"
  gem "jekyll-paginate", "~> 1.1"
  gem "jekyll-sitemap", "~> 1.3"
  gem "jekyll-gist", "~> 1.5"
  gem "jekyll-feed", "~> 0.1"
  gem "jekyll-include-cache", "~> 0.1"

bundle update jekyll-sitemap
bundle install

## Trouble shoot
- Check jekyll dependency version:
  - https://pages.github.com/versions/
  - Ok, the version I install (4.0.0) is not what github is looking for
  - Install an older version

gem install jekyll -v 3.8.5

- Now create new site

jekyll 3.8.5 new .

- Get stuck with error "Could not locate Gemfile or .bundle/ directory"
  - Create a new gem file per:
    - https://forestry.io/docs/troubleshooting/could-not-locate-gemfile-or-bundle-directory/

bundle init

- Another error:
  - "can't find executable jekyll for gem jekyll. jekyll is not currently included in the bundle"
  - https://talk.jekyllrb.com/t/cant-create-a-new-test-site-w-jekyll/1989/4
  
bundle add jekyll 3.8.5

bundle exec jekyll _3.8.5_ new . --force

- The above does not seem to work properly, try:

jekyll _3.8.5_ new . --force

- Then modified the Gemfile
  - remove the "gem "jekyll"" above 
  - uncomment the line below and add "~> 202"
  - Run bundle update
  
bundle update github-pages

gem install github-pages

- Try again
  - https://rubygems.org/gems/github-pages/versions/202

bundle update github-pages

- Try to create a local site to test

bundle exec jekyll serve

- Run into error:
  - "... Could not find gem 'minima (~> 2.5) x64-mingw32' in any of the gem sources listed in your Gemfile"
  
gem install minima

- Try again

bundle exec jekyll serve

- Error: 
  - " Could not find gem 'github-pages x64-mingw32' in any of the gem sources listed in your Gemfile
  - Downgrade jekyll

gem install jekyll -v 3.8.5


