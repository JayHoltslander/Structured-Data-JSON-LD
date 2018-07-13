# Structured Data - JSON-LD

[![Join the chat at https://gitter.im/Jays-Structured-Data/Lobby](https://img.shields.io/gitter/room/nwjs/nw.js.svg)](https://gitter.im/Jays-Structured-Data/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) ![](https://img.shields.io/chrome-web-store/stars/nimelepbpejjlbmoobocpfnjhihnpked.svg) [![](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](http://www.twitter.com/share?text=Great+collection+of+structured+data+snippets+in+JSON-LD+format+by+@j_holtslander&url=https://github.com/JayHoltslander/Structured-Data-JSON-LD)

Structured Data is hard when you're starting out. Conflicting info. Old outdated information. Poor documentation. I've spent a significant amout of time trying to master it. Now you can benefit from all my hard work and testing. Everything here works properly or it wouldn't be here. Many of these will provide the [fancy Google Search Enhancements](https://developers.google.com/search/docs/guides/search-gallery) you desire and ensure your content types are marked up properly.

|**News**|
|:--|
|Google's Structured Data Testing Tool has stopped seeing Structured Data thats been inserted via Google Tag Manager. This caused a minor little uproar on Twitter when Google's John Mueller tweeted a response of "[I wouldn't rely on a tool like GTM to add Structured Data](https://twitter.com/thisisdelbert/status/1017098840422244352)". Some blogs immediately ~twisted this into~ wrote that Google itself has now declared that GTM should not be used for inserting Structured Data. Which [is ridiculous](https://twitter.com/MattLacuesta/status/1017121141687664640). A new way to insert Structured Data via Google Tag Manager has been found by [Simo Ahava](https://www.simoahava.com/analytics/add-html-elements-page-programmatically/) and this method allows for the testing tool to detect the Structured Data 100% fine.<br><img src="https://media.giphy.com/media/joV1k1sNOT5xC/giphy.gif" width="100%">|


## Installation
<details>
<summary><strong>A.) Hand code it in</strong> (Learn more)</summary>
<p></p>
<p>(Ugh)</p>
<p></p>
 <hr>
</details>


<details>
<summary><strong>B.) Use Google Tag Manager</strong> (Learn more)</summary>
<p></p>
 <p>Use <a href="https://www.google.com/analytics/tag-manager/">Google Tag Manager</a> to insert the code with the "Custom HTML" tag. (See screenshot below.) Why Tag Manager? Because Tag Manager can dynamically change the Structured Data based on the content of the page! (eg: Blog posts) See <a href="https://presencemedia.io/schema-markup-structured-data-2018-guide/#dynamicallyaddschema">this article</a> and <a href="https://moz.com/blog/using-google-tag-manager-to-dynamically-generate-schema-org-json-ld-tags">this older Moz article</a> for more information on how to do that.</p>
 
 <p><strong>UPDATE:</strong> Google changed something. Now, in order to have the Structured Data Testing tool detect inserted Structured Data properly, it must be inserted programatically. Pasting your desired Structured Data within this snippet below will allow it to be detected properly by the testing tool.</p>
 
 <pre class="rich-diff-level-zero"><span class="pl-c rich-diff-level-one"><span class="pl-c">&lt;!--</span> GOOGLE TAG MANAGER VERSION <span class="pl-c">--&gt;</span></span>
<span class="pl-c rich-diff-level-one"><span class="pl-c">&lt;!--</span> Credit: https://twitter.com/SimoAhava/status/1001397355403468802 <span class="pl-c">--&gt;</span></span>
<span class="pl-c rich-diff-level-one"><span class="pl-c">&lt;!--</span> Source: https://github.com/JayHoltslander/Structured-Data-JSON-LD <span class="pl-c">--&gt;</span></span>
&lt;<span class="pl-ent rich-diff-level-one">script</span>&gt;<span class="pl-s1 rich-diff-level-one"></span>
<span class="pl-s1 rich-diff-level-one">(<span class="pl-k">function</span>() {</span>
<span class="pl-s1 rich-diff-level-one">   <span class="pl-k">var</span> jsonData <span class="pl-k">=</span></span>
<span class="pl-s1 rich-diff-level-one"></span>
<span class="pl-s1 rich-diff-level-one"><span class="pl-c"><span class="pl-c">//</span> PASTE THE JSON THAT YOU WANT TO USE, HERE.</span></span>
<span class="pl-s1 rich-diff-level-one"><span class="pl-c"><span class="pl-c">//</span> Only paste what's within the &lt;script&gt; block.</span></span>
<span class="pl-s1 rich-diff-level-one"><span class="pl-c"><span class="pl-c">//</span> Your pasted content should start with a "{" and end with a "}"</span></span>
<span class="pl-s1 rich-diff-level-one"></span>
<span class="pl-s1 rich-diff-level-one">; <span class="pl-k">var</span> el <span class="pl-k">=</span> <span class="pl-c1">document</span>.<span class="pl-c1">createElement</span>(<span class="pl-s"><span class="pl-pds">'</span>script<span class="pl-pds">'</span></span>);</span>
<span class="pl-s1 rich-diff-level-one"><span class="pl-smi">el</span>.<span class="pl-c1">type</span> <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">'</span>application/ld+json<span class="pl-pds">'</span></span>;</span>
<span class="pl-s1 rich-diff-level-one"><span class="pl-smi">el</span>.<span class="pl-smi">innerHTML</span> <span class="pl-k">=</span> <span class="pl-c1">JSON</span>.<span class="pl-c1">stringify</span>(jsonData);</span>
<span class="pl-s1 rich-diff-level-one"><span class="pl-c1">document</span>.<span class="pl-smi">head</span>.<span class="pl-c1">appendChild</span>(el);</span>
<span class="pl-s1 rich-diff-level-one">})();</span>
<span class="pl-s1 rich-diff-level-one"></span><span class="pl-s1 rich-diff-level-one">&lt;</span>/<span class="pl-ent rich-diff-level-one">script</span>&gt;</pre>
 
 <p><strong>See also:</strong></p>
 <ul>
  <li><a href="https://www.google.com/search?rls=en&q=how+to+install+Google+Tag+Manager&ie=UTF-8&oe=UTF-8">How to install Google Tag Manager</a></li>
  <li><a href="https://searchengineland.com/add-schema-markup-site-using-google-tag-manager-272516">Add schema markup site using Google Tag Manager</a></li>
  <li><a href="https://yoast.com/structured-data-google-tag-manager/">Adding JSON-LD structured data with Google Tag Manager</a></li>
 </ul>
 <p></p>
<table>
<tr>
<td><a href="https://camo.githubusercontent.com/460eaed67b255eb426c885e32f8a17bfa180c70c/687474703a2f2f692e696d6775722e636f6d2f71564252326b422e6a7067"><img src="https://camo.githubusercontent.com/460eaed67b255eb426c885e32f8a17bfa180c70c/687474703a2f2f692e696d6775722e636f6d2f71564252326b422e6a7067" width="240"></a></td>
</tr>
<tr>
<td>🔍 <strong>Screenshot</strong></td>
</tr>
</table>
 <p></p>
 <hr>
</details>


<details>
<summary><strong>C.) Use a Wordpress plugin</strong> (Learn more)</summary>
<p></p>
<ul><li>https://wpschema.com/schema-types/</li></ul>
<p></p>
 <hr>
