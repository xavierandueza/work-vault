***what I did:***
- Morning meetings
- PR Reviews
- Retested 
- Got a [fix up for a security issue](https://github.com/readmeio/readme/pull/20365) - if someone has a file key for an editor chat upload that they don't have access to, and guess a file name that exists for something that was uploaded to the AI editor they could gain information (via the LLM) about that file
- Gave some thought on how docs audit might be best to work long-term.
- Retested and merged the [tool call UI bug fix](https://github.com/readmeio/readme/pull/19942) - note merged after release so not live yet.
- Retested and merged the [askAI v2 linking on AI side](https://github.com/readmeio/ai/pull/946) - will trigger an AI release tomorrow to get an sdk bump

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