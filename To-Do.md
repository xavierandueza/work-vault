## Start of Day

- [x] Check Calendar
- [x] Check status of AI apps ([link](https://dashboard.render.com/project/prj-d003snngi27c73ath6j0))
- [x] Check Slack messages and threads
    - [x] Create tasks for anything that needs doing
- [x] Email Check
- [ ] Review everyone else’s updates for the day
    - [x] AI Pod
    - [x] Branching Pod
    - [x] Enterprise bug bash pod
    - [x] Onboarding pod
    - [x] OAS (Hugo)
- [x] Review Linear notifications
- [x] Check triage tickets linear
- [x] Make sure deployments worked fine for my changes
- [x] LinkedIn check
- [x] Make sure my tickets for the next few days are well scoped and understood
- [x] Check weekday-based tasks
- [ ] PR Reviews
- [ ] Check on my outstanding PRs

## End of Day

- [ ] AI Repo CICD
- [ ] Test merged AI CLI Runner stuff
- [ ] Review PRs again
- [ ] Deployments - approve all of the stuff I'm merging in
- [ ] Look at deployments, for anything from me/AI test out and make sure its good to go

## What I want to get done this week
### Monday
### Tuesday
- [ ] Do my 1:1 notes
- [x] Make sure that this gets merged + over the line: https://github.com/readmeio/readme/pull/20269
- [ ] Follow-up ticket for the askAI work - on disabled the other endpoint should be disabled just like what we do with the other one
- [ ] Get agents working for the following:
	- [x] [Project-scoped knowledge issue](https://linear.app/readme-io/issue/RM-17829/ask-ai-does-not-pull-answers-from-child-projects-when-project-scope)
		- [x] Note - this was probably an issue that'll be resolved with another merge, the inheriting v2 from parent issue. 
		- [x] Check on prod after this goes live.
	- [ ] Any other askAI v2 issue
	- [x] finish work on enterprise projects not getting their [custom prompts from parent projects](https://linear.app/readme-io/issue/RM-17831/custom-prompt-ignored-on-enterprise-projects-ask-ai-api) 
- [ ] Start up the work to use langfuse to get all of the information that we need - we don't actually need the retrieve tool calls
- [ ] Tool calling UI fixup - use w/e is on next for this UI
- [ ] Medium response length for monorepo
- [ ] AskAI - get the backend to return urls in-text

FOR UPDATE
- Note that I actually don't know how the `readme-enterprise` works in terms of the db - I don't know how this could impact results... Is it different somehow?
### Wednesday-
- [ ] PR Reviews
### Thursday
- [ ] Got the AskAI projects setup for the QA team to use - refer to those projects for details
### Friday
- [ ] PR Reviews
- [ ] Read over the importer stuff from previous day
- [ ] [URLs embedded in askAI v2 responses](https://linear.app/readme-io/issue/RM-17823/askai-links-in-response)
	- [ ] Got the PR up for monorepo and AI repo
	- [ ] @ryan would be good to get your POV on how we do the links - its intentionally really soft about how we link atm, any thoughts on what works best from the [loom](https://www.loom.com/share/085e289a669b4ae69287d9e0250c439c)?
	- [ ] Saw a small bug that I'll resolve early next week and move out for review
- [ ] Tool calling UI fixup - use w/e is on next for this UI
- [ ] Medium response length for monorepo
- [ ] AskAI - get the backend to return urls in-text
	- [ ] Note - this is something that will need some evals


## PR Reviews
- [ ] `readme`
	- [x] https://github.com/readmeio/readme/pull/20148
	- [x] https://github.com/readmeio/readme/pull/20209
	- [x] https://github.com/readmeio/readme/pull/20220
	- [ ] https://github.com/readmeio/readme/pull/20228
- [ ] `ai`
	- [ ] https://github.com/readmeio/ai/pull/936
	- [ ] https://github.com/readmeio/ai/pull/941
	- [ ] https://github.com/readmeio/ai/pull/954
	- [ ] https://github.com/readmeio/ai/pull/956
- [ ] `gitto`
	- [ ] 
- [ ] `ai-cli-runner`
- [ ] `cli`

## Backlog
- [ ] Tooling via lsps like anand mentioned → see what we can add for this...
- [ ] Ask everyone who's tackling a vertical - dig up the tickets that other teams can work on - probably a label on issues that are just "outsidePod" tickets:
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


