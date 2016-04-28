# GitHub Directory
Generates a page of your GitHub repositories. Useful for a user/org GitHub Pages
site when you're not sure what to put there.

[![screenshot](http://i.imgur.com/m5Rt8pJ.png)](http://github-directory.surge.sh)

## Usage
Just fork this repository, then rename it `<your-username>.github.io`. You may need
to make a commit for GitHub to generate the site (just add a space to 
[`_config.yml`](_config.yml) or something).

**But** you'll need to make a change each time you create or change one of your repos,
so this page will regenerate.

Prefer to use a project page instead of a user/org page? You'll just have to rename
the `master` branch to `gh-pages`. You'll have to do that using the GitHub Desktop
application or at the command line though. :-/

You can change the way the repositories are sorted by editing
[`_config.yml`](_config.yml).

## How's it work?
GitHub Pages provides some [metadata](https://help.github.com/articles/repository-metadata-on-github-pages/)
to Jekyll in the `site.github` object, including a list of your repositories.
That's all there is to it, really.

## Development
To customize the theme or make other modifications, you may want to work on the site
locally. The GitHub Pages gem can simulate the GitHub Pages environment.

* Install [Jekyll](https://jekyllrb.com/docs/installation/)
* Fork this repo
* Install dependencies via `bundle install`
* Run the Jekyll site via `bundle exec jekyll serve`
