---
title: Sitepress
---

Sitepress is a set of tools that helps you build awesome websites. It is not *soley* a static site generator. It can be embedded in other web frameworks like Rails, it can run stand-alone in a rack server, or you could use it to build your own static site generator.

## Why Sitepress?

Static site generators, like [Middleman](https://middlemanapp.com) and [Jekyll](https://jekyllrb.com), are great frameworks for compiling static websites and publishing them to the web, but what if you need to run a content site from within Rails or Sinatra that needs to have access to a database? Unfortunately most static site generators come bundled with the kitchen sink, so its really hard to embed them.

### Sitepress goals

* **[Minimal dependencies](https://github.com/sitepress/sitepress/blob/master/sitepress/sitepress.gemspec#L24)** - Sitepress ships with as few dependencies as possible so that it may be embedded in other web frameworks without creating rubygem conflicts.

* **Composability** - Sitepress is broken apart into several gems that are optimized for their environments. For example, the `sitepress-rails` gem uses as much of the rendering infrastructure from Rails as possible.

* **Speed** - Sitepress is benchmarked using a 10,000 page site as part of a regular test suite. Performance and speed is a goal of this project.