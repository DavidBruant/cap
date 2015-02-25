# cap

An attempt at a capability URL library

# Use case

Need to share a page to someone, but not everything on the page. It should be possible to create a URL that links to a restricted view of the page.
Eventually, it should be possible to do [Rich sharing](http://www.hpl.hp.com/techreports/2009/HPL-2009-169.html) thus achieving [not one click for security](http://www.hpl.hp.com/techreports/2009/HPL-2009-53.html?mtxs=rss-hpl-tr).




# An Express middleware

For now at least.

On receiving a URL, path gives the resource ("template") and the `s` query parameter (`?s=`) gives the data
The middleware reads cap data (akin to session middleware).

For all resources, no `s` query parameter => 403
Add PUBLIC list of path that don't need a cap.


