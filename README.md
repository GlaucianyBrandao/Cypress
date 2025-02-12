# 🛒 **Cypress Test Automation - nopCommerce Demo**

This project contains test automation for the **nopCommerce Demo** e-commerce site using **Cypress**. The goal is to ensure that essential functionalities such as login, registration, shopping cart, and checkout are working correctly.

## 🚀 **Technologies Used**

- **Cypress**: End-to-end testing automation tool.
- **Node.js**: Environment to run the tests.
- **JavaScript**: Language used for test automation.

## 🛠 **Prerequisites**

To run this project, the following must be installed:

- **Node.js** (version 14 or above)
- **Cypress** (installed automatically via npm)

## 📦 **Installation**

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/cypress-automation-nopcommerce.git
   cd cypress-automation-nopcommerce
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Open Cypress**:
   After installing dependencies, open Cypress to run the tests:
   ```bash
   npx cypress open
   ```

4. **Run the tests**:
   In Cypress, you can run the tests by clicking on the available options in the interface, or run directly in the terminal:
   ```bash
   npx cypress run
   ```

## 🧪 **Automated Test Cases**

### 1. **Login**

- Test login with valid credentials.
- Test login with invalid credentials.

### 2. **Shopping Cart and Checkout**

- Add product to cart.
- Complete checkout successfully.

### 3. **User Registration**

- Register a new user in the system.

## 📝 **Project Structure**

```bash
├── cypress/
│   ├── e2e/
│   │   ├── login.cy.js      # Login tests
│   │   ├── cart_checkout.cy.js # Cart and checkout tests
├── cypress.json             # Cypress configurations
├── package.json             # Project dependencies
├── README.md                # This file
└── node_modules/            # Installed dependencies
```

## ⚙️ **Cypress Configurations**

Cypress configurations can be found in the `cypress.json` file. This file contains the test environment settings, such as the base URL of the site to be tested.

### Example `cypress.json`:
```json
{
  "baseUrl": "https://demo.nopcommerce.com"
}
```

## 🔧 **Running Tests in CI/CD**

You can integrate this project with **GitHub Actions** or other CI/CD tools to run tests automatically whenever there are changes in the code.

Example configuration for **GitHub Actions**:
```yaml
name: Run Cypress Tests

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main

jobs:
  cypress-run:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v2
      - name: Set up Node.js
        uses: actions/setup-node@v2
        with:
          node-version: '14'
      - name: Install dependencies
        run: npm install
      - name: Run Cypress tests
        run: npx cypress run
```

## 📢 **Contributions**

Contributions are welcome! If you'd like to improve the project, follow these steps:

1. Fork this repository.
2. Create a branch for your feature (`git checkout -b feature/new-feature`).
3. Commit your changes (`git commit -am 'Add new feature'`).
4. Push to the remote repository (`git push origin feature/new-feature`).
5. Open a Pull Request.



