# Contributing Guidelines

Thank you for taking the time to contribute to GatorMiner! This guide will help you
to effectively get started and contribute to the project.

## Table of Contents

  - [Code of Conduct](#code-of-conduct)
  - [Raise an Issue](#raise-an-issue)
  - [Make a Pull Request](#make-a-pull-request)
  - [Project Overview](#project-overview)
    - [Development Environment](#development-environment)
    - [Contribute with Github Flow Model](#contribute-with-github-flow-model)
      - [Commits](#commits)
      - [Branches](#branches)
    - [Code Linting and Continuous Integration](#code-linting-and-continuous-integration)

## Code of Conduct

To build a diverse, respectful, and inclusive community, we ask that everyone
contributing to this project follow the [code of conduct](https://github.com/Allegheny-Ethical-CS/escape2020/blob/master/CODE_OF_CONDUCT.md) document.

## Raise an Issue

If you have a new issue to raise (bug report, feature request, etc.), go ahead
and raise it in the [Issue Tracker](https://github.com/Allegheny-Ethical-CS/escape2020/issues)
(the *Issues* tab on the top of the GitHub repository page)! Please follow the
provided issue template and try to fill out the template with
**as much detail as you can** when describing the raised issue.

## Make a Pull Request

The development team uses the [GitHub Flow Model](https://guides.github.com/introduction/flow/)
to guide our engineering of this tool. We invite you to also conform to the
Github model as you make a contribution. Once you have made some new changes and
would like the project maintainers to merge them into the project, we encourage
you to go ahead and open a [pull request](https://github.com/Allegheny-Ethical-CS/escape2020/pulls)
on the GitHub repository. Please follow the provided pull request template and
describe the new feature or bug fix that you are proposing with the necessary
information. The proposed change should not break the existing test cases and/or
features, as each PR will be checked with our Continuous Integration service
(code standard, test suites, etc.) We hope your proposed change is well-documented
and highly recommend you to provide tests along with the PR if you are making a
code contribution.

## Project Overview

### Development Environment

In order to contribute code or documentation to the project, the project
maintainers suggest installing the release of Python versions above 3.7. Information about installing Python can be found [here](https://www.python.org/downloads/).

If you want to use a virtual environment, you can learn more about installing and managing python versions with `pyenv` from [here](https://realpython.com/intro-to-pyenv/).

There are currently no external libraries, Python or otherwise, that the program needs to function.

### Contribute with Github Flow Model

If you are already a collaborator on the project and would like to contribute a
new feature or bug fix, you can do so by creating and publishing a branch off
from the `master` branch. If you are not yet a collaborator, we recommend you
either fork the repository or contact the project maintainers. We would grant you
access as a project contributor as soon as possible. You could then add your
new feature, document, or test it as appropriate.

You are welcome to open an issue first to describe what you want to do. If there
is an issue you would like to work on or if it matches with your PR, leave a
comment there instead and let us know what you plan to do.

#### Commits

A well-crafted git commit message is the best way to document and communicate
context about a change to fellow developers and their future selves. We encourage
you to write proper and descriptive commit messages, as they will become the
project's log and determine the maintainability of the project. Some of the
basic rules of writing a good commit message include:

- Capitalize the commit message.
- Do not end the commit message with a period.
- Use the imperative mood.
- Limit the commit message to within 50 characters.
- Describe why a change is being made.
- How does it address the issue?

#### Branches

You can create and publish a branch via the following commands. Substitute the
name of your branch for the `feature/feature-name`.

```bash
git checkout -b feature/feature-name
git checkout master
git push -u origin feature/feature-name
```

Using a consistent naming convention for branches improves the maintainability
of a project. We encourage you to follow the recommend rules listed below:

- Use hyphen and/or slash as separators: `prefix`/`branch`-`name`-`issue-id`.
- Use the types of the branch as prefixes to the branch name.
  - `feat`: implement or expand a feature.
  - `bug`: bug fix.
  - `doc`: documentation-related contribution.
  - `test`: test-related contribution.
  - `refact`: code refactoring.
  - `expr`: experiment.

### Code Linting and Continuous Integration

When making contributions to the project, please make sure that you adhere to the
coding standard that is enforced by automated linting tools such as
`Flake8` and `Pylint`. The project uses both Travis CI and Github Action to
build and test GatorMiner in Ubuntu and Mac operating systems with Python
versions of 3.6, 3.7, and 3.8. Following are some of the linting checks executed
in Travis CI and Github Action platform. You can also run these checks locally
to see if your changes have conformed to the coding standard.

```sh
pipenv run flake8 src
pipenv run pylint src
```
