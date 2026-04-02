---
name: Bug Report
description: Report a bug that prevents the application from working correctly
labels: ['bug', 'needs-triage']
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to report this bug! 🐛
        
        Please use the **Bug Report Guidelines**: https://github.com/[REPO]/blob/main/CONTRIBUTING.md#bug-reports
        
        Before creating a bug report, please check if:
        - The issue has already been reported
        - There is an open issue addressing this problem
  - type: textarea
    id: description
    attributes:
      label: Bug Description
      description: A clear and concise description of what the bug is
      placeholder: "Example: Login form validation is not working, users can submit empty passwords"
      value: |
        **What is the bug?**
        *Please describe the bug clearly and concisely.*
        
        **Expected behavior:**
        *What should have happened?*
        
        **Actual behavior:**
        *What actually happened?*
    validations:
      required: true
  - type: textarea
    id: steps-to-reproduce
    attributes:
      label: Steps to Reproduce
      description: Steps to reproduce the behavior
      placeholder: |
        1. Go to '...'
        2. Click on '....'
        3. See error
      value: |
        1. Open the application
        2. Navigate to the specific page or section
        3. Perform the action
        4. Observe the unexpected behavior
    validations:
      required: true
  - type: textarea
    id: expected-behavior
    attributes:
      label: Expected Behavior
      description: What you expected to happen
      placeholder: "Password validation should prevent empty passwords"
      value: |
        **Expected behavior:** *What you expected to happen instead*
    validations:
      required: true
  - type: textarea
    id: actual-behavior
    attributes:
      label: Actual Behavior
      description: What actually happened
      placeholder: "Users can submit forms with empty passwords"
      value: |
        **Actual behavior:** *What actually happened*
    validations:
      required: true
  - type: textarea
    id: logs
    attributes:
      label: Logs
      description: Relevant log output, error messages, stack traces
      placeholder: |
        ```
        Error: Validation failed
        at validateForm(P.js:45)
        ...
        ```
    validations:
      required: false
  - type: select
    id: severity
    attributes:
      label: Severity
      description: How critical is this issue?
      options:
        - Critical (Production outage)
        - High (Major functionality broken)
        - Medium (Partial functionality affected)
        - Low (Minor issue or edge case)
      required: true
  - type: input
    id: environment
    attributes:
      label: Environment
      description: Browser, Node.js version, OS, etc.
      placeholder: "Chrome 120, Node.js v20.10.0, macOS Sonoma"
  - type: checkboxes
    id: confirmation
    attributes:
      label: Confirmation
      description: Please confirm the following
      options:
        - label: I have checked that there are no existing reports for this bug
          required: true
        - label: The bug is reproducible with the latest code from the main branch
          required: true