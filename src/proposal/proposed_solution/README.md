# Proposed Solution

The proposed solution is the following:

- setup a new wiki
- migrate any existing documentation from the existing wiki
- identify and write new desired documentation
- ???
- profit

## Why mdBook?

[mdBook](https://github.com/rust-lang/mdBook) is a mature, lightweight documentation tool that generates beautiful documentation from Markdown files.

The advantages that make it ideal for our purposes include:

- It uses Markdown, likely the most common document markup language used in the world of open software/hardware, free culture, hacking and geekery:
    - The EMF Camp badge and developer documentation is written in it.
    - The very large majority of things on GitHub, GitLab, and other OSS repositories are documented in it.
- It generates beautifully minimal documentation, making good use of screen real estate and styled tastefully out of the box.
- It is reactive, i.e. will scale to smaller screen sizes and still be readable and navigable.
- It has good theming out of the box, respecting the system native colour scheme and using optimal colours for e.g. Dyslexia.
- It has native search functionality, which works very well.
- It can format a document for printing if desired.

## So what does this actually mean in practice?

It depends, do you...

- [care about how this actually works?](./technical_details.md), or
- [just want to know how you would edit the wiki?](./editing_workflow.md)
