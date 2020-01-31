---
layout: archive
title: "PR Guidelines"
permalink: /pr/
author_profile: true
---

## General requirements for PRs
In general, PRs should contain the following (where applicable for your particular project): 
 - CODE for whatever algorithm/function/class/etc. for whatever you are working on 
 - TESTS for the code above (tests that actually run in pytest and give True/False output)
 - TUTORIAL notebook for the code above. Here are examples in [GraSPy](https://graspy.neurodata.io/tutorial.html)
  and [sklearn](https://scikit-learn.org/stable/tutorial/index.html). 
  These should explain a bit about what your algorithm is useful for (or not useful for)
   for a beginner, and demonstrate how one can use your code.
 - PROOF that your algorithm works and produces the same, expected output as the original
  algorithm. This could be reproduction of figures in papers or comparison of numerical
   results between your code and established implementations. 
   This may or may not be similar content that is in your TUTORIAL or TESTS. 
   This is the only part of your deliverables that may not be included in the PR itself
    but could be in a separate notebook that you send to us and link to in the PR description. 
    The key thing here is that your results need to be clearly summarized so that we can 
    understand your proof without much effort.

## Review process

Asking someone to review your code is helpful for the code author and the reviewer, but it
is also time consuming. Therefore, please resepect the time of 
the reviewer by checking over all of the guidelines here before requesting a review. If you 
are a reviewing someone's code, please make a full-fledged effort to provide constructive 
feedback. After another student has reviewed your code, and you have addressed all of their 
comments, you can request a review from the TAs.

[**Form for peer code review**](https://forms.gle/c15LWEEoHck9in5J6)

**Form to request TA code review**


## Checklist before requesting a review

### PR itself

- You should follow all of the contribution guidelines for whatever package you are PRing into.
 For example, [here](https://graspy.neurodata.io/contributing.html) are the guidelines for GraSPy.
 This includes giving the PR a descriptive title and filling out all of the boxes in the PR description.
- You should make sure that you are only making the changes that you described in your PR.
 Always check the `Files changed` tab to see if you have made any unnecessary additions.

### Style

- Abide by Python variable naming conventions, one description is
  [here](https://visualgit.readthedocs.io/en/latest/pages/naming_convention.html). Most
  variables should be `snake_case` and classes shoud be defined as `UpperCamelCase`,
  for example.
- Use descriptive variable names
- Remove as much "junk" from your code as possible before asking people to review it,
  this generally just means remove a ton of commented out code if you have it
- Keep line lengths short (Recommend <88 characters, definitely not more than 100). This
  includes docstrings.
- Use a formatting tool like [black](https://black.readthedocs.io/en/stable/). There are
  other options as well. Its best to just set up your IDE to run autoformatting every
  time you save so you don't have to think about it.

### Documentation

- Write docstrings for public classes and functions
- Add any new public classes and functions to be rendered by `sphinx`.
- If `netlify` is set up for this package, check that the changes you have made to the 
documentation are rendered appropriately.
- If making a large feature addition to a package, include a short notebook demonstrating
the purpose and usage of your addition with clear examples. 

### Tests 

- Write tests to do input validation, making sure that the appropriate errors are thrown
when improper input is passed. 
- Write simple performance tests to show that your algorithm gets the correct answer on 
a simulated or real data example. If using simulations, make sure to set the random seed.
- Make sure that tests and other checks (Travis) pass, this may take ~20-30 minutes after
 submitting your PR.
