***what I did:***
- Fix up for gemini 3.7 flash work
	- Made a PR on top of above - just updating the fallback models for other providers to also use the latest
		- A PR merging into this too, better type checking for our modelIds. Basically we had a bunch of magic strings that are easy to mess up on, no type safety around them either
- Fixed up the `ai-client` issue for the merge into prod - had to just reset the pr and open up a new one
- PR reviews
- Added some more thoughts ot the AI Onboarding doc of ours again - TLDR we can actually get started with this very quickly with the approach of using MCP
	- Homepage copy to paste into agent
	- We continue to improve gradually as we add more API endpoints

***AskAI v2***
* At risk of this being delayed if we don't get UI/UX approval of this + merge tomorrow. We'll do QA for the unified search internally but if we don't start resolving issues tomorrow then GA will be pushed back again

***Blockers***
- UI/UX approval for Unified Search
- AskAI v2 delayed because of the 

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