# Problem
- Current askAI judge tries to do too much
- It has different types of data that it is trying to validate

## Restraints
* An evaluator MUST run on all data points from an input.

## Quick Wins

### Fake Question Inputs
- These are things that we don't want as a part of the main dataset - they're unique inputs that we will treat differently
- These can be removed entirely from the original testing set without changing the original prompt
- Needs its own prompt.
## Update the Judge to identify and score based on data points
- Current scrores aren't very strong, they're ultimately VERY vibe-based
- Update this so its a score between 0-1 that's about the amount of datapoints in ground truth
- The dataset for this still won't be amazing, however its better that we start moving towards this and we can likely start seeing some differentiation in results.

- Note that I'll need to actually get the core data points for this.

## Ensure that we have the page type and slug that must be linked to
- we need to make sure that the links that we expect are showing up as expected.
- unique combination of:
	- subdomain
	- slug
	- doc type
	- Note - because of custom domains this actually needs to be handled on the AI server - so that we can validate that also we get the FULL proper links that we expect

## Larger work/fixes
### Come up with a set of actual new questions based on staging data:
* Manual process to start with to make sure I know what I'm looking for and wanting
* Keep overall simple for now
* Focus on targeted questions
* Make sure that the ground truth is more on the key points the ground truth needs to hit on
- Come up with ~20 testing samples, all good quality with good metadata around it.

### Judge - retrieved content disagrees with ground-truth
- So we can catch drift better

# Dataset

This is a list of things that we should include in the new dataset:
## Input
- question - str
- projectSubdomain - str - the main subdomain

Projects:
```ts
export interface ProjectDetails {
  name: string;
  subdomain: string;
  description?: string;
}
```

Customization:
```ts
export interface Customization {
  advancedInstruction?: string;
  answerLength?: 'long' | 'medium' | 'short' | 'unrestricted';
  customTone?: string;
  defaultAnswer?: string;
  forbiddenWords?: string;
  hideSources?: boolean;
  tone?: string;
}
```

## Expected Output
- a list of facts - so a list of strings.
- a list of link data:

```ts
export interface Links {
  subdomain: string;
  type: 'docs' | 'reference' | 'changelog' | 'recipe' | 'discuss'
  slug: string;
  customDomain?: string;
}
```

## Metadata
```ts
export interface Metadata {
	difficulty: 'easy' | 'medium' | 'hard';
}
```
