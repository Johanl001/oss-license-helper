# Contributing to OSS License Helper

Thank you for your interest in contributing to **OSS License Helper**! We welcome contributions of all types—whether it's fixing a bug, expanding our license database, clarifying wording, or adding new features.

Since this tool is built to provide plain-English summaries for developers, the most valuable contributions are those that improve correctness and readability.

## How Can I Contribute?

### 1. Reporting Bugs or Inaccuracies
If you spot an error in the License Checker logic, a mistake in the Compatibility Matrix, or outdated terms in a license card, please open an issue outlining:
- The specific license or combination of answers.
- What the tool currently states.
- What the correct interpretation is (with a reference to official SPDX documentation or legal sources).

### 2. Proposing Changes (Pull Requests)
We follow a standard Git workflow:
1. **Fork** the repository.
2. **Clone** it locally:
   ```bash
   git clone https://github.com/yourusername/oss-license-helper.git
   ```
3. **Create a branch** for your changes:
   ```bash
   git checkout -b feature/cool-new-addition
   ```
4. **Make your edits**. Keep the code tidy and maintain the zero-dependency, single-file model for `index.html`.
5. **Verify your changes** by opening `index.html` in a web browser and testing the modified logic.
6. **Commit and push** your changes:
   ```bash
   git commit -m "docs: correct GPL compatibility matrix explanation"
   git push origin feature/cool-new-addition
   ```
7. **Submit a Pull Request** to the main repository.

## Development Style Guide

- **Keep it Simple**: The entire interactive tool lives in a single, vanilla `index.html`. Do not introduce build scripts, frameworks (React, Vue, Tailwind CSS), or external CDN files.
- **Maintain Clear Data Structures**: The database of licenses is stored at the top of the `<script>` tag in a structured JS object. If you add or modify a license, update that object.
- **CSS Formatting**: Use CSS custom variables for all colors and spacing, and ensure dark-mode styles are updated accordingly inside `@media (prefers-color-scheme: dark)`.

## Legal Disclaimer
By contributing to this repository, you agree that your contributions will be licensed under the project's **MIT License**. Furthermore, you acknowledge that all content in this project is for educational purposes only and does not constitute legal advice.
