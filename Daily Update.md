*what I did:*
- PR Reviews
- Read over the importer stuff from previous day
- Got evals results onto the ticket - v1 before/after for parity.
	- Added to the [PR](https://github.com/readmeio/ai/pull/919)
	- See [google sheet](https://github.com/readmeio/ai/pull/919) for reference, TLDR cost and time now only ~35% more for v2 vs v1, before was ~75% more
	- Will be merged + released monday b/c of the merge freeze
- [URLs embedded in askAI v2 responses](https://linear.app/readme-io/issue/RM-17823/askai-links-in-response)
	- Got the PR up for monorepo and AI repo
	- @ryan would be good to get your POV on how we do the links - its intentionally really soft about how we link atm, any thoughts on what works best from the [loom](https://www.loom.com/share/085e289a669b4ae69287d9e0250c439c)?
		- Can't have a testing branch b/c needs ai deployment.
	- Saw a small bug that I'll resolve early next week and move out for review

*Blockers*
- None - just need to know status on unified search 

*Discussion*
- What do we think about the url stuff from the loom?

*What I’ll be working on next:*
- [URLs embedded in askAI v2 responses](https://linear.app/readme-io/issue/RM-17823/askai-links-in-response)
	- Get the monorepo PR up at least
- Medium response length for monorepo
- AskAI - get the backend to return urls in-text

*Where this puts me/us:*
* Delay risk from unified search

*PR Reviews:*
- `readme`
	- [x] https://github.com/readmeio/readme/pull/20176
- `ai`
	- https://github.com/readmeio/ai/pull/883 
- `ai-cli-runner`
	- https://github.com/readmeio/ai-cli-runner/pull/105
- `cli`
	- https://github.com/readmeio/cli/pull/38
