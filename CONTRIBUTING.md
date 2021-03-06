# Contributing to Smart Units Converter

:+1::tada: First off, thanks for taking the time to contribute! :tada::+1:

The following is a set of guidelines for contributing to Smart Units Converter, which are hosted in the [Smart Units Converter](https://github.com/se20z09/units_converter_extension) on GitHub. These are mostly guidelines, not rules. Use your best judgment, and feel free to propose changes to this document in a pull request.

#### Table Of Contents

[Code of Conduct](#code-of-conduct)

[How Can I Contribute?](#how-can-i-contribute)

-   [Add a New Conversion](#add-a-new-conversion)
-   [Reporting Bugs](#reporting-bugs)
-   [Pull Requests](#pull-requests)

[Styleguides](#styleguides)

-   [Git Commit Messages](#git-commit-messages)

[Documentation](#documentation)

-   [JSDoc](#jsdoc)

## Code of Conduct

This project and everyone participating in it is governed by the [code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to [bjdemick@ncsu.edu](mailto:bjdemick@ncsu.edu).

## What should I know before I get started?

This is a test repository, but feel free to file an issue if you still need to.

## How Can I Contribute?

### Add a New Conversion

Adding a new conversion is straightforward:

1. Create a new conversion source file that handles the conversion, appropriately named, in [`code/conversions/`](code/conversions)
2. Update [`main_scripts/popular_units.js`](main_scripts/popular_units.js) to add the conversion to the map
3. Update [`main/scripts/units_objects.js`](main_scripts/units_objects.js) to add the conversion descriptions
4. Update [`main/scripts/utility.js: get_conversion_class'](main/scripts/utllity.js) to add a case for the new conversion
5. Create a unit test under [`test/`](test) with the name of the conversion and the suffix `.test.js`, ensure that your unit test sufficiently covers the main conversion code

### Reporting Bugs

This section guides you through submitting a bug report for Smart Units Converter. Following these guidelines helps maintainers and the community understand your report, reproduce the behavior, and find related reports.

Before creating bug reports, please check if that bug is already reported as you might find out that you don't need to create one. When you are creating a bug report, please [include as many details as possible](#how-do-i-submit-a-good-bug-report).

> **Note:** If you find a **Closed** issue that seems like it is the same thing that you're experiencing, open a new issue and include a link to the original issue in the body of your new one.

#### How Do I Submit A (Good) Bug Report?

Bugs are tracked as [GitHub issues](https://guides.github.com/features/issues/). Create an issue on the repository and provide as much information as you can provide, like OS details, expected behaviour, etc.

Explain the problem and include additional details to help maintainers reproduce the problem:

-   **Use a clear and descriptive title** for the issue to identify the problem.
-   **Describe the exact steps which reproduce the problem** in as many details as possible.
-   **Provide specific examples to demonstrate the steps**. Include links to files or GitHub projects, or copy/pasteable snippets, which you use in those examples. If you're providing snippets in the issue, use [Markdown code blocks](https://help.github.com/articles/markdown-basics/#multiple-lines).
-   **Describe the behavior you observed after following the steps** and point out what exactly is the problem with that behavior.
-   **Explain which behavior you expected to see instead and why.**

Include details about your configuration and environment:

-   **What's the name and version of the OS you're using**?

## Git Remote Workflow

When adding a new feature to the project, work should be completed in a branch separate from the main repository, with a name that roughly indicates what its purpose is.
To create a new branch on your local machine, run:

`git checkout -b <branch_name>`

You can then make changes in your branch. When you are ready to add this branch to the remote, run:

`git push -u origin <branch_name>`

You will only need to run this command the first time you want to commit your local changes to the remote branch.
After the first commit, a simple `git push` from your repository root will push committed changes to the remote repository.

### Pull Requests

The process described here has several goals:

-   Maintain Smart Units Converter's quality
-   Priritize issues that are important to users
-   Engage the community in working toward the best possible Smart Units Converter
-   Enable a sustainable system for Smart Units Converter's maintainers to review contributions

Please follow these steps to have your contribution considered by the maintainers:

1. Follow the [styleguides](#styleguides)
2. After you submit your pull request, verify that all [status checks](https://help.github.com/articles/about-status-checks/) are passing <details><summary>What if the status checks are failing?</summary>If a status check is failing, and you believe that the failure is unrelated to your change, please leave a comment on the pull request explaining why you believe the failure is unrelated. A maintainer will re-run the status check for you. If we conclude that the failure was a false positive, then we will open an issue to track that problem with our status check suite.</details>

While the prerequisites above must be satisfied prior to having your pull request reviewed, the reviewer(s) may ask you to complete additional design work, tests, or other changes before your pull request can be ultimately accepted.

## Styleguides

### Git Commit Messages

-   Use the present tense ("Add feature" not "Added feature")
-   Use the imperative mood ("Move cursor to..." not "Moves cursor to...")
-   Limit the first line to 72 characters or less
-   Reference issues and pull requests liberally after the first line
-   When only changing documentation, include `[ci skip]` in the commit title

### Code Formatter

-   [Visual Studio Code](https://code.visualstudio.com/) IDE
-   [Prettier Formatter for Visual Studio Code](https://github.com/prettier/prettier-vscode/blob/main/README.md)

*   Prettier is an opinionated code formatter. It enforces a consistent style by parsing your code and re-printing it with its own rules that take the maximum line length into account, wrapping code when necessary.

#### Installation

-   Install through VS Code extensions. Search for Prettier - Code formatter
-   It can also be installed in VS Code: Launch VS Code Quick Open (Ctrl+P), paste the following command, and press enter.
    `ext install esbenp.prettier-vscode`
-   To install prettier in your project and pin its version:
    `npm install prettier -D --save-exact`

#### Format On Save

-   Moreover, you choose editor.formatOnSave setting to automatimally let Visual Studio Code IDE format the code on saving modifcations.

## Attribution

-   These contribution instructions were adapted from [Atom's Contributing.md](https://github.com/atom/atom/blob/master/CONTRIBUTING.md)

## Code Style Checker and Analyzer

### eslint

<b>Installation</b>

-   `npm install eslint --global` in comand line interface to install globally
-   `npm install eslint --save-dev` in command line interface to install locally

<b>Running eslint</b>

-   Once installed, eslint will automatically check your syntax as you type
-   Syntax violations will be flagged with red underlines and proposed fixes will be available on hover
-   Our config file automatically integrates eslint with Prettier to avoid conflicts

## Documentation

### JSDoc

<b>Installation</b>

-   `npm init -y` to create/update a package.json file
-   `npm i -D jsdoc` to install as a dev dependency JSDoc

<b>Running JSDoc </b>

-   update jsdoc.json config file with relevant file locations for source and destination
-   add the doc location under scripts in package.json as `jsdoc -c jsdoc.json`
-   after making any changes in the javascript files under code directory use `npm run doc` command to update the html file in docs directory
