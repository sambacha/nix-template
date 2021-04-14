# [Nix](#) 

> Opinionated repository template

[![Nix: Coverage](https://github.com/sambacha/nix-template/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/sambacha/nix-template/actions/workflows/test.yml) [![niv auto update](https://github.com/sambacha/nix-template/actions/workflows/update-niv.yml/badge.svg?branch=master)](https://github.com/sambacha/nix-template/actions/workflows/update-niv.yml)

```bash
wget https://github.com/sambacha/nix-template/archive/master.zip
```

Based on [nix.dev](https://nix.dev) tutorials, repository template to get you started with [Nix](https://nixos.org/):

- [niv](https://github.com/nmattia/niv) for painless dependency management (aka pinning) with a daily cronjob to bump dependencies
- [gitignore.nix](https://github.com/hercules-ci/gitignore.nix) for respecting `.gitignore` when using your project as a source
- [pre-commit-hooks.nix](https://github.com/cachix/pre-commit-hooks.nix) for running linters (defaults to `shellcheck`, `nix-linter` and `nixpkgs-fmt`) when committing and on the CI
- [direnv](https://direnv.net/) for automatically loading your developer environment
- [GitHub Actions](https://github.com/features/actions) for CI with [dependabot](https://dependabot.com/) automatically bumping GitHub Actions versions

## Getting started

1. Follow tutorial for [creating a binary cache](https://nix.dev/tutorials/continuous-integration-github-actions.html)
2. Replace ``nix-getting-started-template`` in ``.github/workflows/test.yml`` with the name of your binary cache

## Using the project

Follow [direnv setup](https://nix.dev/tutorials/declarative-and-reproducible-developer-environments.html#direnv-automatically-activating-the-environment-on-directory-change) and run `direnv allow`
