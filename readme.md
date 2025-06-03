# ⚡︎ RSS

Basic RSS parsing forBoxLang. This module adds one BIF, `rss`. 

The `rss` function takes one argument, either a URL, or an array of URLs.

```js
items = rss('https://www.raymondcamden.com/feed_slim.xml');

// or
items = rss(['https://www.raymondcamden.com/feed_slim.xml', 'https://2ality.com/feeds/posts.atom']);
```

It returns an array of feed items consisting of the keys: `title`, `content`, `pubdate`, `link`. If you pass an array of RSS urls, the items are automatically sorted and merged together by date.

## Release History

| Date | Change |
| ---- | ----- |
| June 3, 2025 | Moved to new template structure for Forgebox support. |
| May 5, 2025 | Moved the creation of the RSS object to the `init` method. |

