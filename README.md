Banshee Media Player web site
=============================

This repository contains the source files for the Banshee media player website, accessible at [http://banshee.fm](http://banshee.fm)

It is automatically transformed into a static site by Jekyll whenever updates are pushed to this repository on GitHub.

For more information on Jekyll and GitHub pages, see the [GitHub help](https://help.github.com/articles/using-jekyll-with-pages).

## Structure

#### Layouts

The content is based on 3 layouts:

  * `page` for general purpose pages. It display a navigation menu in the right sidebar if the `show-sidebar` variable is set to true

  * `page-release` for release notes. It automatically adds links to all other release notes in the right sidebar

  * `post` for blog posts

Those 3 layouts reuse several snippets, found in the _includes folder.

#### Sidebar menu

If enabled through the `show-sidebar` variable, the sidebar menu is populated automatically based on the `group`, `sidebar-group` and `order` variables.
For more details, see the comments in _includes/sidebar

#### Blog posts

In addition to the regular blog posts found in the _posts top-level folder, the release notes pages under /download/archives are also handled as blog posts. This was necessary to make sure they are listed in chronological order in the sidebar.

Those release notes pages can be distinguished from regular posts based on their 'archives' category. This is done for example in the RSS feed, where we only want regular posts.

## Contributing

If you find a problem on the web site, or if you want to help improve it, please [file an issue on GitHub](https://github.com/BansheeMediaPlayer/BansheeMediaPlayer.github.io/issues), or [submit a pull request](https://github.com/BansheeMediaPlayer/BansheeMediaPlayer.github.io/pulls).

To make sure your proposed changes work as expected, please validate them by generating the web site locally with Jekyll. You can also use GitHub codespaces or GitPod:

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://github.com/codespaces/new?hide_repo_select=true&ref=master&repo=16046940&machine=basicLinux32gb&devcontainer_path=.devcontainer%2Fdevcontainer.json&location=WestEurope)

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/BansheeMediaPlayer/BansheeMediaPlayer.github.io)