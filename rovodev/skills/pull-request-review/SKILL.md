---
name: pull-request-review
description: Review pull request referenced by a github.com URL
---

Prerequisites
-------------

github cli (`gh`) is installed

If needed, authenticate via `gh auth`

How to review a pull request
----------------------------

Inputs: github.com pull request URL such as https://github.com/getoutreach/client/pull/45120 - referenced further as <gh-url>

Use `gh pr view <gh-url>` to read pull request description. The description may further reference a Jira item with further details.
`gh pr diff <gh-url>`  allows to see code changes`.


Determine if the pull request is complete, doesn't introduce regressions or error and addresses the desired goal.
The current repository contains full code of the given pull request for a reference.
Review code changes in the pull request carefully and make sure that there are no side effects, no unintended or uncaught exceptions, and edge cases are covered.
In case of any issues, propose solution.
