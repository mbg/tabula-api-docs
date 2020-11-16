# Template repository for (module) websites with Sitebuilder automation

This repository contains a template for automating Sitebuilder websites. Some configuration is required:

1. If you do not already have an [external user account](https://warwick.ac.uk/services/its/servicessupport/web/sign-on/externalusers) (required for Sitebuilder API access), create one
2. Give the external user account the required permissions on the Sitebuilder page you want to automate
3. Create two secrets named `SB_USER` and `SB_PASSWORD` in your fork of this repository with the username and password for the external user account, respectively
4. Modify `sitebuilder.yaml` to suit your needs. [Full documentation for the format of this file is available](https://github.com/mbg/uow-apis/blob/master/docs/Sitebuilder/Sync.md).

That is all the configuration that is required. Once completed, all commits you push to the `master` branch will run the GitHub workflow that will update the pages configured by `sitebuilder.yaml`.