# Coded Clique

[![GitHub CI](https://github.com/tlylt/coded-clique/actions/workflows/test.yml/badge.svg)](https://github.com/tlylt/coded-clique/actions/workflows/test.yml)

This action provides the following functionality for GitHub Actions users:

- Encode your issue content

# Usage

You may use the action without any additional parameters.

```yaml
steps:
- uses: tlylt/coded-clique@v1
```

# Testing

```yaml
name: Test coded-clique

on:
  issues:
    types: [opened, edited]
  issue_comment:
    types: [created, edited]

jobs:
  build:
    runs-on: ubuntu-latest
    name: Coded Clique test
    steps:
      - uses: tlylt/coded-clique@main
```

# Development

Updates will be done on the main branch. When ready, tag and release according to semver.

# License

The scripts and documentation in this project are released under the [MIT License](LICENSE)
