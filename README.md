![ ](https://github.com/kelseyaubrecht/playwright-extension-testing-template/actions/workflows/test_playwright.yml/badge.svg)

# Playwright extension testing template

This project serves as a template for testing chrome extensions using Playwright.

## Contents

- [Getting started](#getting-started)
- [Run tests](#run-tests)
- [Useful links](#useful-links)
- [Example extension](#example-extension)
- [GitHub Action](github-action)

## Getting started

To set up the environment for the first time run:

- `yarn`
- `yarn playwright install chromium`

## Run tests

To execute all tests use:

- `yarn playwright test`

## Useful links

- [Playwright Extension Testing](https://playwright.dev/docs/chrome-extensions)
- [Playwright CLI](https://playwright.dev/docs/test-cli)
- [Playwright in VSCode](https://playwright.dev/docs/getting-started-vscode)

## Example extension

The project contains a rudimentary extension to demonstrate use in tests.

[Extension](extension) contents:

- index with title and current date
- script that loads current date
- background script to launch service worker (necessary to retrieve the extensionID via fixture)
- content script that adds a \<div>testDivText\</div> to any visited site

## GitHub Action

An [example workflow](.github/workflows/test_playwright.yml) to show running playwright tests with an extension in GitHub Actions.
The installs dependencies, runs the tests, and uploads the report.
