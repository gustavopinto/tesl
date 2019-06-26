# Relatório do Trabalho Final - Cassio Batista ([@cassiobatista](https://github.com/cassiobatista))

* Nome completo: Cassio Trindade Batista
* Nível: Pós-Graduação
* Matrícula: 201720080005

[Hugo](https://gohugo.io/) (see it on [GitHub](https://github.com/gohugoio/hugo) 
and at the [official webpage](https://gohugo.io/))
is a framework based on Google's Go language for building static pages in GitHub
and GitLab. Among the several templates already created to make developer's
lives easier, there is the **Hugo Academic** template (check the
[Hugo themes page](https://themes.gohugo.io/academic/) and
[official GitHub repo](https://github.com/gcushen/hugo-academic) 
links), which has a typical layout of an online CV; and the **Beautiful Hugo**
template (check [Hugo themes page](https://themes.gohugo.io/beautifulhugo/) and 
[official GitHub repo](https://github.com/halogenica/beautifulhugo) links) which
is a more general template for a personal (or group, although it does not seem
to be the real purpose) webpage.

## Translation on Hugo Academic 
- type: translation
- problem: multilingual for Portuguese still in English
- solution: translate most of the Brazilian Portuguese stuff that goes in HTML 
hyperlinks ([PR #1121](https://github.com/gcushen/hugo-academic/pull/1121)).
- status: :heavy_check_mark: accepted
- grade: 1 pt

## Customise pulication share buttons on Hugo Academic 
- type: small functionality
- problem: The current version provides some static, fixed buttons to
share a publication page on social media such as Facebook or Twitter. But let's
say you didn't want the Facebook button to be there. At the current version you
would have to edit an HTML file where the URL and the icons are "hardcoded" and
comment the Facebook list item 
([issue #1108](https://github.com/gcushen/hugo-academic/issues/1108)).
- solution: allow this configuration to be performed inside the publication's 
own `index.md` file, which is more accessible to the user/site dev. The social
networks are defined as lower case strings inside the `social` list (TOML-like
configuration), and through some golang code inside the HTML I can read theses
config parameters and put them to the GUI automatically in the same order 
they're defined on the list
([PR #1131](https://github.com/gcushen/hugo-academic/pull/1131)).
- status: :heavy_check_mark: accepted
- grade: 3 pt

## Improve multilingual documentation on Beautiful Hugo
- type: documentation
- problem: the documentation of Beautiful Hugo theme did not give any clue on 
how to enable the multilingual functionality, although it has more than 10 
languages available. 
- solution: new section on README that instructs the user on how to set the 
configuration parameters to enable switching the default language directly at 
the navigation bar (top-right corner)
([PR #285](https://github.com/halogenica/beautifulhugo/pull/285)).
- status: :hourglass_flowing_sand: waiting for approval (or rejection...)
- grade: 1 pt

---

## Members section page on Beautiful Hugo
- type: big functionality
- problem: no section to present members of a group or company or organization
- solution: new members section layout
([PR #287](https://github.com/halogenica/beautifulhugo/pull/287)).
    - based on the Tags layout because of its awesome collapsible panels
    - partial layout created in `layouts/member-card.html` to display an avatar 
    and the user description side by side
    - some buttons included leading to the social media of the member via
    [Font Awesome](https://fontawesome.com/icons?d=gallery&m=free), and some
    academic ones I had to add via
    [Academicons](https://jpswalsh.github.io/academicons/) CSS file
- status: :hourglass_flowing_sand: waiting for approval (or rejection...)
- grade: 3.5 pt


### Task 4.1: Publication section
Submitted on [PR #286](https://github.com/halogenica/beautifulhugo/pull/286),
this contribution solves 
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
created a section theme specifically for publications by modifying the tags 
section. Now all I had to do was to create some high-level Markdown-based 
interface for the users to insert their publications into the newly created 
section, which goes inside the `content/publication/` dir.

To do so, I had to make another amazing *almost*-contribution to a script called
`parse_bib`, which I found by messing around the issues of the Hugo Academic
template. The [original project on GitHub](https://github.com/apetros/parse_bib)
uses the Python `bibtexparser` library to extract publication info directly from
the LaTeX's BibTeX .bib files and insert that info into Markdown files (actually 
it is most TOML configuration defined on the page front matter than Markdown
itself). I decided to work on the script because I was too lazy to manually
input all the info from the .bib file into the markdown front matter content.

So I created a 
[fork on my own GitHub account](https://github.com/cassiobatista/parse_bib/tree/beautiful-hugo)
and adapted the script to my needs: converting a .bib file to Markdown with YAML
front matter (used in Beautiful Hugo rather than the TOML used on Hugo
Academic). But I have made so much improvements that I almost created a totally 
independent script, since the `bibtexparser` library had
too much limitations I decided to switch to `pybtex` (https://pybtex.org/). The
advantage of `pybtex` is that it is easy to create plain text endnotes for
publications, since I wanted to show endnotes at the title of the collapsible
panels (in spite of being possible, which definitely cannot be said about the
`bibtexparser` lib). When the endnote was clicked and therefore the panel was 
expanded, the .bib file entry could be shown to the reader alongside the
referred paper abstract, and this was easier
to do with `bibtexparser` because `pybtex` presents some problems when dealing 
with latex workarounds for non-ascii characters (such as `\~`, `\^`, etc., which
are usual for given names in Brazilian Portuguese).

And I also switched from `getopt` to `argparse` which is more pythonic :) The
thing is I'm still thinking about submitting a PR to this script because it is
kind of serving another purpose now.
