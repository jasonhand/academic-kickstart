# Contributing

Pull requests are appreciated.

On-call life is a Hugo site using the Academic theme.

When changes are made to the master branch of this repo, Netlify builds the site and pushes the static HTML and associated files to [https://oncall.life](https://oncall.life)

## Where content is stored

All content is stored in the [`content`](content/)  folder. There are two primary folders. 

Most of the existing content is stored in `content/post` but there are a few in `content/project`. 

Those are the "Phases of an Incident" Section of the site (*Detection, Response, Remediation, Analysis, Readiness*)

## Creating a NEW post

1. Create a new directory inside `post` using the nameing convention: `this-is-my-post` where the text exactly matches the title of the article separated by hyphens.
2. Create a new file inside the newly created directory named `index.md`.
3. Add the following header.

```markdown
---
title: This Is My Post
date: 2020-03-18
profile: false
image:
  placement: 3
tags: []
editable: true
---
```
4. Add your content using **markdown** syntax including
   1. Link to next article
   2. Link to at least one resource

5. Save, commit, and submit PR

Once I have reviewed the pull request and merged the new content, Hugo will build the new HTML and publish it at [https://oncall.life](https://oncall.life)

## Editing an existing post

**Method 1: (Direct on Github)**
1. Click on the **Edit this page** link at the bottom of the article
2. Edit and commit changes directly on Github
![](https://jhandcdn.blob.core.windows.net/blob/edit-post.gif)

**Method 2: (Local Dev Env)**
1. Navigate to the `index.md` file associated with the post and edit/save
2. Add/commit/push, and submit a PR

>**IMPORTANT:** Every article must fit somewhere in line with the current narrative. Think about how to transition the beginning and end of each article so that it stands on its own as a useful piece of content but also helps carry the reader along from the previous article and on to the next.