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
- To create a new GitHub repository from the command line using GitHub CLI:
  1. Create a new repository and push your code:
     ```sh
     gh repo create your-repo-name --public --source=. --remote=origin --push
     ```
     Replace `your-repo-name` with your desired repository name.
- To delete a repository from the command line:
  1. Make sure you have the required permissions ("delete_repo" scope):
     ```sh
     gh auth refresh -h github.com -s delete_repo
     ```
  2. Delete the repository:
     ```sh
     gh repo delete your-username/your-repo-name --yes
     ```
     Replace `your-username/your-repo-name` with the correct path.

## Spring Boot Project Setup (Maven-Style)
src/
└── main/
  ├── java/
  │   └── com/
  │       └── yourdomain/
  │           └── yourapp/
  │               ├── controller/      -> REST Controllers (API layer)
  │               ├── service/         -> Business logic
  │               ├── repository/      -> Spring Data JPA repositories
  │               ├── model/           -> Entity & DTO classes
  │               ├── config/          -> Configuration classes (Security, CORS, etc.)
  │               ├── exception/       -> Custom exceptions & handlers
  │               └── YourAppApplication.java -> Main class (with @SpringBootApplication)
  └── resources/
    ├── application.properties (or application.yml)
    ├── static/          -> Static web files (if using frontend here)
    ├── templates/       -> Thymeleaf (if used)
    └── messages.properties -> i18n messages (optional)

### Spring Boot Best Practices
-Group related functionality into packages/modules.
-Follow SOLID principles.
-Use DTOs to transfer data between layers.
-Implement proper exception handling with custom exceptions.
-Keep controllers thin, business logic in services.
-Use dependency injection instead of creating objects directly.
-Leverage Spring's features (validation, caching, etc.).
-Include comprehensive documentation with Swagger/OpenAPI.
-Follow RESTful API design principles.
-Implement proper logging throughout the application.

## React Project Setup
src/
├── assets/             # Images, fonts, static files
├── components/         # Reusable UI components (Button, Modal, etc.)
│   └── Button/
│       ├── Button.jsx
│       └── Button.module.css
├── features/           # Feature-specific folders (modular structure)
│   └── user/
│       ├── UserList.jsx
│       ├── UserForm.jsx
│       └── userSlice.js (if using Redux Toolkit)
├── hooks/              # Custom React hooks
├── pages/              # Page-level components (Home, Profile, etc.)
├── routes/             # App routing setup
│   └── AppRoutes.jsx
├── services/           # API calls and external services
│   └── userService.js
├── utils/              # Utility functions/helpers
├── App.jsx             # Main component
├── main.jsx            # Entry point (Vite) or index.js (CRA)
└── index.css

### React Best Practices
-Group files by feature (modular design).
-Keep components small and focused.
-Use props for reusability.
-Prefer CSS Modules, Tailwind, or styled-components to avoid global CSS conflicts.
-Split app into components/, pages/, features/, and services/.
-Use PropTypes or TypeScript for component typing.
-maintain a consistent naming convention (PascalCase for components, camelCase for functions).
-Use hooks for state and lifecycle management.
-maintain a clean separation of concerns (UI vs. logic).
-maintain a centralized design pattern (like Atomic Design).

## Node.js Project Setup
src/
├── controllers/        # Route handlers
├── models/             # Database models (Mongoose, Sequelize, etc.) 
├── routes/             # Express route definitions
├── services/           # Business logic and service layer
├── middlewares/        # Custom middleware functions
├── config/             # Configuration files (DB, environment variables)
├── utils/              # Utility functions/helpers
├── tests/              # Unit and integration tests
├── app.js              # Main application file (Express setup)

### Node.js Best Practices
-Use a modular structure (controllers, models, routes, services).
-Implement proper error handling with custom error classes.
-Use environment variables for configuration (dotenv).
-Use async/await for asynchronous operations.
-Implement logging (Winston, Morgan).
-Use a linter (ESLint) and formatter (Prettier) for code consistency.
-Write unit tests for all modules.
-Use a task runner (like npm scripts) for build and development tasks.


## SMTP Details
- SMTP Server: smtp.gmail.com
- Username: umanjunath2003@gmail.com
- Password: aqao xgkb mxxw ayra 
- Port: 587 (TLS) or 465 (SSL)
- Security: Requires TLS or SSL
- Authentication: Yes (using your Gmail credentials)
