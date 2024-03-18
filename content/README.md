# George's Compendium of DND Notes

Currently the only entry here is for Hunter's Steinhardt's guide to the eldritch hunt campaign.

#### This is a sub repo that restricts sensitive character info docs via gitignore
So this repo can be the source of published information for things like Session notes, NPCs, Locations, etc.
### Features I'd like to add:
1. (COMPLETED) Ability to blacklist/white list files/directories that display on the blog/website
	1. This can be achieved via git ignore
2. recognition of obsidian hyper links?
	1. 
3. would be ideal if I could just embed obsidian with plugins as the website for the other addons I have like properties and whatnot
	1. I could just leave properties invisible and allow someone to search by the tag property though if I do it custom!
	2. Maybe I can export to HTML for this rather than having to parse it all out myself custom like?

There are 2 routes I can take this from here for further development:

## Custom Markdown Processor Method
Ok, so I did the github thing, now I'd need to make a MARKDOWN PREPROCESSOR to generate the proper formatting for a Gist/HTML generation?
- Could I just do HTML generation and pop that on Vercel?

## HTML Generation Method
I'll try the html generation route and upload to Vercel.
I might be able to make a script or some simple obsidian plugin that automagically uploads that info to Vercel post Parse!

If this works perfectly, it could be the easiest by far.

Else I may have to do a combination of Markdown Processing and HTML generation before deploying with an intelligent router in NEXTjs?

Either way, I'll want to play around with the HTML Export Plugin!
- In this case, I'd be exporting an entire vault? (Sub vault of main vault, I need to re-organize files again I think...)
Oh damn! It even supports a bunch of plugins!

It'd be great if I could use github actions to trigger the HTML Export to run...
- maybe try the method recommended [here](https://linked-blog-starter.vercel.app/home) instead?


### SHIT! 
If I want to do the HTML Export method locally, it'll include Waron's character files, since they aren't git ignored!

If I can trigger this from the repo, rather than on my local machine on a push, then it'll still work though!
- Maybe I can achieve this via github actions?

- [ ] Try hosting the generated files to see if the links work!
	- [ ] Do I need to include these in a NEXTjs project as base HTML files with a static router?
		- [ ] Probably, yes.

## Referenced for creation:
https://youtu.be/6s6DT1yN4dw
