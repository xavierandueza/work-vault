*what I did:*
- Got the [PR up ](https://github.com/readmeio/readme/pull/20269)for the final part of the security issue, merged.
- Tested out an issue with AskAI v2 - was actually resolved by another fix.  [Project-scoped knowledge issue](https://linear.app/readme-io/issue/RM-17829/ask-ai-does-not-pull-answers-from-child-projects-when-project-scope)
- Got a branch up for getting akamai their info on the askAI security issue. Sending instructions separately for this in the fire channel.
	- https://github.com/readmeio/ai/pull/955
- PR up for making sure that owlbot disabling turns off the askAI v2 endpoint too
	- https://github.com/readmeio/readme/pull/20279
	- Need to do more testing and a loom for this
- Tool calling UI fixup - WIP but will be done early tomorrow
- PR Reviews

*Blockers*
- None

*Discussion*
- What do we think about the url stuff from this [loom](https://www.loom.com/share/085e289a669b4ae69287d9e0250c439c)? @ryan
	- We can chat about in standup tomorrow/chat after call
- how do we want to handle the likely delay for the Unified search?

*What I’ll be working on next:*
- Tool calling UI fixup
- any feedback from url stuff
- Medium response length for monorepo
- AskAI - get the backend to return urls in-text

*Where this puts me/us:*
* as before - AskAI v2 core will be ready by Thursday for release, but I don't think that the unified search will be.

*PR Reviews:*
- `readme`
	- https://github.com/readmeio/readme/pull/20148
	- https://github.com/readmeio/readme/pull/20209
	- https://github.com/readmeio/readme/pull/20220
	- https://github.com/readmeio/readme/pull/20228
- `ai`
	- https://github.com/readmeio/ai/pull/936
	- https://github.com/readmeio/ai/pull/941
	- https://github.com/readmeio/ai/pull/954
	- https://github.com/readmeio/ai/pull/956
