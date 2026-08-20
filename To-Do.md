## Start of Day
- [x] Check Calendar
- [x] Check status of AI apps ([link](https://dashboard.render.com/project/prj-d003snngi27c73ath6j0))
- [x] Check Slack messages and threads
    - [x] Create tasks for anything that needs doing
- [x] Email Check
- [x] Review everyone else’s updates for the day
    - [x] AI Pod
    - [ ] Branching Pod
    - [ ] Enterprise bug bash pod
    - [ ] Onboarding pod
    - [ ] OAS (Hugo)
- [ ] Review Linear notifications
- [ ] Check triage tickets linear
- [ ] Make sure deployments worked fine for my changes
- [ ] LinkedIn check
- [ ] Make sure my tickets for the next few days are well scoped and understood
- [ ] Check weekday-based tasks
- [ ] PR Reviews
- [ ] Check on my outstanding PRs

## End of Day
- [ ] AI Repo CICD
- [ ] Test merged AI CLI Runner stuff
- [ ] Review PRs again
- [ ] Deployments - approve all of the stuff I'm merging in
- [ ] Look at deployments, for anything from me/AI test out and make sure ķts good to go

## What I want to get done this week
### Monday
- [ ] 

### Tuesday
- [x] Merge the ai client: https://github.com/readmeio/readme/pull/20437 
### Wednesday
- [x] review PR here: https://github.com/readmeio/ai/pull/982
- [ ] Unified search for askAI v2 - need to make sure this gets over the line
	- [ ] Make sure its merged
- [ ] Medium Length migration - run this on staging when the staging mongo is live again
- [ ] Get the PR up to remove the feature flag for askAI v2 -> meaning everything should now just default to using askAI v2 stuff.
	- [ ] Merge into the migration PR
- [ ] Take a look over the v1 prompt vs the v2 prompt - what's the difference b/w the two?
	- [ ] Do some testing on the different settings that we currently have b/w the two
- [ ] Do my 1:1 notes

### Thursday
- [ ] Worked on changing askAI v2 links to now be superscript links - looks a lot better:
	- [ ] [Draft PR up](https://github.com/readmeio/readme/pull/20500) - agents need to settle first
	- [ ] Also want to get UI sorted before anyone reviews Get the work done for the links being superscript:
	- [ ] Need to adjust the AI prompt for how we embed links slightly for this but UI is ready to get approved
- [ ] Got the PII for changelogs work ready for review - WIP on the rest just need to self-review the code and test to ensure that it's resolved issues, no issues introduced.
	- [ ] [changelogs](https://github.com/readmeio/readme/pull/20487) g2g, other prs in draft
	- [ ] discuss:
		- [ ] self-review PR
		- [ ] test
		- [ ] loom
	- [ ] Owner info:
		- [ ] self-review PR
		- [ ] test
		- [ ] loom
	- [ ] Git info:
		- [ ] Find the ticket that exists for this
		- [ ] self-review PR
		- [ ] test
		- [ ] loom
- [ ] [Medium response length for monorepo](https://github.com/readmeio/readme/pull/20084): 
	- [ ] Up for internal review, but still need to complete testing for this
	- [ ] Testing:
		- [ ] Project on legacy business doesn't change (thats askAI full)
		- [ ] Project on askAI lite does change
		- [ ] Project on askAI full doesn't change
		- [ ] that when the setting is undefined on a project in UI it is medium
		- [ ] that when the setting is undefined, we use medium from AI side of things too (show the langfuse traces)
- [ ] Give feedback on this: https://linear.app/readme-io/issue/RM-18009/refactor-translation-pipeline-to-use-mongo-ledger
- [ ] Get the PR up to deprecate/remove the askAI v1 logic from the monorepo, AI repos
	- [ ] This will migrate in after we've verified that everything is looking good

### Friday
- [ ] Evals improvements for askAI v2
	- [ ] Better judge(s) - main judge for the valid dataset.
	- [ ] get a better dataset of questions:
	- [ ] 10x easy
	- [ ] 10 medium - usually coordinating a couple of different data points
	- [ ] 10x hard - coordinating a lot of different data points

## PR Reviews
- [ ] `readme`
- [ ] `ai`
- [ ] `gitto`
- [ ] `ai-cli-runner`
- [ ] `cli`

## Backlog
- [ ] Tooling via lsps like anand mentioned → see what we can add for this...
- [ ] Ask everyone who's tackling a vertical - dig up the tickets that other teams can work on - probab
    - [ ] So we know when people can jump in and help.
- [ ] Send through some feedback that I've been hearing from different members of the README team to everybody and ask for the solid asks that I have from them. Which one of them is where this puts us, and the other one is what I'll be working on next, where it should be at least a few days' worth of work
    - [ ] Major highlight here is that they did raise a couple of problems about people not having the next bit of work scoped out, and that they would actually prioritize helping you and scoping it out for you. But of course, when time zones conflict, then that's actually the problem
    - [ ] Where this puts us, next tasks
- [ ] Langfuse improve dataset
- [ ] Think long-term about the role:
    - [ ] Where do they want me involved and doing things?
    - [ ] This should be me being across the pods
    - [ ] Across the individual work people are on to some extent...
        - [ ] Need to use managers for this
    - [ ] Maybe I can handle the evals stuff for IC work...
        - [ ] But aside from that, my work is making sure readme is happy with our output, that the relationships are managed and working well
    - [ ] To that end:
        - [ ] I should get evals to a good point in next few days
        - [ ] Organize for me to be added to all of the syncs
            - [ ] Fly on the wall for the first 1 at least, just understand how the pod works
            - [ ] So I can ask how they do things, what tools they use/don't use...
    - [ ] Probably want to become a Notion power-user, so that's where everything can be stored.
        - [ ] Helps with making sure that I have all of my stuff in one place

# Weekdays

## Monday

- [ ] Do the bug and improvements triage, send Ryan what I think needs to be done
- [ ] Check in on the tasks that everyone’s assigned, and just give them a bump that these are the things we want done by EOW

## Tuesday

- [ ] Prep for my 1:1s with the guys
    - [ ] Minh
    - [ ] Dimas
    - [ ] Falco
    - [ ] Alex

## Wednesday

- [ ] Prep for my 1:1 with Dimas

## Thursday

- [ ] Timesheet with all the receipts in it

## Friday

- [ ] Reflect on the week, feedback I've received, and what I'll do differently


