# starter-template

This repository provides a foundational setup for starting new projects with essential features like automated release workflows, code quality analysis with SonarCloud, dependency management with Dependabot, and a clear licensing structure.

## Table of Contents

- [starter-template](#starter-template)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Release Version Workflow](#release-version-workflow)
  - [SonarCloud](#sonarcloud)
  - [Dependabot](#dependabot)
  - [License](#license)

## Features

- **Automated Release Workflow**: Manage your releases effortlessly with GitHub Actions.
- **SonarCloud Integration**: Ensure code quality and maintainability with SonarCloud.
- **Dependabot**: Keep your dependencies up to date automatically.
- **Standard Licensing**: A default GPL-3.0 license included.

## Release Version Workflow

This repository uses GitHub Actions to automate the release process. The workflow must be manually triggered using the `workflow_dispatch` event. The workflow includes the following steps:

1. **Check out the code**.
2. **Set up Node.js**.
3. **Create a release**: Automatically tag and create a release based on the commit messages.

To customize the release workflow, modify the `.github/workflows/release.yml` file.

## SonarCloud

SonarCloud is used for static code analysis to ensure code quality. Script in this repository generate `.sonarcloud.properties` automatically.

## Dependabot

Dependabot helps you keep your dependencies up to date. It is configured to check for updates to your dependencies and open pull requests automatically. The configuration file is located at `.github/dependabot.yml`.

You can customize the update frequency, target dependencies, and more by modifying this file.

## License

This project is licensed under the GNU General Public License v3.0. See the [LICENSE](LICENSE) file for details.
