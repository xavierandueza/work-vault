*what I did:*
- For askAI v2 we didn't disable the hub endpoint when ask. Security adjacent if we can get reviewed quickly cc @anand [PR](https://github.com/readmeio/ai/pull/946) 
- Tool call UI bug where between text chunks tool calls weren't rendering - PR here.
	- @ryan if you don't mind looking at the UI in the [loom](https://www.loom.com/share/fc48c2938ff64be2a7b6362562e61659) (skip past code showing part). Any issues lmk and I'll fixup ASAP
- AskAI - get the backend to return urls in-text
	- [AI side](https://github.com/readmeio/ai/pull/946) is good for review
	- [monorepo side](https://github.com/readmeio/ai/pull/946) also good for review, but needs an sdk bump
- [Medium response length for monorepo](https://github.com/readmeio/readme/pull/20084): 
	- Up for internal review, but still need to complete testing for this
- PR Reviews

*Blockers*
- Need feedback on the [loom](https://www.loom.com/share/fc48c2938ff64be2a7b6362562e61659)  for tool calls from you @ryan - its same as what we currently have just want to make sure you're all good with it.

*Discussion*
- None

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