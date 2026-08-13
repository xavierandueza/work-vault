## What is the ideal UX for this?
Note - I'm thinking of this like we would do a Github PR. 

- User immediately sets up their style guide:
	- They can have AI help set this up - basically the hub editor can assist them with this setup:
		- If there's the ability to modify any text then we can actually have the hub agent modify this style guide on-demand asw - essentially can modify a context.md as it goes
	- They don't need to actually codify set rules, just dump text and we figure it out from there
	- Its clear that this is a generic thing that AI will use as inputs, not just something for docs audit.
- For a user "warnings", "errors" don't mean anything vs a style guide so just can it.
- The comments that come in have a grade for them - high/med/low but better worded...
	- Inline commented when viewing via UI
	- **It should have the fix for it ready to apply**
- The hub agent can run the linter on pages manually
	- It can also view the linter results that are active for a page alongside the pages information
- Full docs audit mostly unchanged, fix all mostly unchanged:
	- Maybe they can choose from a list of models to do this, but its not a big deal
	- These features are good for a change of a style guide/update on a large doc.
### General
- All tools exposed via our hub agent editor should also be tools that we expose via our MCP too - these can be tools that only paid customers can actually have access to though...?
	- eventually people may use the readme ui less and less for edits, have agents do a lot of the work.
## Implementation considerations
- We want a gradual rollout of improvements
- Best to focus on major issues/wins

### Single Text Instructions
- Move from warnings, errors, style guide to 1 unified input
	- Needs a migration
	- We should change where these settings live - its across ALL AI FEATURES that we use this information
- Page linting needs to check against these sections
- We have a recommended way that people format this
- seeding works for this like it does now, just 1 big textbox instead

### 
