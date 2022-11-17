# playwright-notes
Notes on the Playwright test tool

https://playwright.dev/docs/intro

## Setup

```sh
npm init playwright@latest
.
Need to install the following packages:
  create-playwright@1.17.123
```

Choose JavaScript, e2e


Full output:

```txt
Getting started with writing end-to-end tests with Playwright:
Initializing project in '.'
✔ Do you want to use TypeScript or JavaScript? · JavaScript
✔ Where to put your end-to-end tests? · e2e
✔ Add a GitHub Actions workflow? (y/N) · true
✔ Install Playwright browsers (can be done manually via 'npx playwright install')? (Y/n) · true
Initializing NPM project (npm init -y)…
Wrote to /Users/user.name/git/playwright-notes/package.json:

{
  "name": "playwright-notes",
  "version": "1.0.0",
  "description": "Notes on the Playwright test tool",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "repository": {
    "type": "git",
    "url": "git+https://github.com/Qarj/playwright-notes.git"
  },
  "keywords": [],
  "author": "",
  "license": "ISC",
  "bugs": {
    "url": "https://github.com/Qarj/playwright-notes/issues"
  },
  "homepage": "https://github.com/Qarj/playwright-notes#readme"
}


Installing Playwright Test (npm install --save-dev @playwright/test)…

added 3 packages, and audited 4 packages in 2s

found 0 vulnerabilities
Downloading browsers (npx playwright install)…
Downloading Chromium 108.0.5359.29 (playwright build v1033) from https://playwright.azureedge.net/builds/chromium/1033/chromium-mac-arm64.zip
118 Mb [====================] 100% 0.0s
Chromium 108.0.5359.29 (playwright build v1033) downloaded to /Users/user.name/Library/Caches/ms-playwright/chromium-1033
Downloading FFMPEG playwright build v1008 from https://playwright.azureedge.net/builds/ffmpeg/1008/ffmpeg-mac-arm64.zip
1 Mb [====================] 100% 0.0s
FFMPEG playwright build v1008 downloaded to /Users/user.name/Library/Caches/ms-playwright/ffmpeg-1008
Downloading Firefox 106.0 (playwright build v1364) from https://playwright.azureedge.net/builds/firefox/1364/firefox-mac-11-arm64.zip
69.2 Mb [====================] 100% 0.0s
Firefox 106.0 (playwright build v1364) downloaded to /Users/user.name/Library/Caches/ms-playwright/firefox-1364
Downloading Webkit 16.4 (playwright build v1735) from https://playwright.azureedge.net/builds/webkit/1735/webkit-mac-12-arm64.zip
54.8 Mb [====================] 100% 0.0s
Webkit 16.4 (playwright build v1735) downloaded to /Users/user.name/Library/Caches/ms-playwright/webkit-1735
Writing playwright.config.js.
Writing .github/workflows/playwright.yml.
Writing e2e/example.spec.js.
Writing tests-examples/demo-todo-app.spec.js.
Writing package.json.
✔ Success! Created a Playwright Test project at /Users/user.name/git/playwright-notes

Inside that directory, you can run several commands:

  npx playwright test
    Runs the end-to-end tests.

  npx playwright test --project=chromium
    Runs the tests only on Desktop Chrome.

  npx playwright test example
    Runs the tests in a specific file.

  npx playwright test --debug
    Runs the tests in debug mode.

  npx playwright codegen
    Auto generate tests with Codegen.

We suggest that you begin by typing:

    npx playwright test

And check out the following files:
  - ./e2e/example.spec.js - Example end-to-end test
  - ./tests-examples/demo-todo-app.spec.js - Demo Todo App end-to-end tests
  - ./playwright.config.js - Playwright Test configuration

Visit https://playwright.dev/docs/intro for more information. ✨

Happy hacking! 🎭
```

## test

```sh
npx playwright test
npx playwright test example.spec.js
npx playwright test example.spec.js --project=chromium
npx playwright test example.spec.js --project=chromium --debug
```

## view report

```sh
npx playwright show-report
```