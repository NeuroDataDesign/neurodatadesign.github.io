## Peer review checklist

### PR itself (on GitHub)
- [ ] PR has a descriptive and succinct title.
- [ ] PR has a _brief_ description of what was changed.
- [ ] PR cites any related issues in the PR description (if applicable) and uses [closing keywords](https://docs.github.com/en/free-pro-team@latest/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword) for any issues that should be closed as a result of the PR.
- [ ] PR does not have any extraneous file changes associated with it. One common example of an extraneous change is one that was already made in the target branch, but is showing up as part of this PR under `Files changed`.
- [ ] PR does not have any unresolved merge conflicts.
- [ ] If implementing a major new feature or algorithm, a notebook demonstrating the proof of effectiveness is linked in the PR description. Depending on the feature, this kind of validation may take too long to run as a test or in a tutorial notebook. 

### Style
- [ ] Code follows Python variable naming conventions, one description is [here](https://visualgit.readthedocs.io/en/latest/pages/naming_convention.html). Most variables should be `snake_case` and classes shoud be defined as `UpperCamelCase`, for example.
- [ ] Code uses descriptive variable names throughout.
- [ ] Code has no commented out "junk code."
- [ ] Line lengths are short (recommended <88 chars). This includes docstrings. Note:  [black](https://black.readthedocs.io/en/stable/) tries to shorten line lengths but sometimes it is unable to do so automatically, especially for docstrings.

### Documentation
- [ ] Any new public classes/functions have docstrings. 
- [ ] Any new public classes/functions have been added to the appropriate `.rst` file [here](https://github.com/microsoft/graspologic/tree/dev/docs/reference) to be rendered by `Sphinx`.
- [ ] Any major new features (like a new algorithm) are accompanied by a succinct tutorial notebook. Or, if it is agreed upon with the maintainers that this is out of scope for the current PR, a new issue has been created specifying that we need a tutorial notebook for this functionality.
- [ ] Any new tutorial notebooks have been added to the appropriate folder [here](https://github.com/microsoft/graspologic/tree/dev/docs/tutorials) and included in the `.rst` file [here](https://github.com/microsoft/graspologic/blob/dev/docs/tutorial.rst) to be rendered by `Sphinx`.
- [ ] Modifications to the documentation render appropriately in the `Netlify` build.

### Testing
- [ ] New public classes/functions are tested to ensure they achieve the desired output.
- [ ] New public classes/functions are tested to ensure proper errors are thrown when invalid inputs are passed.
