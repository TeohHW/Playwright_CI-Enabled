# Playwright Test Automation Practice

This repository showcases my knowledge of Playwright test automation using TypeScript and Node.js.

It contains a collection of personal practice tests covering different Playwright scenarios, including UI automation, API validation, reusable locators, and test data handling.

## What This Repo Demonstrates

The test suite covers a range of Playwright testing concepts, including:

- UI interaction tests for forms, dropdowns, checkboxes, radio buttons, sliders, alerts, iFrames, tabs, and new windows
- E-commerce style flows such as product search, filtering, sorting, comparison, cart deletion, guest checkout, and purchase flow validation
- Contact form validation using both JSON and TypeScript test data
- Registration and login flow coverage
- API response validation and filtering scenarios
- Page locator reuse through a shared locator class
- Cross-browser execution using Chromium, Firefox, and WebKit
- Playwright configuration for timeouts, retries, traces, and HTML reporting

## Project Structure

```text
.
|-- tests/
|   `-- Practice/              # Active Playwright test specs
|-- pages/                     # Shared locator class / page object style helpers
|-- test-data/                 # JSON, TypeScript, and upload fixture test data
|-- hars/                      # HAR files and related network assets
|-- examples/                  # Optional reference material
|-- playwright.config.ts       # Playwright test configuration
|-- package.json
`-- README.md
```

The active test directory is configured in `playwright.config.ts`:

```ts
testDir: './tests'
```

## Test Areas

### Practice UI Scenarios

Located in `tests/Practice/Practice.spec.ts`.

These tests cover common UI automation skills such as:

- Radio buttons
- Suggestion boxes
- Dropdowns
- Checkboxes
- Browser tabs and windows
- Hide/show elements
- Alerts and confirmations
- Web tables
- Mouse hover interactions
- iFrames

### Additional Practice Scenarios

Located in `tests/Practice/PracticeB.spec.ts`.

These tests cover:

- Registration page validation
- Slow loading page handling
- JavaScript alerts

### Shopping And E-Commerce Scenarios

Located in `tests/Practice/ShoppingPage.spec.ts`.

These tests cover more complete user journeys, including:

- Product selection
- Search
- Price slider interaction
- Checkbox filters
- Pagination
- Sorting
- Category navigation
- Contact form validation
- File upload
- Product comparison
- User registration
- Cart item deletion
- Guest checkout and payment flow

### API Scenarios

Located in `tests/Practice/API Test.spec.ts`.

These tests cover API-style validation such as:

- Listing resources
- Reading a specific resource
- Filtering resources
- Validating nested resource responses

## Getting Started

Install dependencies:

```bash
npm install
```

Install Playwright browsers if needed:

```bash
npx playwright install
```

List available tests:

```bash
npx playwright test --list
```

Run the full test suite:

```bash
npx playwright test
```

Run tests in the Playwright UI:

```bash
npx playwright test --ui
```

Open the HTML report after a run:

```bash
npx playwright show-report
```

## Notes

This project is focused on practicing Playwright automation rather than testing a single owned application. The tests intentionally cover different websites and interaction patterns to build experience across UI automation, API validation, reusable locators, test data handling, and Playwright configuration.
