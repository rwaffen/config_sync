# config_sync

[![License](https://img.shields.io/github/license/rwaffen/config_sync.svg)](https://github.com/rwaffen/config_sync/blob/main/LICENSE)

## How to use config_sync.rb

config_sync.rb syncs `config_sync/**/*` into `.github` for defined repositories.
It commits, pushes and creates a pull request for the changes.

The repositories are defined in [`config_sync.yml`](config_sync.yml)

```shell
bundle config set --local path 'vendor/bundle'
bundle install
export GITHUB_TOKEN='your_token_here'
bundle exec ruby config_sync.rb
```