</details>

## Contents

### [AggregateRating.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/AggregateRating.json)
An average rating based on multiple ratings or reviews utilizing the [AggregateRating schema](http://schema.org/AggregateRating). Be sure to read [this article](https://whitespark.ca/blog/how-to-use-aggregate-review-schema-to-get-stars-in-the-serps/) to see why using this example as written might not be the best idea. Hmm. 🤔 Also note that using a 3rd party's ratings (like say Google or Yelp) for a [localBusiness](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/LocalBusiness.json) seems to go against [Google's guidelines](https://developers.google.com/search/docs/data-types/review#review-snippet-guidelines). BUT, also see [this note](https://www.schemaapp.com/how-to/get-rating-rich-results-for-local-business-with-third-party-reviews/) on using 3rd party reviews.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/AggregateRating.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FAggregateRating.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22AggregateRating%5C%22%22/)
<br><br>

### [Article.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/Article.json)
If you’re a publisher website, the more specific schema types like [NewsArticle](https://schema.org/NewsArticle) or [BlogPosting](https://schema.org/BlogPosting) are recommended (choose one or the other, depending on your site/content). Leveraging these markups accordingly can help your content to appear in Google News and in-depth articles search suggestions. See: [Enabling Rich Snippets for Articles](https://developers.google.com/structured-data/rich-snippets/articles). **Note:** To show up in Google's News Carousel not only will the page require Structured Data but it's also [required to be a valid AMP page](https://developers.google.com/search/docs/data-types/article). If you are using the [official AMP Plugin for Wordpress](https://en-ca.wordpress.org/plugins/amp/) you will definitely want to use Tag Manager to insert your Structured Data as opposed to other methods since you will be able to [dynamically generate Schema.org JSON-LD Tags](https://moz.com/blog/using-google-tag-manager-to-dynamically-generate-schema-org-json-ld-tags) from pages that contain the correct pattern for your posts. **eg:** ``?amp=1`` or ``/amp``
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/Article.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FArticle.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22Article%5C%22%22/)
<br><br>


### [BlogPosting](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/BlogPosting.json)
An even more specific version of Article for a blog post. See the [BlogPosting schema](http://schema.org/BlogPosting) for more info.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FBlogPosting.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22BlogPosting%5C%22%22/)
<br><br>


### [BreadcrumbList.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/BreadcrumbList.json)
The [BreadcrumbList schema](https://schema.org/BreadcrumbList) allows you to mark up the breadcrumbs on your site to generate breadcrumb rich snippets for your pages in the SERPs. [Learn more](https://developers.google.com/search/docs/data-types/breadcrumb).
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/BreadcrumbList.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22BreadcrumbList%5C%22%22/)
<br><br>


### [Course.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/Course.json)
The [Course schema](https://schema.org/Course) allows you to mark up courses on your site to generate rich snippets for your courses in the SERPs. [Learn more](https://developers.google.com/search/docs/data-types/course).
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FCourse.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22Course%5C%22%22/)
<br><br>


### [Dataset.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/Dataset.json)
The [Dataset schema](https://schema.org/Dataset) is for a body of structured information describing some topic(s) of interest. It should use the sameAs property to link to the canonical page.  [Learn more](https://developers.google.com/search/docs/data-types/dataset).
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FDataset.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22Dataset%5C%22%22/)
<br><br>


### [ImageObject.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/ImageObject.json)
An example of the [ImageObject](http://schema.org/ImageObject) schema. Demonstrates use of the [exifData](http://schema.org/exifData) schema.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FImageObject.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22ImageObject%5C%22%22/)
<br><br>


### [ItemList-1.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/ItemList-1.json)
The [ItemList](http://schema.org/ItemList) schema makes a page's items eligible for the [Carousel Feature](https://developers.google.com/search/docs/guides/mark-up-listings) on mobile devices ([Screenshot](https://developers.google.com/search/docs/guides/images/search-features03-HostCarousel.png)). This example is for a summary page which has a short description of each item in the list, and each item points to a separate details page that is focused entirely on one item. The details page is where the more detailed Structured Data on the item would be located. See: Docs https://developers.google.com/search/docs/guides/mark-up-listings#summary-page--multiple-full-details-pages
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/ItemList-1.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22ItemList%5C%22%22/)
<br><br>


### [ItemList-2.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/ItemList-2.json)
The [ItemList](http://schema.org/ItemList) schema makes a page's items eligible for the [Carousel Feature](https://developers.google.com/search/docs/guides/mark-up-listings) on mobile devices ([Screenshot](https://developers.google.com/search/docs/guides/images/search-features03-HostCarousel.png)). This example is for a single, all-in-one-page list hosts all list information, including full text of each item: for example, a gallery of recipes for various kinds of muffins, all contained on one page.
See: Docs https://developers.google.com/search/docs/guides/mark-up-listings#single-all-in-one-page-list
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/ItemList-2.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22ItemList%5C%22%22/)
<br><br>


### [ItemList-3.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/ItemList-3.json)
The [ItemList](http://schema.org/ItemList) schema makes a page's items eligible for the [Carousel Feature](https://developers.google.com/search/docs/guides/mark-up-listings) on mobile devices ([Screenshot](https://developers.google.com/search/docs/guides/images/search-features03-HostCarousel.png)). This example shows usage with the [CollectionPage](http://schema.org/CollectionPage) schema. 
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/ItemList-3.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22ItemList%5C%22%22/)
<br><br>


### [JobPosting.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/JobPosting.json)
Adding structured data makes your job postings eligible to appear in a special user experience in Google Search results leading to increased chances of discovery and conversion. Your postings are eligible to be displayed more prominently in the dedicated Job Search UI, featuring your logo, reviews, ratings, and job details. The new user experience enables job seekers to filter by various criteria like location or job title, meaning you’re more likely to attract applicants who are looking exactly for that job. [Learn more](https://developers.google.com/search/docs/data-types/job-posting).
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool/u/0/?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/JobPosting.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FJobPosting.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22JobPosting%5C%22%22/)
<br><br>


### [LocalBusiness.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/LocalBusiness.json)
An example of a LocalBusiness with multiple locations defined. Each location having it's own defined service areas.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FLocalBusiness.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22LocalBusiness%5C%22%22/)
<br><br>


### [LocalBusiness-2.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/LocalBusiness-2.json)
An example of a LocalBusiness customized for a law firm. Demonstrates combined @types (LocalBusiness/Organization/LegalService) and [Corporate Contact](https://developers.google.com/search/docs/data-types/corporate-contact) useage.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FLocalBusiness-2.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22LocalBusiness%5C%22%22/)
<br><br>


### [LocalBusiness-3.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/LocalBusiness-3.json)
A detailed example of a complex LocalBusiness customized for a Notary. Demonstrates combined @types (LocalBusiness/Organization/Notary) and [Corporate Contact](https://developers.google.com/search/docs/data-types/corporate-contact) useage.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FLocalBusiness-3.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22LocalBusiness%5C%22%22/)
<br><br>


### [LocalBusiness-4.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/LocalBusiness-4.json)
An example of a LocalBusiness customized for an online store with no physical location. Demonstrates combined @types (LocalBusiness/Organization/Store)
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FLocalBusiness-4.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22LocalBusiness%5C%22%22/)
<br><br>


### [Person.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/Person.json)
My personal structured data snippet for "Person" in JSON-LD format.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/Person.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FPerson.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22Person%5C%22%22/)
<br><br>


### [Question-w-Answers.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/Question-w-Answers.json)
An example of some markup that results in Rich Snippets for Questions as observed in the wild being used on [Stack Exchange websites](https://stackexchange.com/sites). [SERP Screenshot](http://cdn.skunkworks.ca.s3.amazonaws.com/temp-screenshots/Screen_Shot_2017-12-07_at_11.44.40_AM.png) This example includes additional Schema types for "Answer" and "QAPage" which do not seem to be required but complement each other.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FQuestion-w-Answers.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22QAPage%5C%22%22/)
<br><br>


### [Service.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/Service.json)
A collection of services that a LocalBusiness may provide with per/service ratings.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/Service.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FService.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22Service%5C%22%22/)
<br><br>


### [ServiceArea](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/ServiceArea.json)
How to define a service area for a local business.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FServiceArea.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22ServiceArea%5C%22%22/)
<br><br>


### [SiteNavigationElement.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/SiteNavigationElement.json)
The [SiteNavigationElement schema](http://schema.org/SiteNavigationElement) can help increase search engines’ understanding of your site structure and navigation and can be used to influence organic sitelinks. (See also WPHeader on this page for an example of usage within a Navbar!)
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/SiteNavigationElement.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FSiteNavigationElement.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22SiteNavigationElement%5C%22%22/)
<br><br>


### [SpeakableSpecification](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/SpeakableSpecification.json)
For Voice search a SpeakableSpecification indicates via css selector(s) sections of a document that are highlighted as particularly speakable. See [this article](https://translate.google.com/translate?hl=en&sl=auto&tl=en&u=https%3A%2F%2Fwww.effektiv.com%2Fready-for-voice-search-strukturierte-daten-nach-schema-org-verfuegbar-4464.html) for more info.
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FSpeakableSpecification.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22SpeakableSpecification%5C%22%22/)
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
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22Website%5C%22%22/)
<br><br>


### [WPHeader.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/WPHeader.json)
("Webpage Header" not "Wordpress Header") Define structured Data for items within a site's header with the [WPHeader schema](http://schema.org/WPHeader). Includes SiteNavigationElements within! Also see an example of this in use within the snippet [WebSite.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/WebSite.json)
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FWPHeader.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22WPHeader%5C%22%22/)
<br><br>


