# CODE STANDARDS

This document defines the coding standards for the **BudgetWise** project. Adhering to these standards ensures consistency, readability, and maintainability throughout the codebase.

---

## Naming Conventions

### 1. **Classes and Interfaces**
- **Classes**: Use PascalCase. Example: `BudgetManager`
- **Interfaces**: Use PascalCase with an "I" prefix. Example: `IBudgetService`
- **Abstract Classes**: Use PascalCase. Example: `BaseController`

### 2. **Methods**
- Use PascalCase for method names. Example: `CalculateExpenses()`
- Methods should be named with a verb or a verb phrase that clearly indicates what they do.

### 3. **Variables and Fields**
- **Local Variables**: Use camelCase. Example: `totalExpense`
- **Instance Fields**: Use camelCase and prefix with an underscore (`_`). Example: `_budgetLimit`
- **Constants**: Use ALL_CAPS with underscores. Example: `MAX_BUDGET_AMOUNT`

### 4. **Properties**
- Use PascalCase. Example: `BudgetAmount`
- Prefer using auto-properties when possible.

### 5. **Namespaces**
- Use PascalCase, and make sure namespaces reflect the folder structure. Example: `BudgetWise.Services.DataAccess`

---

## Formatting

### 1. **Indentation and Spacing**
- Use 4 spaces for indentation. **Do not use tabs**.
- Add a blank line between method definitions and around blocks of code to improve readability.

### 2. **Braces**
- Always use braces `{}` for loops, conditionals, and other blocks, even for single-line statements.
- Place the opening brace `{` on the same line as the statement. Example:
  ```csharp
  if (condition){
      // Code block
  }
  ```

### 3. **Line Length**
- Limit each line to a maximum of 120 characters.

### 4. **File Organization**
- Place one class per file, unless classes are tightly related (e.g., nested types).
- Keep files organized in folders based on their purpose (e.g., `Models`, `Services`, `DataAccess`).

---

## Error Handling

### 1. **General Guidelines**
- Always catch exceptions explicitly, and avoid catching `System.Exception` unless necessary.
- Use custom exception classes when appropriate.

### 2. **Logging**
- Log errors using a consistent logging framework, like **Serilog** or **NLog**.
- Provide meaningful messages that help identify the cause and location of the error.

---

## Coding Best Practices

### 1. **SOLID Principles**
- Follow the SOLID principles to create clean, maintainable, and scalable code.
  - **S**ingle Responsibility Principle
  - **O**pen/Closed Principle
  - **L**iskov Substitution Principle
  - **I**nterface Segregation Principle
  - **D**ependency Inversion Principle

### 2. **Avoid Magic Numbers**
- Use named constants or enums instead of hard-coded values.

### 3. **Async/Await**
- Use asynchronous programming where appropriate to avoid blocking operations.

---

## Code Review and Pull Requests

### 1. **Code Review Checklist**
- Ensure that all methods are appropriately documented.
- Check for consistent naming conventions.
- Verify that there are no unused variables or methods.
- Review error handling and logging practices.

### 2. **Pull Request Guidelines**
- Describe the changes clearly in the pull request description.
- Make sure all new features are tested and that the code passes existing tests.
- Request at least one review before merging (self-review if working alone).