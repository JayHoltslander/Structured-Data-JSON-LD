# Structured Data - JSON-LD

[![Join the chat at https://gitter.im/Jays-Structured-Data/Lobby](https://badges.gitter.im/Jays-Structured-Data/Lobby.svg)](https://gitter.im/Jays-Structured-Data/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

## Contents

* **[Article](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/Article.json)** - If you’re a publisher website, the [NewsArticle](https://schema.org/NewsArticle) or [BlogPosting](https://schema.org/BlogPosting) schemas are recommended (choose one or the other, depending on your site/content). Leveraging these markups accordingly can help your content to appear in Google News and in-depth articles search suggestions. Google Resource Page: [Enabling Rich Snippets for Articles](https://developers.google.com/structured-data/rich-snippets/articles)
* **[BreadcrumbList.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/BreadcrumbList.json)** - The [BreadcrumbList schema](https://schema.org/BreadcrumbList) allows you to mark up the breadcrumbs on your site to generate breadcrumb rich snippets for your pages in the SERPs.
* **[Person.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/Person.json)** - My personal structured data snippet for "Person" in JSON-LD format. Results in [this](https://search.google.com/structured-data/testing-tool?url=https%3A%2F%2Fjay.holtslander.ca%2F#url=https%3A%2F%2Fjay.holtslander.ca%2F) detected entity.
* **[SiteNavigationElement](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/SiteNavigationElement.json)** - The [SiteNavigationElement schema](http://schema.org/SiteNavigationElement) can help increase search engines’ understanding of your site structure and navigation and can be used to influence organic sitelinks.
* **[WebSite](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/WebSite.json)** - The [WebSite schema](https://schema.org/WebSite) markup helps generate the Sitelinks Search Box feature for brand SERPs and can help your site name to appear in search results. You must, of course, have an existing site search on your website to enable the Sitelinks Search Box element.
* **[VideoObject](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/VideoObject.json)** - A site with embedded or hosted video content can leverage the VideoObject schema. Google primarily displays video rich snippets for YouTube videos, but this will help video rich snippets to appear for your Web pages in Google Video Search. Google Resource Page: [Enabling Rich Snippets for Videos](https://developers.google.com/structured-data/rich-snippets/videos)

## Installation
**A.)** Use [Google Tag Manager](https://www.google.com/analytics/tag-manager/) to insert the code with the "Custom HTML" tag. (See screenshot below.)

**B.)** Hand code it in.

**C.)** Use a Wordpress plugin of some type.

![](http://i.imgur.com/qVBR2kB.jpg)

## Testing
Wordpress users can use the awesome [Structured-Data-Test-Button Plugin](https://en-ca.wordpress.org/plugins/structured-data-test-button/), Yoast's Admin bar functions, or others. Everyone else can just visit the Google [Structured Data Test Tool](https://search.google.com/structured-data/testing-tool).
