# How to do a blogging

See [Jekyll's docs](https://jekyllrb.com/docs).
Also github pages docs.

High-level:
- posts go in `_posts/` and are named `YYYY-MM-DD-post-title.md`
- drafts go in `_drafts/` and no one will ever see them.

## local preview
To check it all goes before you push (thumbs up):
1. `> gem install bundler`  if you haven't already
2. `> bundle install` but probably only if it's your first time
3. `> bundle exec jekyll serve --watch` and go to town on it.
  - if you want to see drafts add the `--drafts` flag.

## writing stuff
posts should start with the following
[YAML front matter](https://jekyllrb.com/docs/frontmatter/):
```yaml
---
  layout: post
  title: Some post about a stuff.
---
```

Then just write _pro_ markdown like a hero.


## how to be less ugly

`index.html` is, unsurprisingly, the main page. It uses the default
layout which right now comes straight from the theme.

`_layouts/post.html` is the template for the individual posts.

To really look good we will probably want to make a `css/` folder
which will just get copied over and contain our styles. If we make
a `_sass` folder full of SASS then Jekyll will build those too,
and this could be positive.
