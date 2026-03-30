# docker-build

This is an orphan branch whose only purpose is to host the GitHub Actions
workflow in [`.github/workflows/docker-build.yml`](.github/workflows/docker-build.yml).

The workflow is triggered manually, takes an upstream `attestantio/vouch` tag as
input, checks out that tag, merges this fork's `multi-arch-dockerfile` branch,
and builds and pushes a multi-architecture Docker image to GitHub Container
Registry.

The branch is intentionally kept minimal so it can act as a dedicated
workflow-only branch, separate from the main repository history.
