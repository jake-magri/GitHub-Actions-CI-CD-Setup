# Continuous Integration and Deployment with GitHub Actions
![License](https://img.shields.io/badge/MIT%20License-purple)

## Description

This project demonstrates the implementation of a robust Continuous Integration (CI) and Continuous Deployment (CD) pipeline using GitHub Actions. The pipeline is designed to automate testing with Cypress upon Pull Requests to the develop branch and deploy the application automatically to Render upon merging develop into main. This setup ensures streamlined development processes, consistent code quality, and efficient deployment of new features to production.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [How to Contribute](#how-to-contribute)
- [Tests](#tests)
- [License](#license)
- [Questions](#questions)

## Installation

1. Clone the repository from GitHub.
    ```
    git clone <https://github.com/jake-magri/GitHub-Actions-CI-CD-Setup>
    ```

2. Navigate to the project directory:
    ```
    cd <project-directory>
    ```

3. Install dependencies using your package manager (e.g., npm):
    ```
    npm install
    ```

4. Configure your Render deployment:
    1. Turn off auto-deploy on Render.
    2. Obtain the deploy hook URL and API key.
    3. Add the deploy hook URL and API key to GitHub Secrets.

5. Create develop and feature branches:
    ```
    git checkout -b develop
    ```

## Usage

### Screenshots

#### Continuous Deployment to Production Successful
![Continuous Deployment Successful](https://github.com/user-attachments/assets/0e86937d-0a46-42e4-b86c-e3c587e8808b)

#### Continuous Deployment Jobs Passed
![Continuous Deployment Tests Passed](https://github.com/user-attachments/assets/0f5e7628-20a6-44ce-a69e-c3678eb416f3)

#### Continuous Integration Component Tests Passed
![Continuous Integration Component Tests Passed](https://github.com/user-attachments/assets/f4c22687-59a8-4384-b5db-23d702721d51)


### Usage Information
1. Developers should work on feature branches and submit Pull Requests to the develop branch for review.
2. Upon submitting a Pull Request, GitHub Actions will automatically trigger Cypress tests to validate code quality and ensure no regressions.
3. After successful testing and approval, merge the develop branch into main. This action will trigger an automatic deployment to Render.
4. Monitor GitHub Actions workflows for detailed logs on test results and deployment status.

## How to Contribute
1. Create a new feature branch for your work.
2. Ensure all changes are tested locally using Cypress before submitting a Pull Request.
3. Adhere to the repository's code style and naming conventions.
4. Provide meaningful commit messages and detailed descriptions in Pull Requests.
5. All contributions must pass CI tests and be reviewed before merging.

## Tests

1. Run tests locally before pushing code:
    ```
    npm run cypress:open
    ```

2. Submit a Pull Request to the develop branch to trigger automated testing via GitHub Actions.
3. Review test results on the GitHub Actions page.
4. Ensure that all Cypress component tests pass.

## License 
This application is covered under MIT License.
See the [full license](https://opensource.org/licenses/MIT) for more information.

## Questions
To reach me with additional questions please message me on either GitHub at jake-magri or via email jake.magri2@gmail.com.
