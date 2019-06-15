# Trabalho Final de Cassio Batista ([@cassiobatista](https://github.com/cassiobatista))

## Task 1 [1pt]: Translation on Hugo Academic Template
[Hugo](https://gohugo.io/) (see it on [GitHub](https://github.com/gohugoio/hugo))
is a framework based on Google's Go language for building static pages in GitHub
and GitLab. Among the several templates already created to make developer's
lives easier, there is the Academic template (check
[this](https://sourcethemes.com/academic/) and
[this](https://github.com/gcushen/hugo-academic) 
links), which has a typical layout of an online CV. My accepted contribution in
in [PR #1121](https://github.com/gcushen/hugo-academic/pull/1121) was to
translate most of the Brazilian Portuguese stuff that goes in HTML hyperlinks.

## Task 2 [3pt]: Small functionality on Hugo Academic Template
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

**Edit:** PR was accepted (with some refactoring by the owner) on Jun 15, 2019 
:).

## Task 3 [1pt]: Improve Multilingual documentation on Beautiful Hugo
The documentation for [Beautiful Hugo](https://themes.gohugo.io/beautifulhugo/)
theme for GitHub/GitLab static pages did not give any clue on how to enable the
multilingual functionality, although it has more than 10 languages available. 
Therefore, I have submitted 
[PR #285](https://github.com/halogenica/beautifulhugo/pull/285) with a new
section on README that instructs the user on how to set the configuration
parameters to enable switching the default language directly at the navigation
bar (top-right corner).

## Task 4 [7pt]: Big functionality on Beautiful Hugo Template
I've created two additional pages for the Beautiful Hugo theme: the first one
for listing publications and the second to display all members in a research
group or company.

### Task 4.1: Publication section
Submitted on [PR #286](https://github.com/halogenica/beautifulhugo/pull/286),
this contributions solves 
[issue #283](https://github.com/halogenica/beautifulhugo/issues/283) by adding a
section for listing academic publications on the Beautiful Hugo theme. It
wasn't easy since I had to watch half of a
[Hugo Tutorial](https://www.youtube.com/playlist?list=PLLAZ4kZ9dFpOnyRlyS-liKL5ReHDcj4G3) 
on YouTube in order to understand how things work underneath the Hugo framework. 

I had to create a special section template file called `publication.html` under 
the `layouts/section`. I actually got some inspiration from the Tags section
available at the Beautiful Hugo theme itself, which has some 
[amazing collapsible panels](https://themes.gohugo.io//theme/beautifulhugo/tags)
defined in HTML (and perhaps some JavaScript that I haven't seen so far). So I
created a section theme specific for publications by modifying the tags section.
Now all I had to do was to create some high-level Markdown-based interface for
the users to insert their publications into the newly created section.

To do so, I had to make another amazing almost-contribution to a script called
`parse_bib`, which I found by messing around the issues of the Hugo Academic
template. The [original project on GitHub](https://github.com/apetros/parse_bib)
uses the Python `bibtexparser` library to convert publication info directly from
the LaTeX's BibTeX .bib files to Markdown (actually it is most TOML
configuration defined on the page front matter that Markdown itself). I decided
to work on the script because I was too lazy to manually input all the info from
the .bib file into the markdown front matter content.

So I created a 
[fork on my own GitHub account](https://github.com/cassiobatista/parse_bib/tree/beautiful-hugo)
and adapted the script to my needs: converting a .bib file to Markdown with YAML
front matter (used in Beautiful Hugo rather than the TOML used on Hugo
Academic). But I have made so much improvements that I almost created a totally 
independent script, since the bibtexparse library had
too much limitations I decided to switch to `pybtex` (https://pybtex.org/). I
also switched from `getopt` to `argparse` which is more pythonic :)

### Task 4.2: Members section
TBD.

<!--
## [1pt] Task 4: Bug report on XFCE 4.
There's something really wrong when trying to load an image from a non-default
repository (such as `~/Dropbox/wallpapers`) since the Dialog box won't let me.
I'll report this tomorrow
Edit: although it seems to be a still-non-solved bug, it's been already highly 
reported :(
- https://www.reddit.com/r/archlinux/comments/4zztq8/cannot_change_wallpaper_folder_on_fresh_install/
-->
