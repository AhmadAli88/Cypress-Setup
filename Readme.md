
# Cypress Installation and Usage Guide

This guide explains how to install Cypress in your project and run tests effectively.

## Installation

### Step 1: Install Cypress
Run the following command in your project directory to install Cypress as a development dependency:
```bash
npm install cypress --save-dev
```

### Step 2: Open Cypress
To open Cypress, use the command:
```bash
npx cypress open
```

This will launch the Cypress Test Runner, where you can configure and run tests.

### Step 3: Initialize Cypress
Cypress will automatically create a `cypress` folder in your project, including:
- **`cypress/e2e/`**: Store your test files here.
- **`cypress/fixtures/`**: Use for sample data or mock responses.
- **`cypress/support/`**: Utility functions and shared configurations.

If this folder isn't generated, initialize it manually by running:
```bash
npx cypress init
```

### Step 4: Run Tests
To run tests in a headless browser, use:
```bash
npx cypress run
```

### Step 5: Add Scripts (Optional)
Add the following scripts to your `package.json` for easier access:
```json
"scripts": {
  "cypress:open": "cypress open",
  "cypress:run": "cypress run"
}
```

Then use these commands:
```bash
npm run cypress:open
npm run cypress:run
```

## Additional Notes
- **Avoid Global Installation**: Cypress works best as a project-specific dependency.
- **System Requirements**: Ensure Node.js (>=12.0.0) is installed.
- **Configuration**: Customize Cypress by editing the `cypress.config.js` file.

## Learn More
Visit the [Cypress Documentation](https://docs.cypress.io) for more details.
