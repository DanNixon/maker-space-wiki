# Editing Workflow

Please note, this document is just an overview of the processes available, it is **not** documentation of how to author the wiki.
Actual documentation will be written in due course should this solution be selected.

In general, there are two options: editing entirely via the GitHub website, or editing locally with Git setup.
If you are comfortable with Git then you likely want to use the latter option, if you are new to Git or only need to make a small change then the former option is best.

## Making changes

### Editing an existing page

If you just want to edit a single page then you may follow the edit link in the top right hand corner of the page.
Assuming you are signed in to GitHub, this will take you directly to a page where you can edit the contents and submit a Pull Request.

### Editing the wiki using GitHub via the web browser

Files may be uploaded via the GitHub website (text or images) and edited via GitHub's text editor.
After uploading or editing files GitHub will prompt you to commit them and optionally create a Pull Request.

### Editing the wiki locally

I am lazily going to assume I don't need to say much here.
If you are familiar with Git then follow the usual create branch, do changes, commit, push, open Pull Request workflow.

It is possible to run mdBook locally, or just use any Markdown renderer you may already have to preview changes.

## After the Pull Request has been created

One may wish to ask for people to review it, e.g. if you have editing a page relating to the CNC mill then you may wish to ask David Pye to look over it.

Whenever a new commit is added to a Pull Request, a GitHub Action runs which builds the page and deploys it in a test environment, allowing to to see exactly what your changes will actually look like.
A bot will comment on the Pull Request with a link you can follow to read the wiki with your changes applied (always use the most recent comment).

If the bot did not post a comment, then check the status of the Action, it may show a red cross indicating that something has gone wrong.
You will have to inspect the logs to see exactly what the issue is, if it is an error from mdBook then they are usually pretty descriptive as to what is wrong.

When happy the PR is merged, an Action runs and the live wiki is updated.
