# Implementation Plan

A general idea of how this will be put into practice.

1. Create a Cloudflare Pages project named "makerspace-wiki" (or something close to that) under the Maker Space account
1. Create a repository named "wiki" under the MakerSpaceNewcastle GitHub organisation containing all but the content of the repository behind this wiki
1. Create an API key allowing publishing to the above project and store it as a repository Actions secret in the above repository
1. See that GitHub Actions publishes to the Cloudflare Pages project
1. Apply repository settings described in [technical details](./technical_details.md)
1. Apply DNS settings described in [technical details](./technical_details.md)
1. Move the repository behind this demo wiki under the MakerSpaceNewcastle organisation and archive it
1. Begin migrating content to/creating content on the new wiki
1. Once the new wiki contains all of the useful information from the old wiki, replace any wiki links with `wiki.makerspace.org.uk`
1. When we are certain that any useful content has been migrated from the old wiki, delete it.
