# GitHub Action cleanup disabled workflows

## Usage

```yml
on:
  workflow_dispatch:

permissions:
  actions: write

jobs:
  main:
    steps:
      - uses: mykiwi/cleanup-disabled-workflows@v1
```
