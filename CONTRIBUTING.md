# 🤝 Contributing Guidelines

Thank you for your interest in gatsby-plugin-component-to-image! This document outlines the guidelines for contributing to this project, including the development workflow and style guide.

## Reporting Issues

Not a coder? See the [support resources](https://github.com/twocaretcat/.github/blob/main/docs/SUPPORT.md) for information on how to:

- request features
- report bugs
- ask questions
- report security vulnerabilities

## Finding Issues to Work On

Issues with the `🚦 ready` label are ready to be worked on. If you comment on an issue, I can assign it to you.

Issues with the `🚦 needs triage` label generally need some more information before they can be worked on, but if you
**start a discussion** about it or leave a comment on the issue, I can likely get it ready for you.

If an issue is unclear or you have any questions about how a feature should be implemented, reach out before making any
changes so we can discuss the best way to do it.

## Guidelines

This project follows [semantic versioning] to better communicate the impact of changes to users.

## Style Guide

[Biome.js] is used to enforce a consistent code style across the project. You can format the code by running `pnpm biome format` or lint the code by running `pnpm biome lint`, but the easiest way to ensure that your code is properly formatted is to install a [Biome.js plugin for your code editor].

##  Development Workflow

### Prerequisites

To contribute to this project, you will need to have the following tools installed on your machine:
- [Node.js] 20.0.0+
- [Git]
- [Pnpm]

### Installation

After installing the prerequisites and cloning the repository, you can install the project dependencies by running `pnpm install`.

### Building

This project is built using [TypeScript]. Running `pnpm build` will compile source code in the `src/` directory and output the compiled JavaScript files to the `lib/` directory, along with type definitions.

When developing locally, keep in mind that the project will not automatically recompile when changes are made to the source code. You can run `pnpm watch` to automatically recompile the project when you save changes to a file.

### Testing

While developing, you can run `pnpm test` to run the test suite. This will also generate a coverage report in the `coverage/` directory.

Tests are run on the source `.ts` files, so there is no need to build the project before running tests.

Please ensure that all tests pass and that the coverage does not decrease before opening a pull request.

### Cleaning

If you need to clean the project directory, you can run `pnpm clean` to remove the `dist/` directory and any other generated files.

### Publishing (Maintainers Only)

To create a new release:
1. Update the version number in `package.json` according to the [semantic versioning] guidelines.
2. Run `pnpm pack` to create a tarball of the project.
3. Create a new release on GitHub and upload the tarball as an asset. This will trigger the publish workflow, which will automatically publish the package to npm.

## License

By contributing to this project, you agree that your contributions will be licensed under the project license.

[Biome.js plugin for your code editor]: https://biomejs.dev/guides/integrate-in-editor/
[Biome.js]: https://biomejs.dev/
[Git]: https://git-scm.com/
[Node.js]: https://nodejs.org/
[open an issue]: https://github.com/twocaretcat/gatsby-plugin-component-to-image/issues
[Pnpm]: https://pnpm.io/
[semantic versioning]: https://semver.org/
[TypeScript]: https://www.typescriptlang.org/
