# Ankra Homebrew Tap

Homebrew formulae for [Ankra](https://ankra.io) tools.

## Install the Ankra CLI

```sh
brew install ankraio/tap/ankra
```

Or tap first, then install:

```sh
brew tap ankraio/tap
brew install ankra
```

## Upgrade

```sh
brew update && brew upgrade ankra
```

Note: a Homebrew-managed `ankra` refuses to self-update via `ankra upgrade`
and points you at `brew upgrade ankra` instead, so Homebrew stays the single
owner of the binary.

## How this tap is maintained

`Formula/ankra.rb` is regenerated automatically by the
[ankra-cli release workflow](https://github.com/ankraio/ankra-cli/blob/master/.github/workflows/release.yml)
on every stable release, from the template in
`packaging/homebrew/ankra.rb.tmpl`. The formula installs the prebuilt,
checksum-verified binaries published on
[GitHub releases](https://github.com/ankraio/ankra-cli/releases).

Do not edit the formula here by hand — change the template in
[ankraio/ankra-cli](https://github.com/ankraio/ankra-cli) instead.

## Support

- Issues: https://github.com/ankraio/ankra-cli/issues
- Documentation: https://docs.ankra.ai
