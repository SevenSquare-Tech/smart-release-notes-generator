smart-release-notes-generator

Automated semantic versioning and package publishing for Node.js
projects.

🚀 Overview

smart-release-notes-generator automates the whole package release workflow including:

- Determining the next version number
- Generating release notes
- Publishing to npm
- Creating GitHub releases

It follows Semantic Versioning (SemVer) and Conventional Commits to
ensure consistent and reliable releases.

---

📦 Installation

    npm install smart-release-notes-generator --save-dev

---

🧩 Requirements

- Node.js: ^22.14.0 || >=24.10.0
- npm: >=11
- A configured CI environment (GitHub Actions, GitLab CI, etc.)

---

⚙️ Basic Usage

Run smart-release-notes-generator in your CI pipeline:

    npx smart-release-notes-generator

Or via npm script:

    npm run smart-release-notes-generator

---

🔌 Included Plugins

This project uses:

- @smart-release-notes-generator/commit-analyzer
- @smart-release-notes-generator/release-notes-generator
- @smart-release-notes-generator/npm
- @smart-release-notes-generator/github

These handle version detection, changelog creation, npm publishing, and
GitHub releases.

---

🧪 Testing

Run all checks and tests:

    npm test

Individual commands

    npm run test:unit
    npm run test:integration
    npm run test:e2e

---

🧹 Linting

    npm run lint:prettier
    npm run lint:lockfile
    npm run lint:engines
    npm run lint:publish

---

📁 Project Structure

    bin/        → CLI entry
    lib/        → Core logic
    docs/       → Documentation
    test/       → Test suites
    index.js    → Main entry
    cli.js      → CLI wrapper

---

🔐 Publishing

Publishing is automated via CI using smart-release-notes-generator. No manual version
bumping is required.

Ensure:

- Proper commit messages (Conventional Commits)
- CI has npm and GitHub tokens configured
