# READ ME

This repository is for the published presence of Amaranthos on Github.

While this is now serving as our homepage, that will change over time when we install [gitea](https://docs.gitea.io/en-us/)

We use 2 different models currently...
Jekyll controls the theming, while we use[pandoc](https://pandoc.org/) to assembly pages.

The .devcontainer here is a full pandoc and jekyll development environment. Changes here can be published automatically through testing and ci/cd.

We also use Jekyll Themes:

Previewing the theme locally
If you'd like to preview the theme locally (for example, in the process of proposing a change):

Clone down the theme's repository (git clone https://github.com/pages-themes/time-machine)
cd into the theme's directory
Run script/bootstrap to install the necessary dependencies
Run bundle exec jekyll serve to start the preview server
Visit localhost:4000 in your browser to preview the theme