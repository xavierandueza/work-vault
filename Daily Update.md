***what I did:***
- PR reviews - quite a few longer ones today so took up quite a bit of time
- Continued updates on the AI Onboarding doc - need some more time with this to actually ticket out, likely to have done EOW
- Started on a [security issue](https://linear.app/readme-io/issue/CX-3841/avoid-pii-in-ssr-props-unless-used-in-a-public-way) that was brought up, concern around showing PII that isn't required from akamai
	- This isn't emails its full names, but just as bad
	- Spent some time digging into and verifying what SSR props we're currently exposing that we probably don't want to be
	- Changelogs are WIP, will be able to get other ones up in background tomorrow.

***AskAI v2***
* Delayed to Thursday 27th
* Will get testers onto unified search tomorrow

***Blockers***
- Having issues running the migration test for medium projects locally (connection refused) but I need to look into a bit more, have had higher prio tasks today b/c of the delay

***Discussion***
- None 

***What I’ll be working on next:***
- Security fixups for SSR props
- PR up to remove the askAI v2 feature flag
- Ticketing of work for the AI Onboarding
- Otherwise just working on better evals for askAI - has been on to-do for a while but kept having things pop up

***Where this puts me/us:***
* Okay for Thursday next week for askAI v2

***PR Reviews:***
- `readme`
	- https://github.com/readmeio/readme/pull/20148
	- https://github.com/readmeio/readme/pull/20388
	- https://github.com/readmeio/readme/pull/20411
	- https://github.com/readmeio/readme/pull/20435
	- https://github.com/readmeio/readme/pull/20446
- `ai`
	- https://github.com/readmeio/ai/pull/980
	- https://github.com/readmeio/ai/pull/981
	- https://github.com/readmeio/ai/pull/983
	- https://github.com/readmeio/ai/pull/986