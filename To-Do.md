## Start of Day

- [x] Check Calendar
- [x] Check status of AI apps ([link](https://dashboard.render.com/project/prj-d003snngi27c73ath6j0))
- [x] Check Slack messages and threads
    - [x] Create tasks for anything that needs doing
- [x] Email Check
- [x] Read over the importer incoming inputs
- [x] Review everyone else’s updates for the day
    - [x] AI Pod
    - [ ] Branching Pod
    - [ ] Enterprise bug bash pod
    - [ ] Onboarding pod
    - [ ] OAS (Hugo)
- [x] Review Linear notifications
- [x] Check triage tickets linear
- [x] Make sure deployments worked fine for my changes
- [x] LinkedIn check
- [x] Make sure my tickets for the next few days are well scoped and understood
- [x] Check weekday-based tasks
- [x] PR Reviews
- [x] Check on my outstanding PRs

## End of Day

- [ ] AI Repo CICD
- [ ] Test merged AI CLI Runner stuff
- [ ] Review PRs again
- [ ] Deployments - approve all of the stuff I'm merging in
- [ ] Look at deployments, for anything from me/AI test out and make sure its good to go

## What I want to get done this week
### Monday
- [ ] 
### Tuesday
- [ ] 
### Wednesday-
- [x] PR Reviews
### Thursday
- [x] Get the AskAI projects setup for the QA team to use - refer to those projects for details
- [x] PR Reviews
- [ ] Read over the importer stuff from previous day
- [ ] Worked on dataset improvements:
	- [ ] Broke out the dataset into what's stored on disk more - we have the negative cases, the forbidden words cases, and normal cases
	- [ ] Forbidden words are good on v1, v2
	- [ ] Negatives (ie OOS inputs) on v1 actually doesn't perform as well - v2 performs better, aside for GPT5.6 Terra and Luna that perform equally. Good news since its not a degradation:
		- [ ] Made [a ticket for this](https://linear.app/readme-io/issue/RM-17820/askai-v2-handles-bad-queries) - but its not something that we should actually worry about for now since this is better than current and is a long-term improvement
		- [ ] Fast-follow is fine but anything more is unneccessary
- [ ] Finished the ai seeding task - its simplified from what I was doing before:
	- [ ] Addressed anandBot comments - sent anand some info on this
	- [ ] @anand anandbot never resolved but I think its overkilling atm - assigned you for review: https://github.com/readmeio/ai/pull/919
	- [ ] Evals re-running for v1, v2 at present
	- [ ] Add in the delta achieved time-wise b/w the 3 models used, score-wise, and cost-wise
	- [ ] Get anand review until passed
- [ ] AskAI Judge/Dataset Improvements
### Friday
- [ ] [URLs embedded in askAI v2 responses](https://linear.app/readme-io/issue/RM-17823/askai-links-in-response)
	- [ ] Get the monorepo PR up at least
- [ ] Medium response length for monorepo
- [ ] AskAI - get the backend to return urls in-text
	- [ ] Note - this is something that will need some evals

## PR Reviews
- [ ] PR Reviews
    - [ ] `readme`
        - [x] https://github.com/readmeio/readme/pull/20176
    - [ ] `ai`
        - [x] https://github.com/readmeio/ai/pull/883 
    - [ ] `gitto`
        - [ ] 
    - [ ] `ai-cli-runner`
        - [x] https://github.com/readmeio/ai-cli-runner/pull/105
    - [ ] `cli`
        - [x] https://github.com/readmeio/cli/pull/38

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


