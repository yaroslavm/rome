# rome-core

rome-core is the core library for generating, parsing and converting RSS and Atom feeds.

## Examples

### Generate

```java
SyndFeed feed = new SyndFeedImpl();
feed.setFeedType("rss_2.0");
feed.setTitle("title");
feed.setDescription("description");
feed.setLink("https://example.org");

System.out.println(new SyndFeedOutput().outputString(feed));
```

### Parse

```java
String url = "https://stackoverflow.com/feeds/tag?tagnames=rome";
SyndFeed feed = new SyndFeedInput().build(new XmlReader(new URL(url)));
System.out.println(feed.getTitle());
```

**Beware!** The `URL` class used in this example is rudimentary and works only for simplest cases. Please consider using a separate library for fetching the feed (see example in [#276](https://github.com/rometools/rome/issues/276)).

### Convert

TODO
