~~1. An organization member (e.g. Martins-23) can commit to the public repository, on the "main" branch.~~ ➡ Check point 3.  
~~2. An organization owner (e.g. Martins-33) can commit to the public repository, on the "main" branch.~~ ➡ Check point 4.  
3. An organization member (e.g. Martins-23) **CANNOT** commit directly to the "main" branch, but needs to create a PR, and it needs at least one approval.  
    ~~3.1. By setting an organization rule~~ ➡ ❌ (does not work)  
    3.2. By setting a repository-specific rule.  
4. An organization owner (e.g. Martins-33) **CANNOT** commit directly to the "main" branch, but needs to create a PR, and it needs at least one approval.  
5. A simple setup exists, to test a Python file (and function) using Pytest module.  
6. Repository has GitHub Actions.  
    6.1. Pytest tests (from *python-pytest_example*) are executed as a GitHub Action.  
    6.2. It **CANNOT** be merged a PR if Pytest tests execution fails.  
