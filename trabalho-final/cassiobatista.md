# Trabalho Final de Cassio Batista ([@cassiobatista](https://github.com/cassiobatista))

## [1pt] Task 1: Translation on Hugo Academic Template
Hugo is a framework based on Google's Go language for building static pages in
GitHub or GitLab. Among the several templates already created to make
developer's lives easier, there is the Academic template (check 
[this](https://sourcethemes.com/academic/) and
[this](https://github.com/gcushen/hugo-academic) 
links), which has a typical layout of an online CV. My accepted contribution in
in [PR #1121](https://github.com/gcushen/hugo-academic/pull/1121) was to
translate most of the Brazilian Portuguese stuff that goes in HTML hyperlinks.

## [3pt] Task 2: Small functionality on Hugo Academic Template
I've solved [issue #1108](https://github.com/gcushen/hugo-academic/issues/1108),
which was scheduled to be solved and released on version 4.4 of the Hugo
Academic framework. The current version provides some static, fixed buttons to
share a publication page on social media such as Facebook or Twitter. But let's
say you didn't want the Facebook button to be there. At the current version you
would have to edit an HTML file where the URL and the icons are "hardcoded" and
comment the Facebook list item. This is not very intuitive. My contributtion,
submitted on [PR #1131](https://github.com/gcushen/hugo-academic/pull/1131) now
allows this configuration to be performed inside the publication's own
`index.md` file, which is more accessible to the user/site dev. The social
networks are defined as lower case strings inside the `social` list (toml-like
configuration), and through some golang code inside the HTML I can read theses
config parameters and put them to the GUI automatically in the order they're
defined on the list. Therefore, going back to the aforegiven example, I could
just commented the Facebook item on the index markdown's list and *voilà!*
Facebook would be now gone as social sharing button.

## [1pt] Task 3: Improve Multilingual documentation on Beautiful Hugo
The documentation for [Beaultiful Hugo](https://themes.gohugo.io/beautifulhugo/)
theme for GitHub/GitLab static pages did not give any clue on how to enable the
multilingual functionality, although it has more than 10 languages available. 
Therefore, I have submitted 
[PR #285](https://github.com/halogenica/beautifulhugo/pull/285) with a new
section on README that instructs the user on how to set the configuration
parameters to enable switching the default language directly at the navigation
bar (top-right corner).

<!--
## [1pt] Task 4: Bug report on XFCE 4.4
There's something really when trying to load an image from a non-default
repository (such as `~/Dropbox/wallpapers` since the Dialog box won't let me.
I'll report this tomorrow
-->
