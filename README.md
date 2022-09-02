# stunning-indie-web
Trying out a concept to create a indie web blog engine

 ## initial concept
 I want the blog engine to be indie-web centric. So I want to get things
 like webmentions and a feed to be first class citizens.
 
 The trick is, I also want this to exist in a single static page with no dependencies and I'm taking inspiration from [TiddlyWiki](https://tiddlywiki.com/dev/static/TiddlyWiki.html). In addition I want it easy to post updates, work on my phone, and **Gasp!**
 be readable without JavaScript.

## i spot some trouble
SEO is gonna be an issue. Especially since my first attempt is going to use 
url hashes to do "pages." Now, that could be worked around by using history api
and some JavaScript but since this blog engine is for me and for the small web I'm going 
to put that on the back burner.

If I do go that route, I'll need a host that does wildcard redirects ...
so everything is redirected back to the index.html file.

 - https://docs.netlify.com/routing/redirects/rewrites-proxies/
 - https://www.markhneedham.com/blog/2022/07/27/vercel-redirect-wildcards-nested-paths/
 
 ## to do (eventually, no particular order)
 
 - [ ] Add in some way to search: https://gomakethings.com/how-to-create-a-vanilla-js-search-page-for-a-static-website/
 - [ ] for webmentions: https://web.dev/sandboxed-iframes/#further-reading
 - [ ] Make sure all code has proper attribution/licencing
 - [ ] What about NoJS? Is it worth almost double the file size or should I not save the JSON and make a parser for the HTML?
 - [ ] What about this concept? https://indieweb.org/friending
 - [ ] Have tags input on post look like other tag UI's and have lookup
 - [ ] Password protected portions
 - [ ] Add in unsplash settings area and fix up the parser when changing it to HTML
 - [ ] Add in delete button on posts
 - [ ] Do I need an explicit save button or is navigating away from the page enough
 - [ ] Finish the Github API integration for auto save files
