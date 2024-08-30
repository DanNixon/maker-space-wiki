# Solutions Considered

## Continue using PBworks and just update the content

Essentially keep on doing what we currently are, but perhaps with a bit of a push to keep the documentation up to date.

Pros:

- Low-ish effort
- The devil you know

Cons:

- Does not fix aesthetic issues
- Does not fix accessibility issues

## MediaWiki

Host a [MediaWiki](https://www.mediawiki.org/wiki/MediaWiki) instance and move documentation over there.

Pros:

- Very well proven platform
- Intuitive editor
- Search out of the box
- Accessible out of the box

Cons:

- Requires hosting somewhere (plus the ongoing maintenance this involves)

## mdBook

Use [mdBook](https://github.com/rust-lang/mdBook) to generate a static site containing our documentation, with source content hosted on GitHub.

Pros:

- Well proven platform
- Intuitive editor (via GitHub's markdown editor)
- Search out of the box
- Accessible out of the box
- Good review/discussion ability via GitHub Pull Requests
- Hosted for free on platforms we already use (GitHub and Cloudflare)

Cons:

- Git based contribution workflow is more of a barrier
