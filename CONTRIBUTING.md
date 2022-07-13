# Contributing to Harness Community Repositories

We currently accept contributions to Drone as well as Harness CD Community.

# Proposing Changes to Drone

## Introduction

The Drone project's development process is design-driven. Significant changes to the project, libraries, or tools must be first discussed, and sometimes formally documented, before they can be implemented.

This document describes the process for proposing, documenting, and implementing changes to the Drone project.

## The Proposal Process

### Goals

- Make sure that proposals get a proper, fair, timely, recorded evaluation with a clear answer.
- Make past proposals easy to find, to avoid duplicated effort.
- If a design doc is needed, make sure contributors know how to write a good one.

### Definitions

- A **proposal** is a suggestion filed as a GitHub issue, identified by having the Proposal label.
- A **design doc** is the expanded form of a proposal, written when the proposal needs more careful explanation and consideration.

### Scope

The proposal process should be used for any notable change or addition to the project, libraries and tools. Since proposals begin (and will often end) with the filing of an issue, even small changes can go through the proposal process if appropriate. Deciding what is appropriate is matter of judgment we will refine through experience. If in doubt, file a proposal.

### Yaml changes

Drone is a mature project with thousands of active installations, as such, significant or breaking yaml changes are unlikely to be accepted.

### Process

- [Create an issue](https://github.com/drone/proposal/issues/new) describing the proposal.

- The proposal is followed by an initial discussion about the suggestion.
	- The goal of the initial discussion is to reach agreement on the next step:
		(1) accept, (2) decline, or (3) ask for a design doc.
	- The discussion is expected to be resolved in a timely manner.
	- If the author wants to write a design doc, then they can write one.

- If a Proposal issue leads to a design doc:
	- The design doc should be checked in to [the proposal repository](https://github.com/drone/proposal/) as `design/{number}-{shortname}.md`, where `{number}` is the GitHub issue number and `{shortname}` is a short title.
	- The design doc should address any specific issues asked for during the initial discussion.
	- It is expected that the design doc may go through multiple checked-in revisions.
	- Comments on the proposal should be addressed to the related GitHub issue.

- Once comments and revisions on the design doc wind down, there is a final discussion about the proposal.
	- The goal of the final discussion is to reach agreement on the next step:
		(1) accept or (2) decline.
	- The discussion is expected to be resolved in a timely manner.

- The author (and/or other contributors) do the work as described by the "Implementation" section of the proposal.

# Our review/merge process for issues:
We currently accept creating an issue on the following repos:
 - [Drone](https://github.com/harness/drone/issues)

We meet on a Tuesday morning (10am BST) every week
The team has a Github query that lists all open pull requests from the last 30 days from all repos in the Drone org (93) and all Drone repos in the Harness org (5)

From the list we choose the PR's that:

- Are the most obvious to fit with our guidelines and are likely to be merged without much 	interaction (quick wins)
- Will have a positive impact without negatively impacting an already large audience (PR's that don't change behaviour)
- Address bugs/subjects that are currently of interest to our roadmap
- Any others we have time for

- Once the list is generated, our 2 engineers agree a strategy to prevent overlapping effort and get started
- Near the end of the day (3pm - 4pm BST) we get together and discuss any PR's that are questionable so that a decision can be made on next actions taken
the remainder of the working day is spent taking those actions or returning to priority items if no further actions are required.

*During the day all or none of the PR's could be merged although there tends to be a few that have value and can be merged immediately. We intend to introduce stalebot in the near future, it's already implemented for the plugin marketplace repo, the intention is to remove any PR that has been sitting for over 30 days without a response. It will comment on a repo saying that it has become stale, and give the author 5 days to take an action (comment for example) to keep it open.*

For other issues please use our Discourse and file the issue under the [Drone Bugs Section](https://community.harness.io/c/bugs/17) or slack to bring issues to our attention.


## Help

If you need help with this process, please contact the project contributors by posting
to the [Slack channel](https://join.slack.com/t/harnesscommunity/shared_invite/zt-90wb0w6u-OATJvUBkSDR3W9oYX7D~4A).
