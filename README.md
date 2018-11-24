# plain-html-blog
*plain-html-blog* is a very clean, minimal [Jekyll][jekyll] blog that works without CSS. It was inspired by websites which (for valid reasons) still make minimal use of styling with CSS and the like.

You can see it live right here: [https://sebbas.org][sebbas]

![screenshot-plain-html-blog][screenshot]

## Installation

1. [Fork this repository][fork]
2. Clone it: `git clone git@github.com:yourusername/plain-html-blog.git`
3. Install ruby things: `bundle install` (if this doesn't work, look into [installing Bundler][bundler])
4. Start it up: `jekyll serve -w`

You should have a server up and running locally at <http://localhost:4000>.

### Optional

If you would like to have the `updated` field (used to show the last modification date in the footer) in the YAML front matter to update automatically each time the page was modified and you make a commit, then symlink the executable `pre-commit` script ([scripts/pre-commit][precommit]) to your `.git/hooks`. You can do this by running

`ln -s -f ../../scripts/pre-commit .git/hooks/pre-commit`

## Customization

1. [_config.yml][config]: Your email, personal information and usernames should go here.
2. [CNAME][cname]: Want to use a custom domain? Just place yours in here.
3. [images/][images]: If you have a photo or icon you'd like to use I recommend generating `favicon`, `apple-touch-icon.png` and the like with an online icon generator (just google for one). Place all generated images and files in this directory and, if necessary, adapt the paths in [_includes/head.html][head]

## Deployment

This blog is all set for use with Github (it's not using any additional Jekyll plugins). So all you have to do is rename your repository to `username.github.io`. Your site will be available at [https://yourusername.github.io][githubio]

[sebbas]: https://sebbas.org
[jekyll]: https://jekyllrb.com
[screenshot]: https://dl.dropboxusercontent.com/s/jbb5nfdas6h400b/screenshot_plain_html_blog.png
[stallman]:   https://stallman.org
[graham]: http://www.paulgraham.com/index.html
[motherfuckingwebsite]: https://motherfuckingwebsite.com
[source-code-blog]: https://github.com/sebbas/plain-html-blog
[fork]: https://github.com/sebbas/plain-html-blog/fork
[bundler]: https://bundler.io
[precommit]: https://github.com/sebbas/plain-html-blog/blob/master/scripts/pre-commit
[config]: https://github.com/sebbas/plain-html-blog/blob/master/_config.yml
[cname]: https://github.com/sebbas/plain-html-blog/blob/master/CNAME
[images]: https://github.com/sebbas/plain-html-blog/tree/master/images
[head]: https://github.com/sebbas/plain-html-blog/blob/master/_includes/head.html
[githubio]: https://username.github.io
