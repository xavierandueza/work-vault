*what I did:*
- Dealt with the fire for the AI job queue issue
	- Mostly resolving the follow ons, ty to JR and Jason for jumping in and helping resolve.
	- Carried over claude issue for the auto-removal work
		- [PR for this here](https://github.com/readmeio/ai/pull/949) - tested and LGTM
- Got back to Kirby on her Qs re: AI writer
- [ ] PR Reviews
- [x] Test out the fix and make sure the jobs have a ttl on them after completing.
- [x] Review Falco PR: https://github.com/readmeio/readme/pull/20236
- [ ] Got a PR up for the last askAI related security issue that the researcher identified. It's
- [ ] Investigated the triage tickets for askAI V2 and get some help from others for any that I need to fix up
	- [ ] WIP: Fix up enterprise projects not getting their [custom prompts from parent projects](https://linear.app/readme-io/issue/RM-17831/custom-prompt-ignored-on-enterprise-projects-ask-ai-api)
	- [ ] [Project-scoped knowledge issue](https://linear.app/readme-io/issue/RM-17829/ask-ai-does-not-pull-answers-from-child-projects-when-project-scope) - will work on tomorrow
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
- Tool calling UI fixup - use w/e is on next for this UI
- Medium response length for monorepo
- AskAI - get the backend to return urls in-text

*Where this puts me/us:*
* Delay risk from unified search

*PR Reviews:*
- `ai-cli-runner`
	- https://github.com/readmeio/ai-cli-runner/pull/105
	- https://github.com/readmeio/ai-cli-runner/pull/106
- `cli`
	- https://github.com/readmeio/cli/pull/38
