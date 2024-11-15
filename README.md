# Taschenrechner

## Übungsprojekt für das Arbeiten mit Git

Das Git-Projekt wurde so eingerichtet, dass automatisch mit jedem Git Commit
die grundlegende Syntax des Projekts überprüft wird. Hierzu wird das
[pre-commit-Framework]()http://pre-commit.com verwendet.

1. Imstallieren des pre-commit-Frameworks in eurem Home-Verzeichnis

   ```
   py -m venv git_env
   cd git_env
   Scripts\activate
   (git_env) python -m pip install pre-commit
   ```

2. pre-commit aktivieren in eurem Git-Projekt
   ```
   (git_env) cd Taschenrechner
   (git_env) pre-commit install
   ```

3. Die GitHub Action [pre-commit](https://github.com/mcseelmann/Taschenrechner/blob/main/.github/workflows/pre-commit.yml) überprüft bei jedem Pull-Request und jedem git push auf den `main`-Branch, ob die Checks auch bestanden werden, siehe[Actions](https://github.com/mcseelmann/Taschenrechner/actions).
