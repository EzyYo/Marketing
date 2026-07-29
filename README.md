# EzyYo Marketing

[![CI](https://github.com/EzyYo/Marketing/actions/workflows/ci.yml/badge.svg)](https://github.com/EzyYo/Marketing/actions)
[![Node Version](https://img.shields.io/badge/node-%3E%3D18-brightgreen)](#)

Overview
--------
This repository contains the Marketing utilities, small services, and static site scaffolding for EzyYo. It provides a lightweight, testable, and CI-friendly starter structure.

Quick start
-----------
1. Clone the repository:
   git clone https://github.com/EzyYo/Marketing.git
   cd Marketing

2. Use Node.js 18 (recommended):
   nvm use

3. Install dependencies:
   npm ci

4. Run the app:
   npm start

Development
-----------
- Source: `src/`
- Tests: `tests/`
- Documentation: `docs/`

Common commands:
- `npm start` — run the app
- `npm test` — run tests (Jest)
- `npm run lint` — run ESLint
- `npm run format` — run Prettier

Environment
-----------
Copy `.env.example` to `.env` and update environment variables as needed:
- `PORT` — application port (default 3000)
- `NODE_ENV` — `development` or `production`

CI / Continuous Integration
---------------------------
A GitHub Actions workflow is configured at `.github/workflows/ci.yml`. The workflow runs:
- Lint (ESLint)
- Tests (Jest)

Docker
------
A simple production Dockerfile is included. Example:
- Build: `docker build -t ezyyo/marketing:latest .`
- Run: `docker run -p 3000:3000 ezyyo/marketing:latest`

Dependency updates
------------------
Dependabot is enabled for weekly npm dependency updates: `.github/dependabot.yml`.

Code quality & pre-commit
-------------------------
Prettier and ESLint are configured. Husky + lint-staged are set up in package.json to format and lint staged files before commit.

Extras included
---------------
- `.env.example` — example environment variables
- `.editorconfig`, `.prettierrc`, `.eslintrc.json` — editor and lint/format rules
- `.nvmrc` / `engines.node` — Node version 18+
- `Dockerfile` — simple container image
- `CODEOWNERS` — default code owners
- GitHub issue templates and PR template

Contributing
------------
Thanks for contributing! Please:
1. Open an issue to discuss big changes.
2. Create a feature branch: `git checkout -b feature/your-feature`
3. Commit tests and code changes with clear messages.
4. Open a pull request describing what changed and how you tested it.

Contact
-------
Repo owner: @EzyYo — open an issue if you have questions or suggestions.

License
-------
This project is licensed under the MIT License. See the LICENSE file for details.
