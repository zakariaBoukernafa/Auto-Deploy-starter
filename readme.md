# Auto-Deploy-starter

Auto-Deploy-starter is a tool that allows you to automate the deployment process of your application using deployment strategies and continuous delivery processes. It integrates with CircleCI and uses ansible as a configuration management tool to deploy your code to cloud-based servers on AWS. The tool also includes centralized structured logging with Prometheus to surface critical server errors for diagnosis.

To configure Auto-Deploy-starter, connect your Git repository to the CircleCI dashboard and add the necessary environment variables, including `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY`, based on the `./circleci/ansible/deploy-backend.yml` and `./circleci/ansible/configure-server.yml` files. The build and deploy commands will be automatic.

## Installation

To install Auto-Deploy-starter, follow these steps:

1.  Clone the repository: `git clone https://github.com/zakariaBoukernafa/Auto-Deploy-starter.git`
2.  Navigate to the directory: `cd Auto-Deploy-starter`

## Usage

To use Auto-Deploy-starter, follow these steps:

1.  Connect your Git repository to the CircleCI dashboard.
2.  Add the necessary environment variables, including `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY`, based on the `./circleci/ansible/deploy-backend.yml` and `./circleci/ansible/configure-server.yml` files.
3.  Push your code to your repository. The deployment will automatically be triggered by CircleCI using the configurations specified in the `./circleci/config.yml` file.

The deployment script will automatically build and deploy your application using deployment strategies and continuous delivery processes with CircleCI and ansible. Prometheus monitoring and centralized structured logging will also be set up to ensure the success of the deployment and surface critical errors.

## Configuration

Auto-Deploy-starter can be further configured by modifying the `config.json` file. The following option is available:

- `branch`: The branch that you want to deploy.

## Contributions

Contributions are welcome! If you have any ideas for improvement or have found a bug, please open an issue or create a pull request.
