# `<details>`/`<summary>` jQuery plugin

This plugin polyfills `<details>`/`<summary>` HTML elements. [More information can be found in my blog post on the subject.](http://mathiasbynens.be/notes/html5-details-jquery)

## Demo & Examples

<http://mathiasbynens.be/demo/html5-details-jquery>

## Example Usage

```js
// Polyfill a given set of elements
$('details').details();
// Detect whether `<details>`/`<summary>` are natively supported
console.log($.fn.details.support ? 'Native support' : 'No native support');
```

## Notes

The plugin doesn’t require you to add any CSS to your document. It will add a `class="open"` to any open `<details>` elements though, so you can easily target these using CSS if you want.

This plugin includes my [noSelect jQuery plugin](http://mths.be/noselect).

This plugin automatically feature tests for native `<details>`/`<summary>` support and only enables the fallback when it’s necessary. You don’t have to write any feature tests yourself.

This fallback works in all A-grade browsers, including IE6. It will only be executed if the `<details>` element is not natively supported in the browser. If it isn’t, and JavaScript is disabled, all elements will still be visible to the user.

## License

This plugin is dual licensed under the MIT and GPL licenses, just like jQuery itself.

_– [Mathias](http://mathiasbynens.be/)_