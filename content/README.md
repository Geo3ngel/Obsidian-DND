# George's Compendium of DND Notes

Currently the only entry here is for Hunter's Steinhardt's guide to the eldritch hunt campaign.

# CURRENT NOTES MODIFICATION TODO:
I want to enforce the following rough note guide:
## Quest Board
- Who's got what going on for their backstory
	- What do we need to do/where do we need to go
- Main vs side quests?
- Most for tracking things we can/need to do, so we don't forget something
- [ ] Write out current primary objectives
- [ ] Also include secondary (not very important objectives)
- [ ] And then have character specific objectives
	- [ ] Stuff to forward a player's character arc!
## PC Notes
- [ ] Character descriptions, notes, etc.
- [ ] What relationships need to be resolved/interact and why
- [ ] Who needs to talk to who/about what
	- [ ] Maybe also include a "Goals"/"Believes or values" Section?
		- The idea being to help players justify aligning with one another for decisions and the like in character better.
## NPC Org Chart/affiliations
## Shop Notes
- [ ] Shop keep(s)
- [ ] specialization
- [ ] Inventory/pricing
- [ ] benefits
- [ ] relation with part/party notes
## Armory
- Page for each item, as well as a link back to where it can be purchased/found for quick referencing for shopping
	- [ ] Go through and back link to shops that have items available for purchase?
## Lore
- For more generic info dumps, like information we know about Eldritch moons, wars, etc.
- [ ] Fill with details from Alessa's notes!
## Session notes:
- [x] Organized by Character Level
- [ ] Should include a link to the respective session's YT video if published.
	- [ ] Some need to be updated
- [ ] Contains notes from that session.
	- Fill out what I can from Alessa's notes!
---
#### This is a sub repo that restricts sensitive character info docs via gitignore
So this repo can be the source of published information for things like Session notes, NPCs, Locations, etc.
### Features I'd like to add:
1. (COMPLETED) Ability to blacklist/white list files/directories that display on the blog/website
	1. This can be achieved via git ignore
	2. Or via Quartz4's `frontmatter`, `ExplicitPublish`, `RemoveDrafts`, `PrivatePages`, `IgnorePatterns`, etc.
		1. I should probably use `IgnorePatterns` and include paths of stuff we don't want to publish!
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
