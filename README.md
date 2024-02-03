# Release Flow

This organization is the home of various Application Lifecycle Management (ALM) tools, mostly around [Release
Flow](https://devblogs.microsoft.com/devops/release-flow-how-we-do-branching-on-the-vsts-team/) conventions.

The [Keep-a-Changelog Action](https://github.com/release-flow/keep-a-changelog-action) repo contains a GitHub Action to
drive versioning from a changelog. It's not related to Release Flow, but it's kinda handy for some scenarios.

## Other release flows

The [releaseflow.org](http://releaseflow.org/) website describes a slightly different form of release flow, which is (as
the site admits) just a 'trendy name for the Release Branching strategy'. This is unfortunate, as the form of Release
Flow described on the Microsoft blog, and implemented here, is different in one crucial way: in true Release Flow,
hotfixes to a release are first performed on the trunk branch then cherry-picked onto the release branch (with few
exceptions). In the release branching strategy, they suggest to fix the release branch and then cherry-pick onto the
trunk.
