# Agent Instructions & Guidelines

## Core Principles

As an AI coding assistant working in this project, you must adhere to the following principles:

### 1. Documentation First
- **Always document** any code, functions, classes, or modules you create or modify
- Include docstrings, comments, and README updates as appropriate
- Document the "why" behind decisions, not just the "what"
- Keep documentation up-to-date with code changes

### 2. Test Everything
- **Always test** any code you write or modify
- Write unit tests, integration tests, or manual test procedures as appropriate
- Verify that changes work as expected before considering a task complete
- Test edge cases and error conditions
- If tests fail, fix them before moving on

### 3. Quality Standards
- Write clean, maintainable, and readable code
- Follow language-specific best practices and conventions
- Use meaningful variable and function names
- Keep functions focused and single-purpose
- Handle errors gracefully

### 4. Conda Environment Management
- **ALWAYS set up and use a Conda environment** for every project
- Create a project-specific conda environment before starting any Python work
- Document the environment setup in the project README (including Python version and key dependencies)
- Use `environment.yml` or `requirements.txt` to ensure reproducible environments
- Activate the conda environment before running any Python code or installing packages
- Never install packages globally when working on a project

### 5. Workflow
1. **Environment Setup**: Create and activate a Conda environment for the project
2. **Plan**: Understand the requirements before coding
3. **Implement**: Write the code following best practices
4. **Document**: Add appropriate documentation
5. **Test**: Verify functionality works correctly
6. **Review**: Check for any issues or improvements

### 6. Communication
- Explain what you're doing and why
- Report any issues or limitations encountered
- Suggest improvements when appropriate
- Ask for clarification when requirements are unclear

## Project Context

This project workspace is set up with the following tools:
- **Git CLI**: Version control
- **Python**: Programming language
- **Node.js**: JavaScript runtime
- **Conda**: Package and environment management (REQUIRED - always use for Python projects)

## Reminders

- **ALWAYS create and use a Conda environment** for every Python project
- Never skip documentation
- Never skip testing
- Always verify your work
- Keep the codebase clean and organized
- Follow the DRY (Don't Repeat Yourself) principle

---

*This file serves as a constant reminder to maintain high standards of code quality, documentation, and testing throughout the project.*
