# GitHub Actions: cleanup disabled workflows

## Usage

```yml
on:
  workflow_dispatch:

permissions:
  actions: write

jobs:
  main:
    runs-on: ubuntu-latest
    steps:
      - uses: mykiwi/cleanup-disabled-workflows@v1
        with:
          # Custom GitHub Token, to not be rate limited to 1,000 requests
          # Default: ${{ github.token }}
          github-token: ''

          # Show which workflows would be deleted (without actually deleting them)
          # default: false
          summarize: ''
```
