# just-the-docs-template

This site is available at : 
https://gaiaviz.github.io/docs/

The documentation uses Just-the-docs Jekyll theme, documented here:
https://just-the-docs.github.io/just-the-docs/

If you want to maintain your docs in the `docs` directory of an existing project repo, see [Hosting your docs from an existing project repo](#hosting-your-docs-from-an-existing-project-repo).

- `index.md` (your new home page)
- `README.md` (information for those who access your site repo on GitHub)

## Changing the version of the theme and/or Jekyll

Simply edit the relevant line(s) in the `Gemfile`.

## Adding a plugin

The Just the Docs theme automatically includes the [`jekyll-seo-tag`] plugin.

To add an extra plugin, you need to add it in the `Gemfile` *and* in `_config.yml`. For example, to add [`jekyll-default-layout`]:

- Add the following to your site's `Gemfile`:

  ```ruby
  gem "jekyll-default-layout"
  ```

- And add the following to your site's `_config.yml`:

  ```yaml
  plugins:
    - jekyll-default-layout
  ```

Note: If you are using a Jekyll version less than 3.5.0, use the `gems` key instead of `plugins`.

----

[Jekyll]: https://jekyllrb.com
[Just the Docs]: https://just-the-docs.github.io/just-the-docs/

[`jekyll-default-layout`]: https://github.com/benbalter/jekyll-default-layout
[`jekyll-seo-tag`]: https://jekyll.github.io/jekyll-seo-tag
