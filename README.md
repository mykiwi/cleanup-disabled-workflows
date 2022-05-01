# GitHub Action cleanup disabled workflows

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
```
