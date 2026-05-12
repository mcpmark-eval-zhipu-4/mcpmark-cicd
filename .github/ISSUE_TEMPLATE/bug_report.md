---
title: "🐛 Bug Report"
labels: ["bug", "needs-triage"]
assignees: []
body:
  - type: markdown
    attributes:
      value: |
        ## 🐛 Bug Report Guidelines
        
        Thank you for helping us improve by reporting this issue! Please complete the following information:
        
        ### Before Reporting
        - [ ] I have checked the [existing issues](../../issues?q=is%3Aissue) to avoid duplicates
        - [ ] I have verified this bug exists in the latest version
        - [ ] I have searched for similar bugs in the documentation
        
        #### 📋 Bug Report Guidelines
        
        1. **Clear Title**: Use a descriptive title that identifies the bug
        2. **Reproduction Steps**: Provide step-by-step instructions to reproduce the issue
        3. **Expected Behavior**: Describe what you expected to happen
        4. **Actual Behavior**: Describe what actually happened instead
        5. **Environment Details**: Include browser/version (if applicable), Node.js version, OS
        6. **Screenshots/Videos**: Add images or GIFs to demonstrate the bug
        7. **Error Logs**: Include any relevant error messages or stack traces
        8. **Additional Context**: Any other information that might be helpful
        
  - type: textarea
    id: description
    attributes:
      label: Bug Description
      description: A clear description of the bug
      placeholder: "Example: The login form validation is not working correctly when...
Expected: Form should validate correctly
Actual: Validation fails"
    validations:
      required: true
  - type: textarea
    id: steps
    attributes:
      label: Steps to Reproduce
      description: "Please list the exact steps to reproduce the issue. Be as detailed as possible."
      placeholder: |
        1. Navigate to ...
        2. Click on ...
        3. Enter ... in the field
        4. Click ...
      render: shell
    validations:
      required: true
  - type: textarea
    id: expected
    attributes:
      label: Expected Behavior
      description: What did you expect to happen?
      placeholder: "I expected the form to validate successfully"
    validations:
      required: true
  - type: textarea
    id: actual
    attributes:
      label: Actual Behavior
      description: What actually happened?
      placeholder: "The form validation failed even though I entered valid data"
    validations:
      required: true
  - type: dropdown
    id: environment
    attributes:
      label: Environment
      description: What environment are you experiencing this bug in?
      options:
        - "Browser (Chrome/Firefox/Safari/Edge)"
        - "Mobile App (iOS)"
        - "Mobile App (Android)"
        - "Desktop App"
        - "Command Line / Terminal"
        - "Other"
      required: true
  - type: textarea
    id: logs
    attributes:
      label: Error Logs
      description: Please paste any error messages, stack traces, or console logs (be careful not to include sensitive information!)$
      placeholder: "Paste error log here..."
      render: shell
  - type: dropdown
    id: severity
    attributes:
      label: Severity
      description: How severe is this issue?
      options:
        - "Critical - System is down or critical feature broken"
        - "High - Major feature not working"
        - "Medium - Feature works but with issues"
        - "Low - Minor issue or UX problem"
      default: "Medium"
      required: true
  - type: textarea
    id: possible-solution
    attributes:
      label: Possible Solution (Optional)
      description: Have you any ideas on how this could be fixed?
      placeholder: "Suggestion: Add proper input validation..."
  - type: checkboxes
    id: cc
    attributes:
      label: Related commit info (Optional)
      description: Link to the specific commit or PR if known
      options:
        - "@authorific-rootic"
        - "@fuecongpr"
        - "@eprobeccro"
      required: false
---