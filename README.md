# printable-slideshare
A bookmarklet to make stuff from SlideShare printable.

```js
javascript:var s=$('.slide_image').map(function(i,e){return $('<img>').attr('src',$(e).attr('data-full'))}).toArray(),c=s.length;$('body').css('background','#fff').empty().append(s);$('img').load(function(){--c||print()});
```
