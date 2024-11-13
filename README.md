# SouthPAN Receiver Documentation

GitHub Pages website providing documentation for configuring GNSS receivers and devices to use the [Southern Positioning Augmentation Network (SouthPAN)](https://www.ga.gov.au/scientific-topics/positioning-navigation/positioning-australia/about-the-program/southpan) Open Services.

The website is built with [Jekyll](https://jekyllrb.com/) and uses the [Just the Docs](https://just-the-docs.com/) theme.

## Updating

There are two main ways of updating the documentation:

>Note: For large changes it is preferred to commit changes to a new branch, and then merge to `main` with a pull request so that they can be reviewed by someone else.

1. Locally:

    - Clone the repository `git clone https://github.com/frontiersi/southpan-receiver-docs.git`.
    - Commit changes to your local version, these can be previewed by [building locally](#building-locally).

2. On GitHub:

    - Changes can also be made directly on GitHub, however these changes cannot be previewed.
    - Visit the repository on GitHub [https://geoscienceaustralia.github.io/SouthPAN-GNSS-Receiver-Documentation/](https://geoscienceaustralia.github.io/SouthPAN-GNSS-Receiver-Documentation/).
    - To edit an existing file, navigate to the file, then click the `edit` button.
    - To create a new file, navigate to the directory to create the file, then click `Add file` &rarr; `Create new file`.
    - To upload a file, navigate to the directory to upload the file, then click `Add file` &rarr; `Upload files`.

>Note: It typically takes about 5 minutes for new changes on the GitHub repository to be reflected on the website.

## Formatting & Theming

The [Just the Docs](https://just-the-docs.com/) theme is used, which provides a hierarchical documentation structure, a sidebar for navigation also a search functionality.

They also provide a [Markdown guide](https://just-the-docs.com/docs/index-test/) ([raw code](https://raw.githubusercontent.com/just-the-docs/just-the-docs/main/docs/index-test.md)) which shows basic markdown syntax and formatting.

## Building Locally

To build the website locally, you will need [Ruby](https://www.ruby-lang.org/en/) and [Bundler](https://bundler.io) installed on your computer.

The project uses the [GitHub Pages Ruby Gem](https://github.com/github/pages-gem) which allows Bundler to setup the dependencies required to build the Jekyll environment locally.

1. Clone or download this repository.
2. Change your working directory to the root directory of the repository.
3. Run `bundle install`.
4. Run `bundle exec jekyll serve` to build your site and preview it at `localhost:4000`.
5. Changes will be reflected automatically in the preview.

The built site is stored in the directory `_site`.
