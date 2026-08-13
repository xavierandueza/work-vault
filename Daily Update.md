*what I did:*
- Bunch of PR reviews
- Got a [fix up for a security issue](https://github.com/readmeio/readme/pull/20365) - if someone has a file key for an editor chat upload that they don't have access to, and guess a file name that exists for something that was uploaded to the AI editor they could gain information (via the LLM) about that file
- Gave some thought on how docs audit might be best to work long-term.
- Retested and merged the [tool call UI bug fix](https://github.com/readmeio/readme/pull/19942) - note merged after release so not live yet.
- Retested and merged the [askAI v2 linking on AI side](https://github.com/readmeio/ai/pull/946) - will trigger an AI release tomorrow to get an sdk bump

*Blockers*
- 

*Discussion*
- `owlbot.enabled = false` currently does not disable the API - intentional. Dan asked if we could have a "disable on api" asw - akamai might want this but they might also just be a bit spooked atm.
- Docs Audit thoughts

*What I’ll be working on next:*
- Medium response length for monorepo - testing
- Finishing testing for issues that anand got claude to setup - bidi sync related

*Where this puts me/us:*
* Still good for core logic release Thursday, but as discussed we're moving askAI 1 week back b/c of the unified search needing QA

*PR Reviews:*
- `readme`
	- https://github.com/readmeio/readme/pull/20253
	- https://github.com/readmeio/readme/pull/20281
- `ai-cli-runner`
	- https://github.com/readmeio/ai-cli-runner/pull/109