*what I did:*
- PR Reviews
- Got the AskAI projects setup for the QA team to use - refer to those projects for details
- PR Reviews
- Read over the importer stuff from previous day
- Worked on askai dataset/judge improvements:
	- Broke out the dataset into what's stored on disk more - we have the negative cases, the forbidden words cases, and normal cases
	- Forbidden words are good on v1, v2
	- Negatives (ie OOS inputs) on v1 actually doesn't perform as well - v2 performs better, aside for GPT5.6 Terra and Luna that perform equally. Good news since its not a degradation:
		- Made [a ticket for this](https://linear.app/readme-io/issue/RM-17820/askai-v2-handles-bad-queries) - but its not something that we should actually worry about for now since this is better than current and is a long-term improvement
		- Fast-follow is fine but anything more is unneccessary
- Finished the ai seeding task - its simplified from what I was doing before:
	- Addressed anandBot comments - sent anand some info on this
	- @anand anandbot never resolved but I think its overkilling atm - assigned you for review: https://github.com/readmeio/ai/pull/919
	- Evals re-running for v1, v2 at present
	- No reason to think results will be different from what I saw before fixes, but want to be double-sure

*What I’ll be working on next:*
- [URLs embedded in askAI v2 responses](https://linear.app/readme-io/issue/RM-17823/askai-links-in-response)
	- Get the monorepo PR up at least
- Medium response length for monorepo
- AskAI - get the backend to return urls in-text

*Where this puts me/us:*
* Still good for GA thursday 13th from my end, just flagging the delay risk now

*PR Reviews:*
- `readme`
	- [x] https://github.com/readmeio/readme/pull/20176
- `ai`
	- https://github.com/readmeio/ai/pull/883 
- `ai-cli-runner`
	- https://github.com/readmeio/ai-cli-runner/pull/105
- `cli`
	- https://github.com/readmeio/cli/pull/38
