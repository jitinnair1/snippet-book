# snippet-book

<p align="center">
<img src="https://snippets.jitin.xyz/assets/img/demo/composite.png" alt="Composite example of the Catppuccin theme for snippet-book"/>
</p>

`snippet-book` is a Jekyll blog theme based on [jekyll-theme-console](https://github.com/b2a3e8/jekyll-theme-console) with a few changes:

- Catpucchin theme defaults for light and dark mode
- User's preferred style (light/dark) is used by default

## Previews

<details>
<summary>🌻 Latte</summary>
<img src="https://snippets.jitin.xyz/assets/img/demo/latte.png" alt="Preview of Latte theme"/>
</details>
<details>
<summary>🪴 Frappé</summary>
<img src="https://snippets.jitin.xyz/assets/img/demo/frappe.png?raw=true" alt="Preview of Frappé theme"/>
</details>
<details>
<summary>🌺 Macchiato</summary>
<img src="https://snippets.jitin.xyz/assets/img/demo/macchiato.png?raw=true" alt="Preview of Macchiato theme"/>
</details>
<details>
<summary>🌿 Mocha</summary>
<img src="https://snippets.jitin.xyz/assets/img/demo/mocha.png?raw=true" alt="Preview of Mocha theme"/>
</details>


## Usage

### _config.yaml

In addition to jekyll's default configuration options, you can provide:
- `style_light` and `style_dark` to specify which predefined style (colors) should be used for light and dar modes

```yaml
style_light: "latte" # available options: latte, frappe, macchiato, mocha
style_dark: "macchiato" # available options: latte, frappe, macchiato, mocha
```

### front matter variables

Besides the predefined [front matter](https://jekyllrb.com/docs/front-matter/) variables from jekyll this theme also supports following variables:

- `title` to set a title for the page
- `lang` to specify the language, defaults to 'en'
- `robots` to control the robot meta tag ([details](http://longqian.me/2017/02/12/jekyll-robots-configuration/)) - this may be useful for example to set `NOINDEX` to tag pages

## Customization

If you want to customize this theme, follow this steps:
1. Fork this repository (you can use the fork as your own theme or directly as your website)
2. Create or modify files in `_layouts` directory for html-based changes
3. Create or modify files in `_sass` under `assets` for css-based changes
   - You can change things which are used in light and dark theme (like font-size) in `_sass/base.scss`. You'll find style variables at the top.
   - Catppuccin colours are under `assets/_sass/colours/_<name-of-theme>.scss`. These varaibles are then used to specify theme-specific colours in `_sass/theme/_theme-<name-of-theme>.scss`. 


## Development

To set up your environment to develop this theme, run `bundle install`.

Your theme is setup just like a normal Jekyll site! To test your theme, run `bundle exec jekyll serve` and open your browser at `http://localhost:4000`. This starts a Jekyll server using your theme. Add pages, documents, data, etc. like normal to test your theme's contents. As you make modifications to your theme and to your content, your site will regenerate and you should see the changes in the browser after a refresh, just like normal.

## License

The theme is available as open source under the terms of the [MIT License](https://opensource.org/licenses/MIT).

PS: If you liked the theme, do star :star: it! Thanks!

### Also, check out:

- [autoCV](https://github.com/jitinnair1/autocv) - a LaTeX template that builds and deploys the CV using GitHub Actions, so you will always have a ready link for your latest CV
- [gradfolio](https://github.com/jitinnair1/gradfolio) - a minimal, quick-setup template for a personal website/portfolio
- [Tail](https://github.com/jitinnair1/tail) - a minimal, quick-setup template for a blog
