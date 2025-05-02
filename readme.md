# bx-rss

I built this after learning about BoxLang modules a whole hour ago so take with a Titanic-sized piece of salt. I'll add
more info on this soon, but in theory, if you copy the `boxlang_modules` folder to your web app, or just the `rss` folder to your system module directory, you get will support for the following BIF function: `rss`

The `rss` function takes one argument, either a URL, or an array of URL.

```js
items = rss('https://www.raymondcamden.com/feed_slim.xml');

// or
items = rss(['https://www.raymondcamden.com/feed_slim.xml','https://2ality.com/feeds/posts.atom']);
```

It returns an array of feed items consisting of the keys: `title`, `content`, `pubdate`, `link`. If you pass an array of RSS urls, the items are automatically sorted and merged together by date.

