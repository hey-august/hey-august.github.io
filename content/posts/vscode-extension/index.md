+++
title = 'Vscode Extension'
date = 2024-04-10T17:54:01-04:00
draft = true
+++

# From 0 to Published VSCode Extension

This blog post documents my experience building a new extension for VSCode from scratch.
While [I am learning JavaScript](./learning-javascript.md), I am not a JavaScript developer.
I'm even further from being a TypeScript developer, [despite their similarities]().

So, how did I write, test, and publish a polished extension on the VSCode Marketplace?

I did what technical writers do when we need to understand a new technical concept:

1. Scope
2. Read the docs
3. Google
4. Ask an LLM
5. Try, fail, and iterate

In case this looks very familiar to how developers solve problems, it's because [Technical Writers *are* developers](todo).
They are jacks-of-all-trades with broad subject knowledge of programming concepts,
paired with deep knowledge of documentation, product, and SDLC.

## Step One: Scope the project

The extension I wanted to write is a simple text formatter to automatically parse Markdown and other text files and add 
[semantic line breaks (sembr)](https://sembr.org).
Simply put, semantic line breaks are line breaks placed after each substantial unit of thought.

SemBr is an intuitive, yet underutilized, set of conventions.
No dedicated extension currently exists in the VSCode Marketplace, meaning that the tasks of checking or converting text to SemBr must be performed manually.

### MVP

My minimum viable product would be a single command to insert line breaks after full stops (periods) in plain text in Markdown files.

### Additional functionality

If I could successfully implement the MVP, I would move on to additional functionality:

- **Converting fixed-column line breaks**.

### Technical Scope

ChatGPT is a very powerful scoping tool.
I began this project by 