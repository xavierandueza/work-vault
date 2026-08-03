*what I did:*
- Looked over the recent AI imports - tagged ryan in the UI/UX ones and Minh in the other technical ones:
	- TLDR: we're not handling links to oas well. 
	- We're not handling non-english titles, excerpts well (ie Chinese body content but english header and excerpt)
	- Some interesting cases coming through, ie pretty sure someone from JPMorganChase uploaded some internal docs
	- **Think we need to allow .zip files and more than 10 docs quickly**
- WIP - the [QA Plan for askAI v2](https://app.notion.com/p/readme/QA-Plan-AskAI-V2-3b1c282774b580a69d62cf1ea163c836)
	- Another couple hours and it'll be good to go
	- Have one case that wasn't considered - askAI suggestion localization
		- @falco made a ticket for you on it [here](https://linear.app/readme-io/issue/RM-17777/make-askai-suggested-questions-respect-locale)
		- Medium prio, if you can fit in by EOW that'd be great
- WIP - better askAI contextualization
	- [PR up here](https://github.com/readmeio/ai/pull/919) - need to get a recording up and do a self-review
	- Also need to run the evals on it yet

*Awaiting Review*

* `ai`
    * [askAI v2 responses too long](https://github.com/readmeio/ai/pull/891) @anand

*Blockers:*
* [@ryan](https://lyra-technologies.slack.com/team/U028C1PJE9X) finishing the testing plan for the askai v2 release tomorrow to send to QA team - I know we have:
    * New askAI placement locations
    * AskAI in search bar
    * All normal chat interface stuff (ie tool call/thinking showing)
    * Is there anything that's part of v2 release that I'm missing?
	- Advanced/custom prompts
	- Links showing up at the bottom
		- Links togglable to show down bottom as before...

*Discussion:*
* Are we cool allowing for more than 10 docs/zip uploads? Seems that some people may have been wanting to upload more but couldn't from what I was looking at.
* Nice on the MCP metrics plan @jarrod - I'll give a read over today and give you any feedback that I have.
	* As a heads up - might be looking to get @Alvin He to take over agent metrics or MCP OAuth so that you're not as stretched across the 3 things - CC @falco
* Do we want to allow for the pages to be searchable as well as llms.txt? ie a /llms/search?query=cat that gets all the actual cat excerpts...
* Happy 5 year work-a-versary Ryan
* For @christian I'll be trying to make it so that you have less PRs to review on AI side so you can revieiw some of the branching teams prs - everyone maybe lessen up on christian so that he can not have the normal AI load and can focus on slack/teams PRs.


*What I’ll be working on next:*
* Tuesday:
	* AskAI testing plan finished
	* AskAI seeding turns finished
    * Get monorepo medium-length answer task for v2 ready for internal review
    * Get the monorepo access pattern work done (Tuesday)

*Where this puts me/us:*
* Still good for GA thursday 13th from my end


*PR Reviews:*
- `readme`
	-  https://github.com/readmeio/readme/pull/20067
	- https://github.com/readmeio/readme/pull/19580
- `ai`
	- https://github.com/readmeio/ai/pull/882 
- `ai-cli-runner`
	- https://github.com/readmeio/ai-cli-runner/pull/103
	-  https://github.com/readmeio/ai-cli-runner/pull/101