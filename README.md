[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/chrisjagoda/iron-page-scroll)

_[Demo and API docs](https://elements.polymer-project.org/elements/iron-page-scroll)_


## &lt;iron-page-scroll&gt;

`iron-page-scroll` is used to select one of its children to scroll to. One use is to scroll between sections of a page.

Example:

```html
<iron-page-scroll>
  <div>One</div>
  <div>Two</div>
  <div>Three</div>
</iron-page-scroll>
```

It is also designed to be compatible with `iron selector`, being substitutible with `iron-pages`.

Example:

```html
<iron-selector attr-for-selected="name">
  <a name="view1">View One</a>
  <a name="view2">View Two</a>
  <a name="view3">View Three</a>
</iron-selector>

<iron-page-scroll>
  <div name="view1">One</div>
  <div name="view2">Two</div>
  <div name="view3">Three</div>
</iron-page-scroll>

<script>
  var pages = document.querySelector('iron-page-scroll#example-2');
  var selector = document.querySelector('iron-selector');
  selector.addEventListener('click', function(e) {
    pages.select(e.srcElement.name)
  });
</script>
```
