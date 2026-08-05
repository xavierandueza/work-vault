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

## Larger work/fixes
### Come up with a set of actual new questions based on staging data:
* Manual process to start with to make sure I know what I'm looking for and wanting
* Keep overall simple for now
* Focus on targeted questions
* Make sure that the ground truth is more on the key points the ground truth needs to hit on
- Come up with ~20 testing samples, all good quality with good metadata around it.

### Judge - retrieved content disagrees with ground-truth
- So we can catch drift better
