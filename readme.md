## (Mixture) Liquid support for Sublime Text

This is a fork of the [Siteleaf](https://github.com/siteleaf/liquid-syntax-mode) & [shopify-liquid](https://bitbucket.org/granteagon/shopify-liquid) syntax, which was based off of the Djaniero package for Django.

## Installation

1. Clone or Download this repo
2. Put the contents of this repo directly inside the Sublime Text packages directory (Submlime Text > Preferences > Browse Packages).

Or use PackageControl.

You might need to switch to the syntax mode. (`cmd + p`, search for Liquid, "Set Syntax: HTML (Liquid)")

## Autocomplete

To show the autocomplete suggestions, your cursor must be within a tag markup or output marker wrapper (`{% %}` or `{{ }}`) 

Then press `ctrl + spacebar`, or add the following to your user settings file:

```
"auto_complete_selector": "source - comment, text.html.liquid punctuation.output.liquid, text.html.liquid punctuation.tag.liquid"
```

## Example Snippets

**block**

```
block + tab >>>

{% block $1 %}{% endblock %}
```


**IF statement**

```
if + tab >>>

{% if $1 %}
  $2
{% endif %}
```

Check the "Snippets" folder for more.