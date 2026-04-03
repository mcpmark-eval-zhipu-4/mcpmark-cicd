---
name: Bug Report
description: Report a bug in our software
labels: ["bug", "needs-triage"]
body:
  - type: markdown
    attributes:
      value: |
        # 🐛 Bug Report
        Thanks for taking the time to report a bug! Please fill in the details below.

        **Bug Report Guidelines:**
        - Make sure you're running the latest version
        - Check if the bug has already been reported
        - Provide clear steps to reproduce the issue
        - Include any relevant error messages or screenshots

  - type: title
    attributes:
      label: Bug Title
      placeholder: Brief description of the bug
    validations:
      required: true

  - type: textarea
    attributes:
      label: Bug Description
      description: Provide a detailed description of the bug
      placeholder: |
        ## Expected Behavior
        What should happen?

        ## Actual Behavior
        What is happening instead?

        ## Steps to Reproduce
        1. Step 1
        2. Step 2
        3. Step 3

        ## Environment
        - Version: ...
        - OS: ...
        - Browser: ...
      required: true

  - type: textarea
    attributes:
      label: Error Messages
      description: Paste any error messages or stack traces here
    validations:
      required: false