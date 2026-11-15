name: Update GitAscii

on:
  workflow_dispatch:

permissions:
  contents: write

concurrency:
  group: gitascii-publication
  cancel-in-progress: true

jobs:
  publish:
    runs-on: ubuntu-latest
    timeout-minutes: 5
    steps:
      - name: Generate and Publish GitAscii SVGs
        uses: Igorcbraz/GitAscii/action@main
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/islammersal2/islammersal2/gitascii/profiles/default/dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/islammersal2/islammersal2/gitascii/profiles/default/light.svg">
  <img alt="GitAscii Profile" src="https://raw.githubusercontent.com/islammersal2/islammersal2/gitascii/profiles/default/dark.svg" width="100%">
</picture>