### [VideoObject.json](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/VideoObject.json)
A site with embedded or hosted video content can leverage the VideoObject schema. Google primarily displays video rich snippets for YouTube videos, but this will help video rich snippets to appear for your Web pages in Google Video Search. Google Resource Page: [Enabling Rich Snippets for Videos](https://developers.google.com/structured-data/rich-snippets/videos)
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/VideoObject.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FVideoObject.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22VideoObject%5C%22%22/)
<br><br>


### [ViewAction](https://github.com/JayHoltslander/Structured-Data-JSON-LD/blob/master/ViewAction.json)
Indicates where something should be viewed. One of the most common implementations is in Google App indexing, where it enables a URL from a website indexed in search results, to be opened inside the corresponding App (if installed in the user's device).
<br><br>
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button.png)](https://search.google.com/structured-data/testing-tool?url=https://raw.githubusercontent.com/JayHoltslander/Structured-Data-JSON-LD/master/ViewAction.json#url=https%3A%2F%2Fraw.githubusercontent.com%2FJayHoltslander%2FStructured-Data-JSON-LD%2Fmaster%2FViewAction.json)
[![](https://github.com/JayHoltslander/Structured-Data-JSON-LD/raw/master/button-2.png)](https://publicwww.com/websites/%22%40type%5C%22%3A%5C%22ViewAction%5C%22%22/)
<br><br>

---

## Tips & Tricks
You can link snippets together and reuse them ([DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)) by defining and referencing their ``@id`` (These are called "Node identifiers") Learn more about them [here](https://webmasters.stackexchange.com/a/98578/77742).

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
* **Schema Markup Structured Data 2018 Guide** - <https://presencemedia.io/schema-markup-structured-data-2018-guide/>
* **Good instructions** - <https://builtvisible.com/micro-data-schema-org-guide-generating-rich-snippets/>
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
