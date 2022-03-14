This fork contains my modifications to logseq dev theme.

1. Increase the main content width
2. Remove unnecessary navigation items, i.e. items that I don't use like "Recent" in the left sidebar, "Join the community" under the top-... dropdown, etc.
3. Move the back/forward page arrows to the left side of the toolbar
4. Decrease the empty line gap for in-line code blocks
5. Reduce the whitespace (darkspace for dark theme) in the right sidebar
6. Adjust height of youtube video embeds
7. Change the "highlight" to actual highlight instead of an underline
8. (Most trivial one) Increase the default font size because I've an amazing eyesight.

--------------------------------
ORIGINAL README
--------------------------------

# Logseq Dev Theme

A theme inspired by Dev.to & Figma.

<img src="./logo.png" width="100" />

## Working Demo

https://pengx17.github.io/knowledge-garden/

## Usage

### Marketplace
This theme and bullet threading are available in the Marketplace.

![](./marketplace.png)

### Using custom.css

The easiest way to adopt this theme is to use jsDelivr CDN by adding the following line to your `custom.css`. You can also change the `@main` part to use the latest version.

```css
/* This must be the first line of the custom.css with other import rules */
@import url("https://cdn.jsdelivr.net/gh/pengx17/logseq-dev-theme@main/custom.css");

/* You can also add other styles below to override the default theme values */
```

Alternatively, you can download this repo and load it as a Logseq Theme Plugin.

### Only use bullet threading styles

Since version `1.20.0`, you can opt in with the only the bullet threading css, which is `bullet_threading.css`.
To change the color and width, set the following variables in `custom.css`:

```css
@import url("https://cdn.jsdelivr.net/gh/pengx17/logseq-dev-theme@main/bullet_threading.css");

:root {
  --ls-block-bullet-active-color: your-favorite-color;
  --ls-block-bullet-threading-width: 2px;
}
```

#### Caveats

If your theme defines border colors for the `children-block`, the bullet threading css may not work as expected.

### [Changelog](./CHANGELOG.md)

## Credits

[PiotrSss](https://github.com/PiotrSss) for his [clean-themes](https://github.com/PiotrSss/logseq-clean-themes)
