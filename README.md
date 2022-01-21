# 🍿 Popcornx

A simple personal project to keep track of favorite movies, series, books and comic-books.

[![MIT license](https://img.shields.io/badge/License-MIT-brightgreen.svg)](LICENSE)
[![Editor Config](https://img.shields.io/badge/Editor%20Config-1.0.1-crimson.svg)][2]
[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)][5]
[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat-square)][5]
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)][8]
[![eslint](https://img.shields.io/badge/code%20style-eslint-green)][26]
[![prettier](https://img.shields.io/badge/code%20style-prettier-ff69b4.svg)][27]
[![jest](https://jestjs.io/img/jest-badge.svg)][24]

## Install

`git clone https://github.com/roalcantara/popcornx`

### Dependencies

- [Git][3]
- [Precommit][6]
- [GitLint][7]

## About

This is just a small personal project in which I aim to deepen and enrich my knowledge in:

### Frontend

- **Monorepo:** [Micro Front Ends][28] (via [Nx][9]);
  - **apps/front:** A [React][19]/[Nextjs][21]/[Typescript][30] project (via [Vercel][31])
  - **apps/admin:** An [Angular][20]/[Typescript][30] project (via [Firebase][32])
  - **apps/api:** A [NestJS][21]/[Typescript][30] project (via [Heroku][33] or [Firebase][32] - not sure)
  - **libs/ui:** A [webcomponents][34] shared library (via [Storybook][35])
  - **libs/domain:** A shared library (following [Enterprise Monorepo Angular Patterns][29])
- **Unit Tests:** Via [Jest][24]
- **E2E Tests:** Via [Cypress][25]
- **Code Style:** Via [ESLint][26] and [Prettier][27]
- **Database:** Via [Postgres][41] or [Firestore][42] - not sure
- **UI:** Responsive (probably via [Tailwindcss][36])

### Organization

- **Project Management:** Kanban via [GitHub Projects](https://github.com/roalcantara/popcornx/projects/1)
- **Semantic Commits:** Applying [Conventional Commits][8] (via [gitlint][7] and [pre-commits][6])
- **Git:** Using [GitHub Flow][43]

### DevOps

- **Automated Environments:** Triggered by each [Pull Requests][47]
- **Continuous Integration:** via [GitHub Actions][45]
- **Continuous Delivery:** For each project (via [GitHub Deployments][46] and [Semantic Release][37])
- **Web Quality:**
  - Running [Lighthouse][38] checks during the CI process
  - Running [WebVitals][39] checks during the CI process
- **Test coverage:** Coverage report (probably via [Codecov][40])

## Usage

- Run `npm run clear` to clear the cache
- Run `npm run purge` to clear the cache and node_modules
- Run `npm run reset` to clear the cache, node_modules and reinstall dependencies
- Run `npm run build` to build the projects
- Run `npm run start` to start the server
- Run `npm run test` to run all project's tests
- Run `npm run e2e` to run all e2e project's tests
- Run `npm run lint` to lint all projects

### Nx: Smart, Fast and Extensible Build System

This project was generated using [Nx][9].

#### Adding capabilities to your workspace

Nx supports many plugins which add capabilities for developing different types of applications and different tools.

These capabilities include generating applications, libraries, etc as well as the devtools to test, and build projects as well.

Below are our core plugins:

- [Angular][13]
  - `npm install --save-dev @nrwl/angular`
- [React][14]
  - `npm install --save-dev @nrwl/react`
- [Express][15]
  - `npm install --save-dev @nrwl/express`
- [Nest][16]
  - `npm install --save-dev @nrwl/nest`
- [Node][17]
  - `npm install --save-dev @nrwl/node`
- Web (no framework frontends)
  - `npm install --save-dev @nrwl/web`

There are also many [community plugins][11] you could add.

#### Generate an application

Run `nx g @nrwl/react:app my-app` to generate an application.

Run `nx generate @nrwl/angular:application my-app` to generate an Angular application.

> You can use any of the plugins above to generate applications as well.

When using Nx, you can create multiple applications and libraries in the same workspace.

#### Generate a library

Run `nx g @nrwl/react:lib my-lib` to generate a library.

> You can also use any of the plugins above to generate libraries as well.

Libraries are shareable across libraries and applications. They can be imported from `@mono-nx-test/mylib`.

#### Development server

Run `nx serve my-app` for a dev server. Navigate to http://localhost:4200/. The app will automatically reload if you change any of the source files.

#### Code scaffolding

Run `nx g @nrwl/react:component my-component --project=my-app` to generate a new component.

#### Build

Run `nx build my-app` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

#### Running unit tests

Run `nx test my-app` to execute the unit tests via [Jest][24].

Run `nx affected:test` to execute the unit tests affected by a change.

#### Running end-to-end tests

Run `ng e2e my-app` to execute the end-to-end tests via [Cypress][25].

Run `nx affected:e2e` to execute the end-to-end tests affected by a change.

#### Understand your workspace

Run `nx help` to update your workspace to the latest version of Nx.

Run `nx report` reports useful version numbers to copy into the Nx issue template.

Run `nx migrate latest` to update your workspace to the latest version of Nx.

Run `nx list` to lists the currently installed Nx plugins and other available plugins.

Run `nx list @nrwl/react` to lists capabilities in the `@nrwl/react` plugin

Run `nx reset` to clear all the cached Nx artifacts and metadata about the workspace and shuts down the Nx Daemon.

Run `nx dep-graph` to see a diagram of the dependencies of your projects.

Run `nx workspace-lint` to lint nx specific workspace files (nx.json, workspace.json) and
check existence of the configured packages and apps.
**Note:** To exclude files from this lint rule, you can add them to the `.nxignore` file

## Acknowledgements

- [Standard Readme][5]
- [Conventional Commits][8]
- [Nx: Smart, Fast and Extensible Build System][9]
- [Nx: CLI][10]
- [Nx: Community Plugins][11]
- [Nx: Workspace Plugin][12]
- [Nx: Angular Plugin][13]
- [Nx: React Plugin][14]
- [Nx: Express Plugin][15]
- [Nx: Nest Plugin][16]
- [Nx: Node Plugin][17]
- [Nx: Web Plugin][18]
- [React][19]
- [Angular][20]
- [Nest][21]
- [Express][22]
- [Node][23]
- [Jest: Delightful JavaScript Testing][24]
- [Cypress][25]
- [ESLint][26]
- [Prettier: Opinionated Code Formatter][27]

## Contributing

- Bug reports and pull requests are welcome on [GitHub][0]
- Do follow [Editor Config][2] rules.
- Everyone interacting in the project’s codebases, issue trackers, chat rooms and mailing lists is expected to follow the [Contributor Covenant][4] code of conduct.

## License

The project is available as open source under the terms of the [MIT][1] [License](LICENSE)

[0]: https://github.com/roalcantara/popcornx 'My favorite movies and series'
[1]: https://opensource.org/licenses/MIT 'Open Source Initiative'
[2]: https://editorconfig.org 'EditorConfig'
[3]: https://git-scm.com 'Git'
[4]: https://contributor-covenant.org 'A Code of Conduct for Open Source Communities'
[5]: https://github.com/RichardLitt/standard-readme 'Standard Readme'
[6]: https://pre-commit.com 'A framework for managing and maintaining multi-language pre-commit hooks'
[7]: https://jorisroovers.com/gitlint 'git commit message linter'
[8]: https://conventionalcommits.org 'Conventional Commits'
[9]: https://nx.dev 'Nx: Smart, Fast and Extensible Build System'
[10]: https://nx.dev/using-nx/nx-cli 'Nx: CLI'
[11]: https://nx.dev/community 'Nx: Community Plugins'
[12]: https://nx.dev/workspace/nrwl-workspace-overview 'Nx: Workspace Plugin'
[13]: https://nx.dev/angular/overview 'Nx: Angular Plugin'
[14]: https://nx.dev/react/overview 'Nx: React Plugin'
[15]: https://nx.dev/express/overview 'Nx: Express Plugin'
[16]: https://nx.dev/nest/overview 'Nx: Nest Plugin'
[17]: https://nx.dev/node/overview 'Nx: Node Plugin'
[18]: https://nx.dev/web/overview 'Nx: Web Plugin'
[19]: https://reactjs.org 'React'
[20]: https://angular.io 'Angular'
[21]: https://nestjs.io 'Nest'
[22]: https://expressjs.com 'Express'
[23]: https://nodejs.org 'Node'
[24]: https://jestjs.io 'Jest: Delightful JavaScript Testing'
[25]: https://cypress.io 'Cypress'
[26]: https://eslint.org 'ESLint'
[27]: https://prettier.io 'Prettier: Opinionated Code Formatter'
[28]: https://micro-frontends.org 'Micro Frontends: extending the microservice idea to frontend development'
[29]: https://go.nrwl.io/angular-enterprise-monorepo-patterns-new-book 'Enterprise Monorepo Angular Patterns'
[30]: https://typescriptlang.org 'TypeScript is JavaScript with syntax for types'
[31]: https://vercel.com 'Vercel: Enables frontend teams to do their best work'
[32]: https://firebase.google.com 'Firebase: Helps you build and run successful apps'
[33]: https://heroku.com 'Heroku: A cloud platform that lets companies build, deliver, monitor and scale apps'
[34]: https://developer.mozilla.org/en-US/docs/Web/Web_Components 'Web Components'
[35]: https://storybook.js.org 'Storybook: Build component driven UIs faster'
[36]: https://tailwindcss.com 'Tailwind CSS: Rapidly build modern websites without ever leaving your HTML'
[37]: https://semantic-release.gitbook.io/semantic-release 'Semantic Release: Fully automated version management and package publishing'
[38]: https://developers.google.com/web/tools/lighthouse 'Lighthouse: Open-source, automated tool for improving the quality of web pages'
[39]: https://web.dev/patterns/web-vitals-patterns 'Web Vitals: Patterns'
[40]: https://codecov.io 'Codecov: Ship healthier code faster with less risk'
[41]: https://heroku.com/postgres 'Heroku Postgres: SQL database as a service for all developers'
[42]: https://firebase.google.com/products/firestore 'Cloud Firestore: Store and Sync app data at global scale'
[43]: https://githubflow.github.io 'GitHub Flow'
[45]: https://www.thoughtworks.com/continuous-integration 'Continuous Integration (CI) is a development practice that requires developers to integrate code into a shared repository several times a day'
[46]: https://docs.github.com/en/actions/deployment/about-deployments/about-continuous-deployment 'GitHub: About continuous deployment'
[47]: https://docs.github.com/en/actions/deployment/targeting-different-environments/using-environments-for-deployment 'Using environments for deployment'
