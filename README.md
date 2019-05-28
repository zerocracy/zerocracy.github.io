<img src="https://www.0crat.com/svg/logo.svg" width="64px" height="64px"/>

[![Build Status](https://travis-ci.org/zerocracy/zerocracy.github.io.svg?branch=master)](https://travis-ci.org/zerocracy/zerocracy.github.io)

See [zerocracy.com](http://www.zerocracy.com).

This is a static website powered by [Jekyll](https://jekyllrb.com/). Every time you
push something to the `master` branch, [Travis](https://travis-ci.org/zerocracy/zerocracy.github.io) picks it up,
re-generates the site with Jekyll, and commits new version
to the `gh-pages` branch. Then, [GitHub Pages](https://pages.github.com/) re-publish the
content to [www.zerocracy.com](https://www.zerocracy.com).

## How to contribute

Read [these guidelines](https://www.yegor256.com/2014/04/15/github-guidelines.html).
Make sure you build is green before you contribute
your pull request. You will need to have [Ruby](https://www.ruby-lang.org/en/) 2.3+
and [Bundler](https://bundler.io/) installed. Then:

```bash
$ bundle update
$ bundle exec jekyll build
```

If it's clean and you don't see any error messages, submit your pull request.

To see how the site looks locally, run this:

```bash
$ bundle exec jekyll serve
```

Then, open the site in your browser via `http://localhost:4000`. Every time
you change the content, Jekyll will re-build the site. You can make your
changes on-fly.
