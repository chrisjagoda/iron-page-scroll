[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/chrisjagoda/iron-page-scroll)

## &lt;iron-page-scroll&gt;

`iron-page-scroll` is used to select one of its children to scroll to and update the target on scrollover.

Example:

```html
<dom-bind>
  <template is="dom-bind">
    <iron-page-scroll selected={{page}}>
      <div>One</div>
      <div>Two</div>
      <div>Three</div>
    </iron-page-scroll>
  </template>
</dom-bind>  
```

It is also designed to be compatible with `iron selector`, being substitutible with `iron-pages`.

Example:

```html
<dom-bind>
  <template is="dom-bind">
    <iron-selector selected="{{page}}" attr-for-selected="name">
      <a name="view1">View One</a>
      <a name="view2">View Two</a>
      <a name="view3">View Three</a>
    </iron-selector>

    <iron-page-scroll selected="{{page}}" attr-for-selected="name">
      <div name="view1">One</div>
      <div name="view2">Two</div>
      <div name="view3">Three</div>
    </iron-page-scroll>
  </template>
</dom-bind>
```
