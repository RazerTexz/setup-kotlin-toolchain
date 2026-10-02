# Setup Kotlin Toolchain
Setup [Kotlin Toolchain](https://kotlin-toolchain.org/latest/) with caching.

> [!NOTE]
> This is a community-maintained GitHub Action, not affiliated with JetBrains.

## Usage
```yaml
name: Build
on: [push, pull_request, workflow_dispatch]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v7

      - name: Setup Kotlin Toolchain
        uses: RazerTexz/setup-kotlin-toolchain@v1

      - name: Build
        run: kotlin build
```
