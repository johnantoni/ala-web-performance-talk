# ala-web-performance-talk
notes on the A List Apart web performance talk

To the client:
Communicating the performance impact of features.

#### Tools

* Web page test / Test every commit.
* Page speed insights
* Network link conditioner
* OSX bandwidth throttling tools
* Performance regression testing
* How do we know our sites fast = speed index (etsy generally aims for 1000, but horses for courses)

#### Points
* Having a performance budget
* Engaging with the client on performance, actually talking about it as a big concern
* Having a performance audits
* Prevent regressions - celebrate performance wins
* Quarterly performance hero - big thing a Etsy
* Examine site, what does the user care about. What's the most important thing for them and focus on making that more performant / immediate -- look at the critical path
* Educating the client why you designed the site that way, to teach optimization, so that your choices will not be lost when a new design comes in. They understand why you did things that way.

#### Tips
* Css inlining. Don't place all the css in the head. Just the parts that stop the flash of unstyled text - can be difficult to employ on large sites already established.

#### Things to look at
* HTTP2 - allows "Server push", 
* Font loading events
* Devising a "Above the fold" technique
* responsive ads
* Design for modularity
* Style guide of optimized content
* Lazy load ads
* Determine blocking events
* Speed perception
* Optimize images
* Font loading - originally as data uris. But the font file will only load when it's needed.
* Use breakpoints!
* At etsy we only use custom fonts on desktop, this can be confusing for designers
* Scalability easier for more restrictive font type setting
* NOTE: IE8, IE9 with compatibility mode on loads all the fonts regardless of if they're needed

#### Responsive images
* Picture element (srcset) http://html5hub.com/html5-picture-element/
* Device conditions
* Picturefill polyfill
