# Contributing

Thanks for helping. This applies to every repository in the organisation unless the repository has its own guide; the main repository's guide is at <https://github.com/runtime-bridge/rbridge/blob/main/CONTRIBUTING.md>.

- Open an issue for anything bigger than a small fix, so we can agree on the approach first.
- One logical change per pull request, with tests. Unit tests run against fake runtimes and need no accounts.
- Explain any new dependency: what it is for, its licence and its size. The SDKs have no third-party dependencies and should stay that way.
- rbridge must never read provider credentials. Changes that do will not be accepted.
- Commit messages: a short imperative subject line, a blank line, then the reason for the change.
