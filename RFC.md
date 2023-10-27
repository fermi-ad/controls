# Request for Comments (RFC)

Many changes, including bug fixes and documentation improvements, can be implemented and reviewed via the normal GitHub pull request workflow.

Some changes, however, are “substantial”, and we ask that these be put through a design process and produce a consensus among the Controls team.

The “RFC” (request for comments) process is intended to provide a consistent and controlled path for new features to enter the control system.

[Active RFCs](https://github.com/fermi-ad/controls/discussions/categories/request-for-comments-rfcs) can be found in the discussions.

[Implemented RFCs](./rfcs) can be found in the RFCs directory of this repo. These function as specifications for the implementation.

## When to use this process

You should consider using this process if you intend to make “substantial” changes to hardware, code, services, architecture, or documentation. Some examples that would benefit from an RFC are:

- A new feature that creates a new API surface area and would require a feature flag if introduced.
- The removal of features that have already shipped as part of the release channel.
- The introduction of new idiomatic usage or conventions, even if they do not include code changes to code.

The RFC process is a great opportunity to get more eyes on a proposal before it is implemented in a released control system version. Quite often, even proposals that seem "obvious" can be significantly improved once a wider group of interested people can provide feedback.

The RFC process can also help encourage discussions about a proposed feature as it is being designed and incorporating important constraints into the design, while it’s easier to change before the design has been fully implemented.

Some changes do not require an RFC:

- Rephrasing, reorganizing or refactoring addition or removal of warnings
- Additions that strictly improve objective, numerical quality criteria (speedup, better browser support)
- Additions only likely to be noticed by other Controls contributors, invisible to users.

## The process

In short, to get a major feature added to the control system, one usually first puts up a Discussion on GitHub. At that point, the RFC is ‘active’ and may be implemented with the goal of eventual inclusion into the control system.

- [Open a new GitHub discussion](https://github.com/fermi-ad/controls/discussions/new?category=request-for-comments-rfcs) in the RFC category
- Fill in the RFC. _Put care into the details: RFCs that do not present convincing motivation, demonstrate an understanding of the impact of the design, or are disingenuous about the drawbacks or alternatives tend to be poorly received._
- As the RFC will receive design feedback from the larger community, you should be prepared to revise it in response. So, build consensus and integrate feedback. RFCs that have broad support are much more likely to make progress than those that don’t receive any comments.
- Eventually, Controls will decide whether the RFC is a candidate for inclusion in the control system.
- RFCs that are candidates for inclusion in the control system will enter a “final comment period” lasting three calendar days. A comment will signal the beginning of this period.
- Controls may reject an RFC after the discussion has settled, and comments summarizing the rationale for rejection have been made. Someone should then add the label “status: rejected”.
- An RFC may be accepted at the close of its final comment period. A team member will add the label “status: accepted”.

## The RFC lifecycle

Once an RFC becomes active, the authors may implement it and submit the feature as a pull request to the controls repo. Becoming ‘active’ is not a rubber stamp, and in particular, still does not mean the feature will ultimately be merged; it does mean that Controls has agreed to it in principle and is amenable to merging it.

Furthermore, the fact that a given RFC has been accepted and is ‘active’ implies nothing about what priority is assigned to its implementation nor whether anybody is currently working on it.

Modifying active RFCs can be done by editing the discussion/commenting on it. We strive to write each RFC in a manner that will reflect the final design of the feature, but the nature of the process means that we cannot expect every accepted RFC to actually reflect what the end result will be at the time of the next major release.

## Implementing an RFC

The author of an RFC is not obligated to implement it. The RFC author (like any other developer) is welcome to post an implementation for review after the RFC has been accepted.

If you are interested in working on implementing an ‘active’ RFC but cannot determine if someone else is already working on it, feel free to ask (e.g., by leaving a comment on the associated issue).

## Reviewing RFCs

Controls will attempt to review some set of open RFC discussions regularly.

Every accepted feature should have a champion representing the feature and its progress.

_This documentation was seeded from: [https://www.gatsbyjs.com/contributing/rfc-process/](https://www.gatsbyjs.com/contributing/rfc-process/)_
