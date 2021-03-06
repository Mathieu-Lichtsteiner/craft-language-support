<!-- TODO Marketplace link -->

<h1>VS Code Craft Language Support</h1>

<!-- TODO Badges -->

- Syntax highlighting
- Snippets
- Emmet
- Pretty Diff 3 Formatting
- Hover

> Simply add these lines to your VS Code settings to get emmet working and also to associate HTML files as twig syntax.

```
"files.associations": {
    "*.html": "twig"
},
"emmet.includeLanguages": {
    "twig": "html"
},
```

## Installation

Install through Visual Studio Code extensions. Search for `Craft Language Support`

[Visual Studio Code Market Place: Craft Language Support](<!-- TODO Marketplace link -->)

## Documentation

Craft Language Support is a Visual Studio Code extension that provides snippets, syntax highlighting, hover, and formatting for the Twig file format.

### Twig syntax highlighting and language support

This extension provides language support for the Twig syntax.

### Information about Twig code on hover

VS Code Craft Language Support shows information about the symbol/object that's below the mouse cursor when you hover within Twig files.

### Craft CMS/Twig code snippets

Adds a set of Craft CMS/Twig code snippets to use in your Twig templates.

### Generic Triggers

```twig

do                {% do ... %}
extends           {% extends 'template' %}
from              {% from 'template' import 'macro' %}
import            {% import 'template' as name %}
importself        {% import _self as name %}
inc, include      {% include 'template' %}
incp              {% include 'template' with params %}
inckv             {% include 'template' with { key: value } %}
use               {% use 'template' %}

autoescape        {% autoescape 'type' %}...{% endautoescape %}
block, blockb     {% block name %} ... {% endblock %}
blockf            {{ block('...') }}
embed             {% embed "template" %}...{% endembed %}
filter, filterb   {% filter name %} ... {% endfilter %}
macro             {% macro name(params) %}...{% endmacro %}
set, setb         {% set var = value %}
spaceless         {% spaceless %}...{% endspaceless %}
verbatim          {% verbatim %}...{% endverbatim %}

if, ifb           {% if condition %} ... {% endif %}
ife               {% if condition %} ... {% else %} ... {% endif %}
for               {% for item in seq %} ... {% endfor %}
fore              {% for item in seq %} ... {% else %} ... {% endfor %}

else              {% else %}
endif             {% endif %}
endfor            {% endfor %}
endset            {% endset %}
endblock          {% endblock %}
endfilter         {% endfilter %}
endautoescape     {% endautoescape %}
endembed          {% endembed %}
endfilter         {% endfilter %}
endmacro          {% endmacro %}
endspaceless      {% endspaceless %}
endverbatim       {% endverbatim %}

```

### Craft Triggers

```twig
asset                    craft.assets.one()
assets, assetso          craft.assets loop
categories, categorieso  craft.categories loop
entries, entrieso        craft.entries loop
feed                     craft.app.feeds.getFeedItems loop
t                        | t
replace                  | replace('search', 'replace')
replacex                 | replace('/(search)/i', 'replace')
split                    | split('\n')
tags, tagso              craft.tags loop
users, userso            craft.users loop

cache                    {% cache %}...{% endcache %}
children                 {% children %}
exit                     {% exit 404 %}
ifchildren               {% ifchildren %}...{% endifchildren %}
css                      {% css %}...{% endcss %}
registercssfile          {% do view.registerCssFile("/resources/css/global.css") %}
js                       {% js %}...{% endjs %}
registerjsfile           {% do view.registerJsFile("/resources/js/global.js") %}
matrix, matrixif         Basic Matrix field loop using if statements
matrixifelse             Basic Matrix field loop using if/elseif
matrixswitch             Basic Matrix field loop using switch
nav                      {% nav item in items %}...{% endnav %}
paginate                 Outputs example of pagination and prev/next links
redirect                 {% redirect 'login' %}
requirelogin             {% requireLogin %}
requirepermission        {% requirePermission "spendTheNight" %}
switch                   {% switch variable %}...{% endswitch %}

csrf                     {{ csrfInput() }}
endbody                  {{ endBody() }}
head                     {{ head() }}

getparam                 craft.app.request.getParam()
getbodyparam             craft.app.request.getBodyParam()
getqueryparam            craft.app.request.getQueryParam()
getsegment               craft.app.request.getSegment()

case                     {% case "value" %}
endcache                 {% endcache %}
endifchildren            {% endifchildren %}
endcss                   {% endcss %}
endjs                    {% endjs %}
endnav                   {% endnav %}

ceil                     ceil()
floor                    floor()
max                      max()
min                      min()
shuffle                  shuffle()
random                   random()
round                    num | round()
url, urla                url('path'), url('path', params, 'http', false)

rss                      Example rss feed

dd                       <pre>{{ dump() }}</pre>{% exit %}
dump                     <pre>{{ dump() }}</pre>
```

## Author

???? **Mathieu Lichtsteiner**

- Github: [@Mathieu-Lichtsteiner](https://github.com/Mathieu-Lichtsteiner)

## ???? Contributing

Contributions, issues and feature requests are welcome !<br />Feel free to check [issues page](https://github.com/Mathieu-Lichtsteiner/craft-language-support/issues).

## Show your support

Give a ?????? if this project helped you !

## ???? License

Copyright ?? 2022 [Mathieu Lichtsteiner](https://github.com/Mathieu-Lichtsteiner).<br />
This project is [MIT](https://github.com/Mathieu-Lichtsteiner/craft-language-support/blob/master/LICENSE.md) licensed.
