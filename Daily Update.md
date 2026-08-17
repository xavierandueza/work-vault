***what I did:***
- Merged our ai package bumps into `readme` repo ([ai](https://github.com/readmeio/readme/pull/20374)) ([ai-client](https://github.com/readmeio/readme/pull/20375))
- Got a pr up for the Gemini 3.7 flash release, adding to our model list for agent, askAI
- Got a PR up for a fix to the `rdme` repo -> security concern that we had
- got a pr up to fix our downstream dep bump issue - a timing issue thing

***AskAI v2***
* Thursday 20th release b/c of unified search work

***Blockers***
- Greptile is blocking [my pr](https://github.com/readmeio/ai/pull/972) with a 4/5 confidence? What do I do I can't seem to retrigger @anand
- @anand can we do a dry run for the change to the [askAI length change](https://github.com/readmeio/readme/pull/20084) - this will touch a lot of projects so want to see how many with you for prod
- @anand would be good to do a dry run for the medium response length migration just to see blast radius - might be very large if you don't mind chatting before standup on it? In case we want to change strategy

***Discussion***
- AI Onboarding - my thoughts are in the [notion doc](https://app.notion.com/p/readme/AI-Onboarding-3bcc282774b580eea386f801cbc64080?source=copy_link) 
- Christian point - merge conflicts in slack writer, generally using the agent for merge readiness:
	- Had a chat to marcus on this, bit complex we're adding in new tools for this that we enable while in that specific mode.
- Notifications for [ai writer branches](https://readmeio.slack.com/archives/C091D173ANL/p1786931284842619?thread_ts=1786719887.566799&cid=C091D173ANL)  - do we want to get done soon?

***What I’ll be working on next:***
- Finish the golden askAI v2 test suite
- [Medium response length for monorepo](https://github.com/readmeio/readme/pull/20084): 

***Where this puts me/us:***
* Still on track for AskAI v2 next Thursday from my POV

***PR Reviews:***
- `readme`
	- https://github.com/readmeio/readme/pull/20148
	- https://github.com/readmeio/readme/pull/20189
	- https://github.com/readmeio/readme/pull/20342
- `cli`
	- https://github.com/readmeio/cli/pull/41
