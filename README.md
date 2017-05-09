# \<sortable-list\>

Polymer 1.X and 2.X custom element for drag-and-drop reorder of items.

For typical use just wrap your dom-repeat template item with a `<sortable-list>`
element to get drag-and-drop reordering.

Relies on
[HTML 5 drag and drop](https://developer.mozilla.org/en-US/docs/Web/API/HTML_Drag_and_Drop_API)
browser support, so if you need to support older browsers
which do not support HTML 5 drag and drop events then we suggest using a polyfill:

https://github.com/Modernizr/Modernizr/wiki/HTML5-Cross-Browser-Polyfills

## Install

```shell
bower install --save polymer-sortable-list
```

## Usage

<!--
```
<custom-element-demo height="200">
  <template>
    <link rel="import" href="sortable-list.html">
    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<sortable-list>
  <template is="dom-repeat" items='["item 1","item 2","item 3","item 4"]'>
    <div style="height:30px;cursor:pointer;">[[item]]</div>
  </template>
</sortable-list>
```

## Viewing This Element

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve this element locally.

```
$ polymer serve
```

## Running Tests

```
$ polymer test
```
