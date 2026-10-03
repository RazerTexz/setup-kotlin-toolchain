# Setup Kotlin Toolchain
![Tests](https://img.shields.io/github/actions/workflow/status/RazerTexz/setup-kotlin-toolchain/test.yaml?style=for-the-badge&label=Tests)
![License](https://img.shields.io/github/license/RazerTexz/setup-kotlin-toolchain?style=for-the-badge)

Set up [Kotlin Toolchain](https://kotlin-toolchain.org) (formerly Amper) with cross-platform caching for the Kotlin Toolchain, JDKs, and dependencies.

> [!NOTE]
> This is a community-maintained GitHub Action, not affiliated with JetBrains.

## Usage
```yaml
name: Build
on: [push, pull_request]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout
        uses: actions/checkout@v7

      - name: Set up Kotlin Toolchain
        uses: RazerTexz/setup-kotlin-toolchain@v1

      - name: Build
        run: kotlin build
```
