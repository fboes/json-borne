JSON-borne
==========

Why invent a new JSON structure for your application if there are already tons of well-documented and interoperable JSON data structures? This repository is an ever growing list of well-defined JSON data sets.

Why do we need well-defined JSON data sets?
-------------------------------------------

JSON ist not only about storing your data. It is also about communication. Javascript in browsers can directly parse JSON, and JSON offered via REST-APIs can be parsed by almost any programming language effortlessly. Using the same data structure for the same type of content allows you to have your data interoperable with another service you might not yet have thought of.

General conversions & validation
--------------------------------

* There is a [general way to convert XML data structures into JSON data structures](http://blog.3960.org/post/8478676503/rss-mit-json).
* There is a [discussion about how to format dates in JSON](http://stackoverflow.com/questions/10286204/the-right-json-date-format). The two favoured options are timestamps (e.g. `1476695864`) or Javascript's Date representation (e.g. `2012-04-23T18:25:43.511Z`).
* [JSON-LD](http://json-ld.org/) is used by Google Knowledge Graph, and describes lots of structured data. See also ["Why JSON-LD"](http://jsonld.com/why-json-ld/).
* For rich text you may want to use [Markdown](https://daringfireball.net/projects/markdown/), as there are tons of parsers for this format.

### Schema

* [JSON Schema](http://json-schema.org/) is a vocabulary that allows you to annotate and validate JSON documents.
* There is a [JSON schema generator](http://jsonschema.net/#/).
* There is a list of schemas at the [JSON schema store](http://schemastore.org/json/).

Data formats
------------

###  Syndication

* [JSON-RSS](http://scripting.com/stories/2012/09/10/rssInJsonForReal.html) as proposed by Dave Winer himself converts the true and trusted RSS into JSON. Currently there is no service out there to digest this information, but it is a convenient way to offer your published articles via REST-API. There is also a [live example for JSON-RSS](http://blog.3960.org/post/8478676503/rss-mit-json) and a [JSON-RSS schema](schemas/json-rss.json).
* [JSON-Sitemap](sitemap.json) tries to output [XML-Sitemaps](http://www.sitemaps.org/de/protocol.html) in JSON. This may be useful to have a list of all URLs in a given domain.
* [Slack Message-API](https://api.slack.com/docs/message-attachments) with [Slack Message-Builder](https://api.slack.com/docs/messages/builder)

### Articles

* [Apple News Article](https://developer.apple.com/library/content/documentation/General/Conceptual/Apple_News_Format_Ref/StructureOverview.html) lets you describe articles in JSON. These articles can be read by Apple News.
* [JSON-LD for Blog Posts](http://jsonld.com/blog-post/)
* [JSON-LD for Articles](http://jsonld.com/article/)

### Calendar & Events

* [ICS-JSON](calendar.json) is a simple conversion of the ICS calendar format to JSON. All property keys are converted into lowercases. For everything else the structure is kept.
* [JSON-LD for Events](http://jsonld.com/event/)

### Geolocation and places

* [GeoJSON](http://geojson.org/) lets you store geometric points, lines and polygons much like KML. It can be read by[ Google Maps](https://developers.google.com/maps/documentation/android-api/utility/geojson?hl=de) and [Leaflet](http://leafletjs.com/examples/geojson/).

### Messaging

* [JSON-LD for E-Mails](http://jsonld.com/email-message/)
* [Slack Message-API](https://api.slack.com/docs/message-attachments) with [Slack Message-Builder](https://api.slack.com/docs/messages/builder)

Contributing
------------

I am happy to merge your contributions to this repository.

Legal stuff
-----------

Author: [Frank Boës](http://3960.org)

Copyright & license: See [LICENSE.txt](LICENSE.txt)
