1. An organization member (e.g. Martins-23) can commit to the public repository...
    1. ~~On the "main" branch.~~ ➡ No longer, check point 1.2.
    2. but **CANNOT** commit directly to the "main" branch; needs to create a PR, and it needs at least one approval.
2. An organization owner (e.g. Martins-33) can commit to the public repository...
    1. ~~On the "main" branch.~~ ➡ No longer, check point 2.2.
    2. but **CANNOT** commit directly to the "main" branch; needs to create a PR, and it needs at least one approval.
3. A simple setup exists to test a Python file (and function) using **Pytest** module.
4. Repository has GitHub Actions:
    1. Pytest tests (from *python-pytest_example*) are executed as a GitHub Action.
        1. It **CANNOT** be merged a PR if any of the Pytest tests executions fail.
        2. The action is **ONLY** executed if any of the changed files is from the *python-pytest_example* folder.
