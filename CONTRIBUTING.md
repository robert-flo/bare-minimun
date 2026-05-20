# Contributing to BARE-MINIMUN

Thank you for your interest in contributing to BARE-MINIMUN! We welcome any contributions, including bug fixes, feature enhancements, documentation improvements, and other general improvements.

---

## Getting Started

1. Fork this repository to your GitHub account. This will create a copy of this repository in your account. You can make changes to this copy without affecting the original repository.
   - To fork this repository, click the **Fork** button in the top right corner of this page or use the [GitHub fork repository option](https://github.com/robert-flo/bare-minimun/fork).

   > [!NOTE]
   > **For first-time contributors:** All new contributors should start by submitting pull requests. Direct repository write access is granted selectively based on contribution history.

2. Clone your forked repository to your local machine.
   - Use the following command to clone your forked repository:

     ```bash
     git clone https://github.com/robert-flo/bare-minimun.git
     ```

3. Create a new branch for your changes.
   - For example, to create a new branch named `your-branch-name`, use:

     ```bash
     git checkout -b your-branch-name
     ```

4. Make your changes and commit them with a descriptive commit message.
   - Make sure to follow our [commit message guidelines](https://github.com/robert-flo/bare-minimun/blob/master/COMMIT_MESSAGE_GUIDELINES.md):

     ```bash
     git commit -m "feat: ✨ Add a new feature"
     ```

5. Code should be documented where appropriate.
   - Changes compared to the latest BARE-MINIMUN release which have a direct effect on the user (as opposed to code refactoring or documentation/tests) also need to be documented in `CHANGELOG.md`.
   - The existing entries should be used as a style guideline.
   - The changelog should document changes from a user perspective instead of explaining technical background. More information can be found on the [Keep a Changelog website](https://keepachangelog.com/).

6. Push your changes to your forked repository.
   - To push your changes to your fork, use:

     ```bash
     git push origin your-branch-name
     ```

7. Submit a **pull request** to the upstream repository.
   - **Important:** Always submit your pull requests to the `dev` branch, **not** directly to `master`. Following our [RELEASE_POLICY.md](https://github.com/robert-flo/bare-minimun/blob/master/RELEASE_POLICY.md), changes go through the `dev` branch first for testing before being merged into `master` during release windows.
   - To create a pull request, use the following steps:
     1. Go to your forked repository.
     2. Click the **Compare & pull request** button next to your `your-branch-name` branch.
     3. Make sure the base repository branch is set to `dev`.
     4. Run pre-commit checks locally using `pre-commit run --all-files`.
     5. Add a title and description for your pull request.
     6. Click **Create pull request** and remember to fill out the [pull request template](https://github.com/robert-flo/bare-minimun/blob/master/.github/PULL_REQUEST_TEMPLATE.md).

---

## Guidelines

- Follow the code style of the project.
- Update the **documentation** if necessary.
- Add tests if applicable.
- Make sure all tests pass before submitting your changes.
- Keep your pull request focused and avoid including unrelated changes.
- Refer to the following files for templates and guidance:
  - [bug_report.yml](https://github.com/robert-flo/bare-minimun/blob/master/.github/ISSUE_TEMPLATE/bug_report.yml) - Use this template to report bugs and issues.
  - [feature_request.yml](https://github.com/robert-flo/bare-minimun/blob/master/.github/ISSUE_TEMPLATE/feature_request.yml) - Use this template to suggest new features.
  - [documentation_update.yml](https://github.com/robert-flo/bare-minimun/blob/master/.github/ISSUE_TEMPLATE/documentation_update.yml) - Use this template to propose doc updates.
  - [custom.yml](https://github.com/robert-flo/bare-minimun/blob/master/.github/ISSUE_TEMPLATE/custom.yml) - Use this template for other custom issues.
  - [PULL_REQUEST_TEMPLATE.md](https://github.com/robert-flo/bare-minimun/blob/master/.github/PULL_REQUEST_TEMPLATE.md) - Use this template when submitting a pull request.
  - [COMMIT_MESSAGE_GUIDELINES.md](https://github.com/robert-flo/bare-minimun/blob/master/COMMIT_MESSAGE_GUIDELINES.md) - Read this to learn about commit formats.
  - [RELEASE_POLICY.md](https://github.com/robert-flo/bare-minimun/blob/master/RELEASE_POLICY.md) - Read this to understand the release and branch cycles.
  - [LICENSE](https://github.com/robert-flo/bare-minimun/blob/master/LICENSE) - Read this file to check the project's license.
  - [README.md](https://github.com/robert-flo/bare-minimun/blob/master/README.md) - Read this file to understand the general project layout.

---

## Contact

If you have any questions, feel free to contact us via [GitHub Discussions](https://github.com/robert-flo/bare-minimun/discussions).
