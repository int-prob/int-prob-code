# Focused Research Group in Integrable Probability

This is a GitHub pages repository for the [Integrable Probability FRG webpage](https://integrable-probability.github.io/). These ReadMe notes are intended to document how the webpage is organized, and facilitate its collaborative editing.

## Things to note first

### 1. Webpage is generated automatically

The source code is hosted here and is automatically compiled into a static HTML that is displayed as the webpage using [Jekyll](https://jekyllrb.com/). [Here](https://help.github.com/articles/using-jekyll-as-a-static-site-generator-with-github-pages/) is GitHub-specific documentation. In particular, any change in the code is reflected on the webpage (within a couple of minutes)

### 2. This is a public code repository

- This repository, including every change, is public
- There is a number of "collaborators" with direct access to modifying the website. Every change is recorded and can be easily reverted, so edits in general cannot break the website
- Any other GitHub user can submit edits (a "pull request") which can be approved by collaborators and included in the code

### 3. How to make changes

- Changes to the code can be made directly in browser. This is especially convenient for smaller changes
- For larger changes:
  - If you have access to changes in the main repositorym clone the git repository: `git clone https://github.com/integrable-probability/integrable-probability.github.io`, make changes, and then commit and push to GitHub
  - If not, fork the repository, make changes, commit and push. Then create a pull request
- You can also preview the local copy of the website by making Jekyll run a simple server. This requires a local installation of Jekyll. Details are explained [here](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/)

## Organization

Besides static pages such as this readme, the list of people, or the page with links to courses, there are two sources from which the content is generated "dynamically":

- The FRG google calendar containing events such as conferences (with details and links) on topics close to Integrable Probability, in which FRG members organize or participate in. The main page shows up to 10 upcoming events from this calendar, and all events (together with a google calendar) are listed in the events tab
- There is a blog-like functionality which powers the lists of publications, talks. Up to 7 new items are displayed on the main page. The blog posts are located in [this folder](https://github.com/integrable-probability/integrable-probability.github.io/tree/writing_readme/blog/_posts). One publication/talk = one file. The publications are pulled from the arXiv by last names of the participants in a semi-automated regime using the [script](https://github.com/lenis2000/arXiv_API). All other items such as publications and other blog entries can be added manually by making a new file. Any other content (pictures, PDFs, etc) can also be uploaded and displayed on the website using usual HTML

The static pages should be updated by hand. Overall, Jekyll provides very nice tools to reuse HTML code (such as in the top navigation bar), see the snippets in the \_includes folder

## Things which need constant maintenance
- arXiv updates by FRG members using the [script](https://github.com/lenis2000/arXiv_API)
- events using the FRG google calendar
- other updates like slides of talks, courses, etc.

## ToDos
1. Add a pretty picture or two on the front page and/or somewhere else
2. Link to homepages by graduate students if they exist
3. As FRG events (workshops, conferences, summer schools) are organized, create and maintain their dedicated webpages, possibly as subpages of this website
4. Create a forum-like space to discuss Integrable Probability, and open it to anonymous comments during FRG events. This item needs technical thinking: how to best organize a moderated forum; can we marry it to [Mathoverflow](https://mathoverflow.net), how to best run LaTeX at the forum, etc.
