Themes proof of concept
=======================

This is a proof of concept for applying different color themes to a webpage, which can also load themes dynamically.

See it live at https://capacitorset.github.io/themes-proof-of-concept/!

## Usage

1. Install [SASS](http://sass-lang.com/install):

```
sudo gem install sass --no-user-install
```

2. Run the following:

```
/usr/bin/sass --scss --watch scss:css
```

To add new themes, you can simply create a new theme in the `scss/themes` folder, specifying the hue (which represents the "color" of your theme) and a name. You can find the hue from the color code with an [online calculator](http://serennu.com/colour/hsltorgb.php) (the hue is the first number in the "HSL:" row).

To add new style properties, edit `scss/_theme-base.scss`. If you specify colors, use the `_hsl` function, and pass the saturation and lightness values for the color you wish to use. Again, you can find these values from a color code [online](http://serennu.com/colour/hsltorgb.php).

> For example, if you want to use #0091EA (a bright blue) and have it change with the theme, you'd use `_hsl(100%, 46%)`. If you don't want it to change with the theme, use `#0091EA` directly.