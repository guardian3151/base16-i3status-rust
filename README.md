# base16-i3status-rust

This is a repository that provides a [base16](https://github.com/chriskempson/base16) template to generate theme
settings for [i3status-rust](https://github.com/greshake/i3status-rust).

The colors were chosen based on what [base16's website](http://chriskempson.com/projects/base16/) says about the
colors (both the example shades in the list saying what the colors are meant to be used for and _what_ it says they
are used for) and the colors of Solarized that the builtin theme chose. This is more optimised for dark themes, as a
result, so I may add another template that should work better for light themes. I'm also 100% open to switching around
what color goes where.

To use, update `themes/custom_theme.toml` with you base16 theme in your i3status-rust config directory (typically `XDG_CONFIG_HOME/i3status-rust`) and include `custom_theme` as a theme in your config as described in the [i3status-rust documentation](https://github.com/greshake/i3status-rust/blob/master/doc/themes.md).

`$XDG_DESKTOP_HOME/i3status-rust/config.toml`:
```toml
[theme]
theme = "custom_theme"
```
