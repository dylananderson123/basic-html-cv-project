# Project 1 — Your CV in HTML

Build a single-page CV using **HTML only**. No CSS. No JavaScript. No frameworks.

It will look plain. That is correct and intentional — you are styling it next week.
This week is about one thing: choosing the right tag for the right piece of content.

---

## The rules

1. **No AI.** Not Claude, not ChatGPT, not Gemini, not Copilot. If Copilot is still
   enabled in VS Code, turn it off before you start.
2. **No Scrimba editor.** Open a blank file in VS Code and type it.
3. **No copying another CV's HTML.** Not from a template, not from a GitHub repo.
4. **MDN is allowed.** Looking up what a tag does is research. Looking up a finished
   answer is not.

You will get stuck on something obvious. Write down what it was — we will talk about
it on the call, and it is usually the most useful part of the whole exercise.

---

## Setup

```
cd ~/Desktop/Code
mkdir phase-0-cv
cd phase-0-cv
```

Copy `index.html` and the `assets/` folder from this starter into it, then:

```
git init
git add .
git commit -m "Add empty CV page"
```

Commit as you go. Not one commit at the end.

---

## What to build

`content.md` in this folder has all the text. Your job is to mark it up — not to
write it. If you would rather use your own real details, do that instead; just keep
the same sections in the same order so the structure matches.

`design/desktop.png` shows roughly what it should look like unstyled in a browser.
Do not chase the exact spacing — that is the browser's default stylesheet, not a
design. Match the **structure and order**, not the pixels.

---

## Requirements

### The document

- [ ] `<!DOCTYPE html>` on the first line
- [ ] `<html>` with a `lang` attribute
- [ ] A `<head>` and a `<body>`
- [ ] `<meta charset>` set correctly
- [ ] `<meta name="viewport">` set for mobile
- [ ] A `<title>` that would make sense as a browser tab and a Google result

### SEO and sharing

- [ ] `<meta name="description">` — one sentence, written for a human reading search results
- [ ] `<meta name="author">`
- [ ] Open Graph tags: `og:type`, `og:title`, `og:description`, `og:url`, `og:image`
- [ ] A favicon linked in the head (`assets/favicon.svg` is provided)

### The content

- [ ] A `<header>` with your name as the **one and only** `<h1>` on the page
- [ ] A `<nav>` holding your contact links
- [ ] A `<main>` wrapping the body of the CV
- [ ] Separate `<section>` elements for: About, Skills, Experience, Education, Projects
- [ ] Each section introduced by an `<h2>`
- [ ] Each job and each qualification wrapped in its own `<article>` with an `<h3>`
- [ ] `<ul>` and `<li>` for every list — skills, responsibilities, contact links
- [ ] `<time datetime="...">` for every date
- [ ] A `<footer>`
- [ ] Email as a working `mailto:` link
- [ ] External links that actually go somewhere

### Heading order

- [ ] Exactly one `<h1>`. Never skip a level — no `<h3>` without an `<h2>` above it.

---

## Before you say you're done

Read your own HTML top to bottom with the question: **"could someone understand the
shape of this page with the CSS switched off and the images gone?"** That is not a
metaphor — that is exactly how a screen reader and a search engine see it.

Then check:

- [ ] Every `<div>` you used — could a real tag do that job instead? Delete it if so.
- [ ] Paste the file into `validator.w3.org` and fix everything it complains about.
- [ ] `git log` shows more than one commit.
- [ ] Pushed to GitHub.

---

## On the call

Come ready to answer these out loud, no notes, with the file closed:

1. What does `<!DOCTYPE html>` actually do?
2. What is the difference between `<head>` and `<header>`?
3. Why should there only be one `<h1>`?
4. What is the difference between `<section>` and `<div>`? When would you use each?
5. Why does `<article>` exist — what makes something an article?
6. What is `alt` text for, and who reads it?
7. You wrote a `<meta name="description">`. Where does that text end up?
8. What would break if you removed `<meta charset="UTF-8">`?
9. Show me one tag you chose and defend it. Then show me one you're unsure about.

Then: open a blank file and type the document skeleton from memory while I watch.
Doctype, html, head, charset, viewport, title, body. That is the bar.
