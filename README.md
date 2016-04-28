# GitHub Directory
Generates a page of your GitHub repositories. Useful for a user/org GitHub Pages
site when you're not sure what to put there.

[![screenshot](http://i.imgur.com/m5Rt8pJ.png)](http://timwis.com/github-directory)

## Usage
Just fork this repository and it will be available at
`<your-username>.github.io/github-directory/`.

To make it your user/org page, rename your fork `<your-username>.github.io`
and it will be available at `<your-username>github.io` (no suffix).

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
