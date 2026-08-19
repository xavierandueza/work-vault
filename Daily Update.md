***what I did:***
- PR reviews - quite a few longer ones today so took up quite a bit of time
- Continued updates on the AI Onboarding doc - need some more time with this to actually ticket out, likely to have done EOW
- Started on a [security issue](https://linear.app/readme-io/issue/CX-3841/avoid-pii-in-ssr-props-unless-used-in-a-public-way) that was brought up, concern around showing PII that isn't required from akamai
	- This isn't emails its full names, but just as bad

***AskAI v2***
* At risk of this being delayed if we don't get UI/UX approval of this + merge tomorrow. We'll do QA for the unified search internally but if we don't start resolving issues tomorrow then GA will be pushed back again

***Blockers***
- UI/UX approval for Unified Search
- AskAI v2 delayed because of the new search settings needing integration work - Ryan will have time to polish settings but we'll start on the QA stuff ASAP

***Discussion***
- AI Onboarding - I'll explain what my general approach recommendations are
	- Need to make sure there's engineering buy in for a couple key parts:
		- Allowing users to actually signup via public api
		- Allowing users to create projects, do almost everything via public API - if there's a hub endpoint that mutates state we probably want it exposed publicly (styles, askAI settings...)
		- We MIGHT need to have a new access token type with higher admin perms

***What I’ll be working on next:***
- PR up to remove the askAI v2 feature flag
- Ticketing of work for the AI Onboarding
- Otherwise just working on better evals for askAI - has been on to-do for a while but kept having things pop up

***Where this puts me/us:***
* Definitely need unified search merged tomorrow - just UI/UX blocking

***PR Reviews:***
- Didn't record today but around 5-7 probably