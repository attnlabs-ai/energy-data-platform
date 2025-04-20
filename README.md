# energy-data-platform
SaaS energy-data platform for real-time CCUS, DER, and methane-emissions signals.

## Overview

This repository contains the codebase for a SaaS energy-data platform that provides real-time insights into CCUS, DER, and methane emissions. It is built with a focus on modern, latency-aware user experience and open APIs.

## Prerequisites

- Node.js (version 14 or higher)
- npm (Node Package Manager)
- AWS account with necessary permissions
- Docker (for running containers)

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/attnlabs-ai/energy-data-platform.git
   cd energy-data-platform
   ```
2. Install dependencies for each component:
   ```sh
   cd infra && npm install
   cd ../data-eng && npm install
   cd ../backend && npm install
   cd ../frontend && npm install
   ```

## Running the Application

1. Set up infrastructure using Terraform:
   ```sh
   cd infra
   terraform init
   terraform apply
   ```
2. Start the data ingestion process:
   ```sh
   cd ../data-eng
   npm run start
   ```
3. Start the backend services:
   ```sh
   cd ../backend
   npm run start
   ```
4. Start the frontend application:
   ```sh
   cd ../frontend
   npm run dev
   ```

## Contribution Guidelines

- Fork the repository and create a new branch for your feature or bug fix.
- Ensure code quality by running linting and tests before committing.
- Submit a pull request with a detailed description of your changes.
- Follow the project's coding standards and guidelines.

## License

This project is licensed under the MIT License.
