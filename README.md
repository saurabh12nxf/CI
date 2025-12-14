# GSH Node.js App with CI/CD

A simple Node.js application demonstrating unit testing and CI/CD pipeline setup.

## Features
- Simple utility functions
- Unit tests using Jest
- Automated CI pipeline using GitHub Actions

## Getting Started

### Prerequisites
- Node.js (v18 or higher)
- npm

### Installation
```bash
npm install
```

### Running Tests
```bash
npm test
```

## CI/CD Pipeline

The project includes a GitHub Actions workflow that:
- Triggers on Pull Requests to `main` or `master` branches
- Triggers on pushes to `main` or `master` branches
- Tests on Node.js versions 18.x and 20.x
- Installs dependencies and runs all unit tests
- **Fails the pipeline if any test fails**

### How to Use the Pipeline
1. Push this code to a GitHub repository
2. Create a Pull Request
3. The CI pipeline will automatically run
4. If all tests pass, the PR can be merged
5. If any test fails, the pipeline will fail and block the merge

## Project Structure
```
GSH/
├── .github/
│   └── workflows/
│       └── ci.yml          # CI pipeline configuration
├── sum.js                  # Application code
├── sum.test.js             # Unit tests
├── package.json            # Project configuration
└── README.md               # This file
```
