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
- [ ] Worked on dataset improvements:
	- [ ] Broke out the dataset into what's stored on disk more - we have the negative cases, the forbidden words cases, and normal cases
	- [ ] Forbidden words are good on v1, v2
	- [ ] Forbidden words on v1 actually doesn't perform as well - v2 performs better, aside for GPT5.6 Terra and Luna:
		- [ ] Made [a ticket for this](https://linear.app/readme-io/issue/RM-17820/askai-v2-handles-bad-queries) - but its not something that we should actually worry about for now since this is better than current and is a long-term improvement
		- [ ] Fast-follow is fine but anything more is unneccessary
- [ ] Post an update on AskAI v2 - where we're at and what needs check offs etc
	- [AskAI v2 responses shorter](https://linear.app/readme-io/issue/RM-17646/make-askai-v2-responses-shorter) 
		- me - will be done by EOD tomorrow but goes live with release
	- [Seed with initial data](https://linear.app/readme-io/issue/RM-17754/feed-in-vector-search-context-from-v1-pipeline-for-askai-v2-seeding) - this is still WIP - logic is all good but anandbot and my bot have been battling all day on this
		- Not doing any more anandbot reviews and just going to get @anand to review fully now
	- [Tool call activity fix](https://github.com/readmeio/readme/pull/19942) - this needs @ryan's UI improvements before I continue work on it
		- [ticket for ui](https://linear.app/readme-io/issue/RM-17677/fixup-ui-for-askai-v2-tool-calling) - @ryan you moved this to done but is it actually done? From memory you said you'd have done by EOW this week is that still on-track?
	- [unified search/askai](https://github.com/readmeio/readme/pull/19746) 
		- For this it seems that we just need @ryan to improve UI is this on track for EOW completion too? Ideally we can get merged by EOW so that we can get QA testing done early next week for it
	- [respecting locale in query suggestions](https://github.com/readmeio/readme/pull/20146)
		- Needs Readme review, AFAIK no additional UI pass
	-  [cross project askai security fix](https://github.com/readmeio/readme/pull/20036)
		- @falco is addressing issues with this today (Thurs AEST) and we can get merged tomorrow
		- This is existing issue however, shouldn't block us from going live.
	-  [ask ai button polish](https://github.com/readmeio/readme/pull/20176)
		- Got eng approval just needs UX approval from @ryan?
	- [AskAI v2 to include links in text](https://linear.app/readme-io/issue/RM-17823/askai-links-in-response) rather than "related docs"
		- Starting on this tomorrow, will have a PR up for monorepo changes if any are required so we can get merged ASAP.
- [ ] Finish the ai seeding task - its simplified from what I was doing before:
	- [ ] Adress anandBot comments
	- [ ] Re-review myself after changes go live
	- [ ] Test on the cases that I have locally for this
	- [ ] Re-run the evals cases
	- [ ] Add in the delta achieved time-wise b/w the 3 models used, score-wise, and cost-wise
	- [ ] Get anand review until passed
- [ ] AskAI Judge/Dataset Improvements
### Friday
- [ ] Medium response length for monorepo - make sure that this is good
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
- [ ] Read over what anand said re: MCP onboarding
    - [ ] https://moekhalil.substack.com/p/mcp-onboarding-is-the-most-exciting?utm_source=tldrfounders
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

# Deadlines Agreed to

* MCP Metrics:
    * Should be testing next week
    * **Should be ready for slow GA by 24th July**
* Slack writer - end of next week (Fri 26th)
* AskAI V2
    * AskAI v2 24th July
* AI Importer - Thursday 2nd July release - Erdman did some retesting last week again, some more feedback...
* **_Agent Metrics - we've started gathering the data, when do we want to release?_**
    * **_What work is actually left on this? Just UI and approvals?_**
* Having it so that askAI can look over all public branches:
    * This MUST wait for askAI v2, I'm not incorporating into tests and we need a clear before/after break


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


