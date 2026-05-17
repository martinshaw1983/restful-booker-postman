# Restful Booker API Test Automation Suite

This repository contains an automated API test suite for the public Restful Booker platform. The tests validate the happy path core functionality of the booking workflow, including authentication, creation, searching, updates, and deletion.

The suite is built using Postman for local development and uses Newman to run automatically in a continuous integration (CI) pipeline via GitHub Actions.

## Project Structure

* `Restful_Booker_Happy_Path.postman_collection.json` — The complete Postman collection containing the requests and JavaScript validation scripts.
* `Restful_Booker.postman_environment.json` — The environment variables configuration managing dynamic tokens and booking IDs.
* `.github/workflows/postman-tests.yml` — The GitHub Actions automation workflow.

## Getting Started

### Local Execution via Postman
1. Clone this repository to your machine.
2. Open Postman desktop.
3. Click **Import** and select the collection and environment JSON files.
4. Ensure the `Restful Booker` environment is selected in the top-right dropdown.
5. Right-click the collection folder and select **Run Collection**.

### Command Line Execution via Newman
If you prefer running tests from your terminal, you can use Newman directly:

1. Install Newman globally if you have Node.js installed:
   ```bash
   npm install -g newman