***what I did:***
- bunch of PR reviews again
- Updated QA plan for askAI v2 + commed with testing team about the unified search being only thing to test
- Merged in the [changelog pii leak work](https://github.com/readmeio/readme/pull/20487)
- Had a chat with ryan and agreed on the best UI for the superscript linking style:
	- Just [the reference is mostly good to go](https://github.com/readmeio/readme/pull/20500) - my agents are still looping on this with anand review though so unfortunately not yet out of internal review
		- Fied up a css styling I saw with askAI links in this too that'll be good to have go live
	- New [PR up for having the links show at bottom](https://github.com/readmeio/readme/pull/20523) and be controlled by the reference
		- Agents still looping on this... As an FYI @anand there's been a LOT of back and forth from this and the above PR. Haven't had the time to audit to see validity of them all yet, but its starting to feel pretty cumbersome and that they keep going for hours on things that are mostly nits
		- Will be ready for design review when you get back @ryan
- Merge [jon's pr](https://github.com/readmeio/readme/pull/20504) once merge freeze lifted
- Fix up the css styling issue for askAI v2
- PII stuff:
	- [changelogs](https://github.com/readmeio/readme/pull/20487) - Merged
	- Unfortunately with PR reviews and other AI pod work I didn't get the time to finish any of these others, I'll make top prio Monday

***AskAI v2***
* On track for Thursday 4th September
* QA testers now on unified search

***Blockers***
- Having issues running the migration test for medium projects locally (connection refused) but I need to look into a bit more, have had higher prio tasks last couple of days:
	- Likely to get to Monday AEST

***Discussion***
- Will need to get feedback when you're back next week @ryan on the UI for the links at the bottom of askAI

***What I’ll be working on next:***
- Security fixups for SSR props - finishing off last 3
- Finishing off the askAI links stuff
- Ticketing of work for the AI Onboarding (Monday)
- PR up to remove the askAI v2 feature flag (Tuesday)

***Where this puts me/us:***
* Ahead for askAI revised timeline
* AI Onboarding doc will be mostly wrapped up + planned by EOD Monday, so by your Monday there'll be a plan for it

***PR Reviews:***
Didn't get to today, so I'll jump back on them ASAP tomorrow morning
- 