# Bookmarklets

If you want to add a bookmarklet from a URL, then do the following, where `example.com` should be your url.

```js
javascript:var bookmarklet="http://example.com/";
document.getElementsByTagName('head')[0].appendChild(document.createElement('script')).setAttribute('src',bookmarklet);
```

If you want to want to append it to the body, do the following instead:

```js
javascript:var bookmarklet="http://example.com/";
(function(){document.body.appendChild(document.createElement('script')).src=bookmarklet})();
```
