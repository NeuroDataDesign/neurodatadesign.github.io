---
layout: archive
title: "PR Guidelines"
permalink: /pr/
author_profile: true
---

## Deadlines for your end of semester PRs
Your assignment is to have PR(s) MERGED by the end of the semester. This means that you need to give the TAs/maintainers of these repos ample time to review your PR and provide feedback, for you to respond to that feedback, and potentially go through multiple rounds of feedback and response. TAs/maintainers are not responsible for your PR not being merged at the end of the semester if you do not give us enough time to review your PR(s).
 - If you PR by **Fri, Nov 22nd**, you will recieve feedback before **Mon, Dec 2nd**. We **strongly recommend** you at least make an initial PR and request feedback by this date. 
 - If you PR by **Fri, Dec 6th**, you will recieve feedback before **Fri, Dec 13**. 
 - Your PR(s) must be merged by the class final date: **Tues, Dec 17th**.

## Requirements for your end of semester PRs
Your PR for the end of the semester should contain the following (where applicable for your particular project): 
 - CODE for whatever algorithm/function/class/etc. for whatever you are working on 
 - TESTS for the code above (tests that actually run in pytest and give True/False output)
 - TUTORIAL notebook for the code above. Here are examples in [GraSPy](https://graspy.neurodata.io/tutorial.html) and [sklearn](https://scikit-learn.org/stable/tutorial/index.html). These should explain a bit about what your algorithm is useful for (or not useful for) for a beginner, and demonstrate how one can use your code.
 - PROOF that your algorithm works and produces the same, expected output as the original algorithm. This could be reproduction of figures in papers, comparison of numerical results between your code and established implementations. This may or may not be similar content that is in your TUTORIAL or TESTS. This is the only part of your deliverables that may not be included in the PR itself but could be in a separate notebook that you send to us. The key thing here is that your results need to be clearly summarized so that we can understand your proof without much effort.

## General guidelines for making PRs
 - You should follow all of the contribution guidelines for whatever package you are PRing into. For example, [here](https://graspy.neurodata.io/contributing.html) are the guidelines for GraSPy. This includes giving the PR a descriptive title and filling out all of the boxes in the PR description.
 - You should make sure that you are only making the changes that you described in your PR. Always check the `Files changed` tab to see if you have made any unnecessary additions.
 - Make sure that you start with a clean version of whatever branch you want to merge into. Many of you incorporated changes that other people made to `master` in the NDD fork of your package. Then when you made your PR, the PR reflected many changes that were not listed as something you were trying to change. 
 - Make sure that tests and other checks (Travis) pass, this may take ~20-30 minutes after submitting your PR.
 - Don't make a PR into a real package (e.g. mainline Graspy, Sporf, ndmg, Sklearn, etc.) unless you do all of the above.

