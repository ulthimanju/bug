## Git Setup Instructions
- Install Git from https://git-scm.com/downloads and follow the installation prompts for your OS.
- Set your global username and email:
  ```sh
  git config --global user.name "ulthimanju"
  git config --global user.email "manju.ulthi@gmail.com"
  ```
- To check your current Git configuration:
  ```sh
  git config --global user.name
  git config --global user.email
  ```
- To initialize a new repository in your project folder:
  ```sh
  git init
  ```
- To add all files and make your first commit:
  ```sh
  git add .
  git commit -m "Initial commit"
  ```
- To connect to a new GitHub repository:
  ```sh
  git remote add origin https://github.com/ulthimanju/your-repo.git
  git push -u origin master
  ```
- For authentication, use a personal access token if prompted for a password.

## Operator Interactions
-when asked to fix code, first explain the problem found in the code.
-when asked to write code, first explain the problem to be solved.
-when asked to generate tests, first explain what tests will be created.
-when making multiple changes, provide a step-by-step overview first.

## Security
-Check the code for vulnerabilities after generating.
-Avoid hardcoding sensitive information like credentials or API keys.
-Use secure coding practices and validate all inputs.

## Environment Variables
-If a .env file exists, use it for local environment variables
-Document any new environment variables in README.md
-Provide example values in .env.example

## Version Control
-Keep commits atomic and focused on single changes.
-Follow conventional commit message format.
-Update .gitignore for new build artifacts or dependencies.

## Code Style
-Follow the project's existing code style and conventions.
-Add type hints and docstrings to functions, classes and for all new functions.
-Include comments to explain complex logic.

## Change Logging
-Each time you generate code, note the changes in "changeLog.md" file.
-Follow semantic versioning guidelines.
-Include Date and description of changes in the change log.

## Testign Requirements
-Write unit tests for all new functionality and bug fixes.
-Maintain a minimum of 80% test coverage.
-Add integration tests for API endpoints.

