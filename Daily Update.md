***what I did:***
- Morning meetings
- PR Reviews
- Fixed up new test cases for the unified search, let the QA team know about them
- Internal 1:1s
- [Retested + Merged ](https://github.com/readmeio/readme/pull/20365)the security related issue for the chat attachments that were exposed cross-project
- Started on a better, golden askAI v2 test case suite based on ReadMe docs:
	- Will have 10x easy, medium, hard questions
	- New judges, validating that the correct links are presented in results
- Started looking into and bumping scoping for ai related ticket that branching pod is tackling - on merging conflicts.
- Team 1:1s

***AskAI v2***
* Thursday 20th release b/c of unified search work
- Links coming from backend after ai release tomorrow, meaning all v2 core features done
- Unified search - need an update on this in standup tomorrow

***Blockers***
- None

***Discussion***
- `owlbot.enabled = false` currently does not disable the API - intentional. Dan asked if we could have a "disable on api" asw - akamai might want this but they might also just be a bit spooked atm.
	- Dan - unless they specifically complain about it.
- Where are we at w.r.t. unified search, sounds like there's some more changes coming down the wire? Maybe a ryan question
- What's the status for the mcp metrics stuff -
- Docs Audit thoughts

***What I’ll be working on next:***
- Review OAS translations pr, give thoughts on that
- Carry over the [fix up for a security issue](https://github.com/readmeio/readme/pull/20365) 
- Trigger AI release
	- Then merge, then check on the linking fix for in-text stream
- [Medium response length for monorepo](https://github.com/readmeio/readme/pull/20084): 

***Where this puts me/us:***
* Still on track for AskAI v2 next Thursday from my POV

***PR Reviews:***
- `readme`
	- https://github.com/readmeio/readme/pull/20350
	- https://github.com/readmeio/readme/pull/20284
	- https://github.com/readmeio/readme/pull/20325
	- https://github.com/readmeio/readme/pull/20342
	- https://github.com/readmeio/readme/pull/19598
- `ai`
	- https://github.com/readmeio/ai/pull/964
	- https://github.com/readmeio/ai/pull/958
	- https://github.com/readmeio/ai/pull/966
	- https://github.com/readmeio/ai/pull/962