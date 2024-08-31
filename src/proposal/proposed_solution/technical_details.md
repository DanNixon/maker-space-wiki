# Technical Details

## Things used

Only three software/services are used by this solution:

- [GitHub](https://github.com/)
- [mdBook](https://github.com/rust-lang/mdBook)
- [Cloudflare](https://www.cloudflare.com/)

I shall skip explaining what GitHub and Cloudflare are because most will already know and we already use them.

### mdBook

mdBook is a static site generator, specifically designed to generate documentation in the form of books.
Whilst "book-centric", you can replace the word "chapter" with "document" and it is just a hierarchical collection of documents.

It is fed plain old Markdown documents, containing nothing extra apart from the content you wish to display.
The pages can be written using whatever Markdown editor the author chooses.
GitHub's online Markdown rendering will show an accurate representation of what mdBook will render in the "main body content" area for a specific document.

It is a single binary with no outside dependencies that is available for all three major platforms.
It is a core part of the documentation tooling for the Rust programming language, so is not going to go away overnight.

## Source files

The source files will be in a repository in the [MakerSpaceNewcastle](https://github.com/MakerSpaceNewcastle/) organisation on GitHub.
The layout/content of the repository will be pretty much identical to the one that contains this demo wiki, which you can view [here](https://github.com/danNixon/maker-space-wiki).

## Publishing process

Changes will be made via a Pull Request, this is so that the site can be built to verify it is syntactically correct.
Pull Requests can only be merged if the GitHub Action passes.

We may choose to use this as a means of having another member review the contents, or have ownership of documents (e.g. Iain might own the membership and induction related documents, and must approve changes to it), however I suggest this be something we do later if the need arises.

Once a Pull Request is merged, a GitHub Action will build the site and publish it to Cloudflare Pages.
This typically takes less than one minute.

## Revocation of changes

The preferred method is via undoing the changes in the source Markdown files, either by `git revert` (or it's equivalent via the GitHub website) or by making the appropriate changes and following the above publishing process.

If there is a need for a quick revert to an older version, then this can be done via the Cloudflare Pages dashboard.

## History

Deployments to Cloudflare Pages are reported in GitHub as deployments, and the previous versions of the site are available to browse if desired (see for this wiki [here](https://github.com/DanNixon/maker-space-wiki/deployments)).

The history of the source files can be viewed, managed and manipulated via all the standard Git methods if the need to do so should arise.
