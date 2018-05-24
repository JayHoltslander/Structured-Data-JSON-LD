# Structured Data - JSON-LD

[![Join the chat at https://gitter.im/Jays-Structured-Data/Lobby](https://img.shields.io/gitter/room/nwjs/nw.js.svg)](https://gitter.im/Jays-Structured-Data/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) ![](https://img.shields.io/chrome-web-store/stars/nimelepbpejjlbmoobocpfnjhihnpked.svg) [![](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](http://www.twitter.com/share?text=Great+collection+of+structured+data+snippets+in+JSON-LD+format+by+@j_holtslander&url=https://github.com/JayHoltslander/Structured-Data-JSON-LD)

Structured Data is hard when you're starting out. Conflicting info. Old outdated information. Poor documentation. I've spent a significant amout of time trying to master it. Now you can benefit from all my hard work and testing. Everything here works properly or it wouldn't be here. Many of these will provide the [fancy Google Search Enhancements](https://developers.google.com/search/docs/guides/search-gallery) you desire and ensure your content types are marked up properly.

## Contents

### [AggregateRating.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/AggregateRating.json)
An average rating based on multiple ratings or reviews utilizing the [AggregateRating schema](http://schema.org/AggregateRating). Be sure to read [this article](https://whitespark.ca/blog/how-to-use-aggregate-review-schema-to-get-stars-in-the-serps/) to see why using this example as written might not be the best idea. Hmm. 🤔 Also note that using a 3rd party's ratings (like say Google or Yelp) for a [localBusiness](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/LocalBusiness.json) goes against [Google's guidelines](https://developers.google.com/search/docs/data-types/review#review-snippet-guidelines).
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/AggregateRating.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FAggregateRating.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22AggregateRating%22/)
<br><br>

### [Article.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/Article.json)
If you’re a publisher website, the more specific schema types like [NewsArticle](https://schema.org/NewsArticle) or [BlogPosting](https://schema.org/BlogPosting) are recommended (choose one or the other, depending on your site/content). Leveraging these markups accordingly can help your content to appear in Google News and in-depth articles search suggestions. See: [Enabling Rich Snippets for Articles](https://developers.google.com/structured-data/rich-snippets/articles). **Note:** To show up in Google's News Carousel not only will the page require Structured Data but it's also [required to be a valid AMP page](https://developers.google.com/search/docs/data-types/article). If you are using the [official AMP Plugin for Wordpress](https://en-ca.wordpress.org/plugins/amp/) you will definitely want to use Tag Manager to insert your Structured Data as opposed to other methods since you will be able to [dynamically generate Schema.org JSON-LD Tags](https://moz.com/blog/using-google-tag-manager-to-dynamically-generate-schema-org-json-ld-tags) from pages that contain the correct pattern for your posts. **eg:** ``?amp=1`` or ``/amp``
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/Article.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FArticle.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22Article%22/)
<br><br>


### [BlogPosting](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/BlogPosting.json)
An even more specific version of Article for a blog post. See the [BlogPosting schema](http://schema.org/BlogPosting) for more info.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FBlogPosting.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22BlogPosting%22/)
<br><br>


### [BreadcrumbList.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/BreadcrumbList.json)
The [BreadcrumbList schema](https://schema.org/BreadcrumbList) allows you to mark up the breadcrumbs on your site to generate breadcrumb rich snippets for your pages in the SERPs. [Learn more](https://developers.google.com/search/docs/data-types/breadcrumb).
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/BreadcrumbList.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22BreadcrumbList%22/)
<br><br>


### [Course.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/Course.json)
The [Course schema](https://schema.org/Course) allows you to mark up courses on your site to generate rich snippets for your courses in the SERPs. [Learn more](https://developers.google.com/search/docs/data-types/course).
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FCourse.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22Course%22/)
<br><br>


### [Dataset.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/Dataset.json)
The [Dataset schema](https://schema.org/Dataset) is for a body of structured information describing some topic(s) of interest. It should use the sameAs property to link to the canonical page.  [Learn more](https://developers.google.com/search/docs/data-types/dataset).
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FDataset.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22Dataset%22/)
<br><br>


### [ImageObject.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/ImageObject.json)
An example of the [ImageObject](http://schema.org/ImageObject) schema. Demonstrates use of the [exifData](http://schema.org/exifData) schema.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FImageObject.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22ImageObject%22/)
<br><br>


### [ItemList-1.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/ItemList-1.json)
The [ItemList](http://schema.org/ItemList) schema makes a page's items eligible for the [Carousel Feature](https://developers.google.com/search/docs/guides/mark-up-listings) on mobile devices ([Screenshot](https://developers.google.com/search/docs/guides/images/search-features03-HostCarousel.png)). This example is for a summary page which has a short description of each item in the list, and each item points to a separate details page that is focused entirely on one item. The details page is where the more detailed Structured Data on the item would be located. See: Docs https://developers.google.com/search/docs/guides/mark-up-listings#summary-page--multiple-full-details-pages
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/ItemList-1.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22ItemList%22/)
<br><br>


### [ItemList-2.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/ItemList-2.json)
The [ItemList](http://schema.org/ItemList) schema makes a page's items eligible for the [Carousel Feature](https://developers.google.com/search/docs/guides/mark-up-listings) on mobile devices ([Screenshot](https://developers.google.com/search/docs/guides/images/search-features03-HostCarousel.png)). This example is for a single, all-in-one-page list hosts all list information, including full text of each item: for example, a gallery of recipes for various kinds of muffins, all contained on one page.
See: Docs https://developers.google.com/search/docs/guides/mark-up-listings#single-all-in-one-page-list
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/ItemList-2.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22ItemList%22/)
<br><br>


### [ItemList-3.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/ItemList-3.json)
The [ItemList](http://schema.org/ItemList) schema makes a page's items eligible for the [Carousel Feature](https://developers.google.com/search/docs/guides/mark-up-listings) on mobile devices ([Screenshot](https://developers.google.com/search/docs/guides/images/search-features03-HostCarousel.png)). This example shows usage with the [CollectionPage](http://schema.org/CollectionPage) schema. 
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/ItemList-3.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22ItemList%22/)
<br><br>


### [JobPosting.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/JobPosting.json)
Adding structured data makes your job postings eligible to appear in a special user experience in Google Search results leading to increased chances of discovery and conversion. Your postings are eligible to be displayed more prominently in the dedicated Job Search UI, featuring your logo, reviews, ratings, and job details. The new user experience enables job seekers to filter by various criteria like location or job title, meaning you’re more likely to attract applicants who are looking exactly for that job. [Learn more](https://developers.google.com/search/docs/data-types/job-posting).
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool/u/0/?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/JobPosting.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FJobPosting.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22JobPosting%22/)
<br><br>


### [LocalBusiness.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/LocalBusiness.json)
An example of a LocalBusiness with multiple locations defined. Each location having it's own defined service areas.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FLocalBusiness.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22LocalBusiness%22/)
<br><br>


### [LocalBusiness-2.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/LocalBusiness-2.json)
An example of a LocalBusiness customized for a law firm. Demonstrates combined @types (LocalBusiness/Organization/LegalService) and [Corporate Contact](https://developers.google.com/search/docs/data-types/corporate-contact) useage.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FLocalBusiness-2.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22LocalBusiness%22/)
<br><br>


### [LocalBusiness-3.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/LocalBusiness-3.json)
A detailed example of a complex LocalBusiness customized for a Notary. Demonstrates combined @types (LocalBusiness/Organization/Notary) and [Corporate Contact](https://developers.google.com/search/docs/data-types/corporate-contact) useage.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FLocalBusiness-3.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22LocalBusiness%22/)
<br><br>


### [LocalBusiness-4.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/LocalBusiness-4.json)
An example of a LocalBusiness customized for an online store with no physical location. Demonstrates combined @types (LocalBusiness/Organization/Store)
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FLocalBusiness-4.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22LocalBusiness%22/)
<br><br>


### [Person.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/Person.json)
My personal structured data snippet for "Person" in JSON-LD format.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/Person.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FPerson.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22Person%22/)
<br><br>


### [Question-w-Answers.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/Question-w-Answers.json)
An example of some markup that results in Rich Snippets for Questions as observed in the wild being used on [Stack Exchange websites](https://stackexchange.com/sites). [SERP Screenshot](http://cdn.skunkworks.ca.s3.amazonaws.com/temp-screenshots/Screen_Shot_2017-12-07_at_11.44.40_AM.png) This example includes additional Schema types for "Answer" and "QAPage" which do not seem to be required but complement each other.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FQuestion-w-Answers.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22QAPage%22/)
<br><br>


### [Service.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/Service.json)
A collection of services that a LocalBusiness may provide with per/service ratings.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/Service.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FService.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22Service%22/)
<br><br>


### [ServiceArea](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/ServiceArea.json)
How to define a service area for a local business.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FServiceArea.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22ServiceArea%22/)
<br><br>


### [SiteNavigationElement.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/SiteNavigationElement.json)
The [SiteNavigationElement schema](http://schema.org/SiteNavigationElement) can help increase search engines’ understanding of your site structure and navigation and can be used to influence organic sitelinks. (See also WPHeader on this page for an example of usage within a Navbar!)
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/SiteNavigationElement.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FSiteNavigationElement.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22SiteNavigationElement%22/)
<br><br>


### [SpeakableSpecification](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/SpeakableSpecification.json)
For Voice search a SpeakableSpecification indicates via css selector(s) sections of a document that are highlighted as particularly speakable. See [this article](https://translate.google.com/translate?hl=en&sl=auto&tl=en&u=https%3A%2F%2Fwww.effektiv.com%2Fready-for-voice-search-strukturierte-daten-nach-schema-org-verfuegbar-4464.html) for more info.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FSpeakableSpecification.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22SpeakableSpecification%22/)
<br><br>


### [WebSite.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/WebSite.json)
The [WebSite schema](https://schema.org/WebSite) markup helps generate the Sitelinks Search Box feature for brand SERPs and can help your site name to appear in search results. You must, of course, have an existing site search on your website to enable the Sitelinks Search Box element.<br>
Includes:
  * the [Webpage](http://schema.org/WebPage) schema. Why both? See [this description](https://stackoverflow.com/a/29889156/751570).)
  * WPHeader
  * WPSidebar
  * WPFooter
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/WebSite.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22Website%22/)
<br><br>


### [WPHeader.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/WPHeader.json)
("Webpage Header" not "Wordpress Header") Define structured Data for items within a site's header with the [WPHeader schema](http://schema.org/WPHeader). Includes SiteNavigationElements within! Also see an example of this in use within the snippet [WebSite.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/WebSite.json)
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FWPHeader.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22WPHeader%22/)
<br><br>


### [VideoObject.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/VideoObject.json)
A site with embedded or hosted video content can leverage the VideoObject schema. Google primarily displays video rich snippets for YouTube videos, but this will help video rich snippets to appear for your Web pages in Google Video Search. Google Resource Page: [Enabling Rich Snippets for Videos](https://developers.google.com/structured-data/rich-snippets/videos)
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/VideoObject.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FVideoObject.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22VideoObject%22/)
<br><br>


### [ViewAction](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/ViewAction.json)
Indicates where something should be viewed. One of the most common implementations is in Google App indexing, where it enables a URL from a website indexed in search results, to be opened inside the corresponding App (if installed in the user's device).
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/ViewAction.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FViewAction.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%22%3A%22ViewAction%22/)
<br><br>

---

## Tips & Tricks
You can link snippets together and reuse them ([DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)) by defining and referencing their ``@id`` (These are called "Node identifiers") Learn more about them [here](https://webmasters.stackexchange.com/a/98578/77742).

## Installation
**A.)** Use [Google Tag Manager](https://www.google.com/analytics/tag-manager/) to insert the code with the "Custom HTML" tag. (See screenshot below.) Why Tag Manager? Because Tag Manager can dynamically change the Structured Data based on the content of the page! (eg: Blog posts) See [this article](https://moz.com/blog/using-google-tag-manager-to-dynamically-generate-schema-org-json-ld-tags) for more information on how to do that.
  * [Add schema markup site using Google Tag Manager](https://searchengineland.com/add-schema-markup-site-using-google-tag-manager-272516)
  * [Adding JSON-LD structured data with Google Tag Manager](https://yoast.com/structured-data-google-tag-manager/)

**B.)** Hand code it in and manually keep it up to date. (Ugh)

**C.)** Use a Wordpress plugin of some type.

![](http://i.imgur.com/qVBR2kB.jpg)

## To-do
* [x] ~~[SiteNavigationElement](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/README.md#sitenavigationelementjson)~~
* [ ] [Table](http://schema.org/Table) ([Examples](https://publicwww.com/websites/%22%5C%22%40type%5C%22%3A%5C%22Table%5C%22%22/))
* [ ] [WPAdBlock](http://schema.org/WPAdBlock) ([Examples](https://publicwww.com/websites/%22%5C%22%40type%5C%22%3A%5C%22AdBlock%5C%22%22/))
* [x] ~~[Website](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/README.md#websitejson)~~
  * [x] ~~[WPFooter](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/README.md#websitejson)~~
  * [x] ~~[WPSideBar](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/README.md#websitejson)~~
  * [x] ~~[WPHeader](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/README.md#wpheaderjson)~~
  * [ ] [CheckoutPage](http://schema.org/CheckoutPage) ([Examples](https://publicwww.com/websites/%22%5C%22%40type%5C%22%3A%5C%22CheckoutPage%5C%22%22/))
  * [ ] [ContactPage](http://schema.org/ContactPage) ([Examples](https://publicwww.com/websites/%22%5C%22%40type%5C%22%3A%5C%22ContactPage%5C%22%22/))
  * [ ] [AboutPage](http://schema.org/AboutPage) ([Examples](https://publicwww.com/websites/%22%5C%22%40type%5C%22%3A%5C%22AboutPage%5C%22%22/))
  * [x] ~~[QAPage](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/README.md#question-w-answersjson)~~
  * [ ] [CollectionPage](http://schema.org/CollectionPage) ([Examples](https://publicwww.com/websites/%22%5C%22%40type%5C%22%3A%5C%22CollectionPage%5C%22%22/))
  * [ ] [ItemPage](http://schema.org/ItemPage) ([Examples](https://publicwww.com/websites/%22%5C%22%40type%5C%22%3A%5C%22ItemPage%5C%22%22/))
  * [ ] [ProfilePage](http://schema.org/ProfilePage) ([Examples](https://publicwww.com/websites/%22%5C%22%40type%5C%22%3A%5C%22ProfilePage%5C%22%22/))
* [x] ~~[Article](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/README.md#articlejson)~~
  * [ ] [NewsArticle](http://schema.org/NewsArticle) ([Examples](https://publicwww.com/websites/%22%5C%22%40type%5C%22%3A%5C%22NewsArticle%5C%22%22/))
  * [x] ~~[BlogPosting](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/README.md#blogposting)~~
  * [ ] [TechArticle](http://schema.org/TechArticle) ([Examples](https://publicwww.com/websites/%22%5C%22%40type%5C%22%3A%5C%22TechArticle%5C%22%22/))
* [ ] [Report](http://schema.org/Report) ([Examples](https://publicwww.com/websites/%22%5C%22%40type%5C%22%3A%5C%22Report%5C%22%22/))
* [x] ~~[Course](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/README.md#coursejson)~~
  * [ ] [List of Courses](https://developers.google.com/search/docs/data-types/course)
* [x] ~~[Dataset](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/README.md#datasetjson)~~
* [ ] [GeoShape](http://schema.org/GeoShape) ([Examples](https://publicwww.com/websites/%22%5C%22%40type%5C%22%3A%5C%22GeoShape%5C%22%22/))
  * **GeoShape info 1** - <https://webmasters.stackexchange.com/questions/28916/how-do-i-use-the-http-schema-org-geoshape-itemtype>
  * **GeoShape info 2** - <https://developers.google.com/schemas/reference/types/GeoShape>


## Say "Thank you"
If you found this saved you time, or helped you in any way, feel free to buy me a coffee.

[![](https://www.paypalobjects.com/webstatic/en_US/i/btn/png/btn_donate_92x26.png)](https://www.paypal.me/jayholtslander)

![](https://embed-cdn.gettyimages.com/photos/starbucks-coffee-cup-is-seen-inside-a-starbucks-coffee-shop-in-dc-picture-id947784930?k=6&m=947784930&s=594x594&w=0&h=YpPViPiGwIX_XG31_jeYeAxNoOiIIKFFkzAW5imQIik=&Expires=1527210000&Key-Pair-Id=APKAJZZHJ4LGWQENK3OQ&Signature=TRLhtvsllYXJTMQFRRMW9HjR6MVDrmxD0qvPnxm12ymn9poFgq5XVkXsJvGLK5x-XXA7woX5~atqea0LLVnS1X8lLOvoGBlq6Uwa3nBJ0Qgvip9LAN6iBiQc1nN8v1GEBkjC-0Lwg3hFXEvX4gtHrqK1B1ZZUCFC1bl~z-6My2Pz2nIggkVvdp-d~FaA15nk0qAW5jMpJ3g1QjkrE-1lwLI4krCbce0MZyGXOyg96y31BY7ObiUN~DRPLjU6UQa~sVd6UOP9QrMfqbt1ArTUogDOGGHh68Qu2wTS2UpIFgasQbWi-giyqgXaWvlHYrnF1DN96SVl-VOWQUucJ1XKzw__)

## Testing
  ### The code
  * [Structured-Data-Test-Button Wordpress Plugin](https://en-ca.wordpress.org/plugins/structured-data-test-button/)
  * Yoast's admin bar functions
  * The Google [Structured Data Test Tool](https://search.google.com/structured-data/testing-tool).

  ### The results
  * [Rich Results Test](https://search.google.com/test/rich-results)

## See also:

### Tools
* **[SchemaApp Web Tool](https://www.schemaapp.com/tools/jsonld-schema-generator/)**
* **[Schema Tool](https://schema.pythonanywhere.com)** ([About this tool](http://polak.es/en/generator.html))

### Articles
* **REALLY good instructions** - <https://builtvisible.com/micro-data-schema-org-guide-generating-rich-snippets/>
* **[Using Google Tag Manager to dynamically generate Schema.org JSON-LD Tags](https://moz.com/blog/using-google-tag-manager-to-dynamically-generate-schema-org-json-ld-tags)**
* **[5 Common schema problems and what to do about them](https://www.distilled.net/resources/5-common-schema-problems-and-what-to-do-about-them/)**
* **[Implement JSON-LD within the Wordpress Divi theme](http://ahmedkaludi.com/structured-data-divi-theme/)**
* **[Structured Data Actions in email](https://developers.google.com/gmail/markup/reference/go-to-action)**
* **[Yoast's "Ultimate Guide"](https://yoast.com/structured-data-schema-ultimate-guide/)**

### Discussions
* **[Structured data markup for multi-location businesses](https://productforums.google.com/forum/#!topic/webmasters/RNTOPTweJZk)**

### Sources
* **Reference - Local Business** - <http://linter.structured-data.org/examples/schema.org/LocalBusiness/>
* **Reference - Corporate Contacts** - <https://developers.google.com/search/docs/data-types/corporate-contacts>
* **Reference - Contact point** - <http://linter.structured-data.org/examples/schema.org/ContactPoint/>
* **[Homepage Structured Data](http://razorrank.com/structured-data/homepage-structured-data-with-json-ld/)**
* **[Steal our JSON-LD](https://jsonld.com)**
