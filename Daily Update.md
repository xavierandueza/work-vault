*what I did:*
- Dealt with the fire for the AI job queue issue
	- Mostly resolving the follow ons, ty to JR and Jason for jumping in and helping resolve.
	- Carried over claude issue for the auto-removal work
		- [PR for this here](https://github.com/readmeio/ai/pull/949) - tested and LGTM
- Got back to Kirby on her Qs re: AI writer
- PR Reviews
- Got a [PR up](https://github.com/readmeio/readme/pull/20256) for the last askAI related security issue that the researcher identified
- QA triage tickets for askAI V2 work (I'll provide a separate status update on this):
	- WIP: Fix up enterprise projects not getting their [custom prompts from parent projects](https://linear.app/readme-io/issue/RM-17831/custom-prompt-ignored-on-enterprise-projects-ask-ai-api)
	- [Project-scoped knowledge issue](https://linear.app/readme-io/issue/RM-17829/ask-ai-does-not-pull-answers-from-child-projects-when-project-scope) - will work on tomorrow

*Blockers*
- PR approvals on some of the high-prio work

*Discussion*
- What do we think about the url stuff from the loom?

*What I’ll be working on next:*
- [Project-scoped knowledge issue](https://linear.app/readme-io/issue/RM-17829/ask-ai-does-not-pull-answers-from-child-projects-when-project-scope)
- finish work on enterprise projects not getting their [custom prompts from parent projects](https://linear.app/readme-io/issue/RM-17831/custom-prompt-ignored-on-enterprise-projects-ask-ai-api) 
- Tool calling UI fixup - use w/e is on next for this UI
- Medium response length for monorepo
- AskAI - get the backend to return urls in-text

*Where this puts me/us:*
* AskAI v2 core will be ready by Thursday for release, but I don't think that the unified search will be.
* Do we want to delay the whole release, or go forward with the better functionality and the placements only and release unified search a week later?

*PR Reviews:*
- `readme`
	- https://github.com/readmeio/readme/pull/20234
	- https://github.com/readmeio/readme/pull/20226 x2
	- https://github.com/readmeio/readme/pull/20251
	- https://github.com/readmeio/readme/pull/20252
- `ai`
	- https://github.com/readmeio/ai/pull/950 x2
- `gitto`
	- 
- `ai-cli-runner`
	- https://github.com/readmeio/ai-cli-runner/pull/108
- `cli`
	- https://github.com/readmeio/cli/pull/39
