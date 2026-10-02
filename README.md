# Setup Kotlin Toolchain
Set up [Kotlin Toolchain](https://kotlin-toolchain.org) (formerly Amper) with caching for dependencies and provisioned JDKs.

> [!NOTE]
> This is a community-maintained GitHub Action, not affiliated with JetBrains.

![GitHub License](https://img.shields.io/github/license/RazerTexz/setup-kotlin-toolchain?style=for-the-badge)

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
