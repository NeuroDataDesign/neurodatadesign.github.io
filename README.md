# NeuroData Design

This is the website for [Neuro Data Design](neurodatadesign.io), a class in the BME Department at JHU.

## Important pages
- [About](https://github.com/NeuroDataDesign/neurodatadesign.github.io/blob/master/_pages/about.md)
- [Syllabus](https://github.com/NeuroDataDesign/neurodatadesign.github.io/blob/master/_pages/syllabus.md)
- [Join](https://github.com/NeuroDataDesign/neurodatadesign.github.io/blob/master/_pages/join.md)

## Onboarding new TAs

Follow [this guide](https://github.com/NeuroDataDesign/neurodatadesign.github.io/blob/master/future/onboarding.md) to onboard new TAs.

## To run locally (not on GitHub Pages, to serve on your own computer)

1. Clone the repository and made updates as detailed above
1. Make sure you have ruby-dev, bundler, and nodejs installed: `sudo apt install ruby-dev ruby-bundler nodejs`
1. Run `bundle clean` to clean up the directory (no need to run `--force`)
1. Run `bundle install` to install ruby dependencies. If you get errors, delete Gemfile.lock and try again.
1. Run `bundle exec jekyll liveserve` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change.
