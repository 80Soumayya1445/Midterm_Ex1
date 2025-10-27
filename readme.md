# Exercise 1 - GitHub Actions CI/CD

This project demonstrates a basic GitHub Actions workflow for continuous integration and continuous deployment (CI/CD). The workflow runs automated tests and builds on every push to the main branch and on pull requests.

## Project Description

A simple Node.js application with GitHub Actions CI/CD pipeline that:
- Runs tests on code changes
- Builds the application
- Ensures code quality through automated checks

## Features

- Automated testing on push and pull requests
- Node.js 18 environment
- Dependency installation and caching
- Build process execution

## GitHub Actions Workflow

The CI/CD pipeline is defined in `.github/workflows/ci.yml` and includes:

### Triggers
- Push to `main` branch
- Pull requests to `main` branch

### Jobs
- **test-and-build**: Runs on Ubuntu latest
  - Checks out code
  - Sets up Node.js 18
  - Installs dependencies with `npm ci`
  - Runs tests with `npm test`
  - Builds application with `npm run build`

## Prerequisites

- Node.js (version 18 or higher)
- npm


3. Run tests:
   ```bash
   npm test
   ```

4. Build the application:
   ```bash
   npm run build
   ```

## GitHub Actions Setup

The workflow file is located at `.github/workflows/ci.yml`. It will automatically run when:
- You push code to the `main` branch
- You create a pull request to the `main` branch

### Viewing Workflow Results

1. Go to your GitHub repository
2. Click on the "Actions" tab
3. Select the workflow run to see detailed logs


## Scripts

- `npm test`: Run the test suite
- `npm run build`: Build the application

## Contributing

1. Create a feature branch from `main`
2. Make your changes
3. Push your branch and create a pull request
4. The CI/CD pipeline will automatically run tests and build checks

