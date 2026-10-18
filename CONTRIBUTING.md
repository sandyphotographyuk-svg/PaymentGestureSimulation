Contributing to PaymentGestureSimulation

Contributions welcome — thank you for helping improve this project!

Please follow these suggested steps when contributing:

1. Fork the repository
   - Click the "Fork" button in the GitHub UI to create a copy under your account.

2. Create a feature branch
   - Name the branch with a short descriptive name, for example:`feature/add-tests` or `fix/typo-readme`.
   - Example:
     ```bash
     git checkout -b feature/<short-description>
     ```

3. Add tests for new behavior
   - Add unit tests for any new features or bug fixes under a tests/ directory.
   - Aim for tests that are small, deterministic, and fast.
   - Run tests locally before committing. Example test runner:
     ```bash
     pytest -q
     ```

4. Commit changes with clear messages
   - Write clear, concise commit messages. Use present tense and include the motivation.
   - Example:
     ```bash
     git add .
     git commit -m "Add unit tests for PaymentStandingAgent gesture smoothing"
     ```

5. Push your branch to your fork
   ```bash
   git push origin feature/<short-description>
   ```

6. Open a Pull Request (PR)
   - On GitHub, open a PR from your fork/branch to `sandyphotographyuk-svg/PaymentGestureSimulation:main`.
   - In the PR description, include:
     - A short summary of changes
     - Which issue it addresses (if any)
     - Any testing steps or commands to reproduce

7. Respond to review feedback
   - Maintain a constructive and collaborative tone.
   - Make follow-up commits to the same branch to address review comments.

8. After merge
   - Pull the latest main branch into your local repository and delete your feature branch if desired:
     ```bash
     git checkout main
     git pull upstream main
     git branch -d feature/<short-description>
     ```

Additional guidance
- Code style: follow the project's existing style. If none is defined, prefer PEP8 for Python.
- Tests: prioritize unit tests and include examples where helpful.
- Issues: if you're not sure what to work on, open an issue or ask for guidance — labeled issues or "good first issue" entries are great starting points.
- License: by contributing, you agree that your contributions will be licensed under the project's Apache-2.0 license.

Optional: Pull Request template
You can add a .github/pull_request_template.md file to provide a checklist for contributors. Example content:

````markdown
### Summary

(Brief description of the changes)

### Related issue

- Fixes #<issue-number> (if applicable)

### Changes

- Bullet list of changes

### How to test

- Steps to reproduce and test the change

### Notes

- Any additional notes for reviewers
````

Thanks again for contributing — every improvement helps!
