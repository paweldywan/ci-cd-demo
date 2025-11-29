# CI/CD Demo

A simple Node.js demonstration project showcasing continuous integration and continuous deployment using Azure Pipelines.

## Description

This repository contains a minimal Node.js application designed to demonstrate CI/CD pipeline concepts with Azure DevOps. The application outputs a simple message to the console and includes an automated pipeline configuration.

## Features

- Simple Node.js console application
- Azure Pipelines configuration for automated CI/CD
- Automated testing on every commit to the main branch

## Project Structure

```
ci-cd-demo/
├── azure-pipelines.yml    # Azure Pipelines CI/CD configuration
├── index.js               # Main application file
├── package.json           # Node.js project configuration
└── README.md              # Project documentation
```

## Prerequisites

- Node.js (version 12 or higher)
- npm (Node Package Manager)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/paweldywan/ci-cd-demo.git
   cd ci-cd-demo
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

## Usage

Run the application:
```bash
node index.js
```

Expected output:
```
Hello, CI/CD Pipeline!
```

## Testing

Run the test suite:
```bash
npm test
```

## CI/CD Pipeline

This project uses Azure Pipelines for continuous integration and deployment. The pipeline is configured to:

- Trigger on commits to the `main` branch
- Run on an Ubuntu-latest virtual machine
- Install project dependencies
- Execute the test suite

### Pipeline Configuration

The pipeline is defined in `azure-pipelines.yml` and automatically runs when changes are pushed to the main branch.

## License

ISC

## Author

Created as a demonstration project for CI/CD concepts.
