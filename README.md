# ormeilu/homebrew-tap

Homebrew formulae for tools published from
[ormeilu](https://github.com/ormeilu).

```sh
brew install ormeilu/tap/ytcli
```

`brew install user/repository/formula` taps this repository on the way, so
there is nothing to run first. `ormeilu/tap` is the short form Homebrew accepts
for a repository named `homebrew-tap`.

## What is here

| Formula | What it is |
|:-|:-|
| [`ytcli`](Formula/ytcli.rb) | [Yandex Tracker from the command line](https://github.com/ormeilu/yandex-tracker-cli), sized for agents |

## How it is maintained

`Formula/ytcli.rb` is **generated**, not written: the release workflow in
[ormeilu/yandex-tracker-cli](https://github.com/ormeilu/yandex-tracker-cli/blob/main/.github/workflows/publish.yml)
builds the release tarballs, hashes them, and pushes the formula here on every
tag. Editing it by hand works until the next release and no longer, so file
anything that needs changing against that repository instead.

The formula installs prebuilt binaries rather than building from source, and
takes its shell completions from the binary itself — a completion script cannot
go stale against a command tree it is generated from.
