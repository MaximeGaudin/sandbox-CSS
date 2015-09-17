# CSS Best practice and Pro Tips

Based on the following resources : 

* https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Writing_efficient_CSS#How_the_style_system_breaks_up_rules
* http://www.innofied.com/25-css-best-practices-we-follow-at-innofied/
* http://sass-lang.com/documentation/file.SASS_REFERENCE.html
* http://htmldog.com/reference/cssproperties/

I tried to improve my understanding of how CSS work and on how I can make it work better _i.e._ faster and with a lower cost of maintenance).

## Obvious rules

* No inline styles
* Use SASS
* Use a reset stylesheet (TODO: Which one ??)

## Golden rules 

### Selectors

* No universal rules
* If possible, no tag name qualifier (_e.g._ `button.admin`, prefer to embed it into the class name like `.button-admin`)
* Write you rule so it uses the least number of selector
* Avoid the descendant selector (_e.g._ `div h1`) and prefer the child selector 
* For custom view, prefer specialized classes to child selector
* Learn property inheritance and rely on it to remove useless and expensives css rules

### Pragmatic

* Keep a color reference in a separated stylesheet. Beside the obvious maintenance benefir, you will be able to publish several color schemes quiet quickly without changing anything but this file.
* Lean which element are block element, and which are inline. Also, be very familiar with the following display : `block`, `inline`, `inline-block`, `table`

TODO: Get the list of inherted CSS properties

