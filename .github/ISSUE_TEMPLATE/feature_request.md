---
name: Feature Request
description: Suggest a new feature or improvement
labels: ['epic', 'enhancement', 'needs-triage']
body:
  - type: markdown
    attributes:
      value: |
        Thanks for suggesting a feature! 🎨
        
        Please use the **Feature Request Process**: https://github.com/[REPO]/blob/main/CONTRIBUTING.md#feature-requests
        
        Before creating a feature request, please check if:
        - The feature has already been requested
        - There is an open issue addressing this feature
  - type: textarea
    id: description
    attributes:
      label: Feature Description
      description: A clear and concise description of the feature you would like to see
      placeholder: "Example: Add dark mode support to the application interface"
      value: |
        **What feature would you like?**
        *Please describe the feature in detail.*
        
        **Why is this feature needed?**
        *What problem does it solve? Who does it benefit?*
    validations:
      required: true
  - type: textarea
    id: use-case
    attributes:
      label: Use Case
      description: Why is this feature needed? What problem does it solve?
      placeholder: "Current users prefer dark mode for better visibility in low-light environments"
      value: |
        **Use case:** *How would this feature be used?*
    validations:
      required: true
  - type: textarea
    id: proposed-solution
    attributes:
      label: Proposed Solution
      description: Describe your proposed solution (optional but helpful)
      placeholder: "Implement a theme toggle in the settings, with system preference detection"
      value: |
        **Proposed solution:** *How would you implement this feature? Details are welcome.*
  - type: textarea
    id: alternatives
    attributes:
      label: Alternative Solutions
      description: Have you considered any alternative solutions or workarounds?
      placeholder: "Users could use browser extensions, but that is not native to the application"
  - type: select
    id: impact
    attributes:
      label: Impact
      description: How significant would this feature be?
      options:
        - Critical (Required for the project to function)
        - High (Significant improvement to user experience)
        - Medium (Nice to have but not blocking)
        - Low (Minor enhancement or polish)
  - type: checkboxes
    id: acceptance-criteria
    attributes:
      label: Acceptance Criteria (Optional)
      description: What criteria would make this feature a success?
      options:
        - label: Feature is implemented as described
        - label: Feature works on all supported platforms
        - label: Feature is documented
  - type: checkboxes
    id: confirmation
    attributes:
      label: Confirmation
      description: Please confirm the following
      options:
        - label: I have searched for existing features or issues
          required: true
        - label: This feature would provide value to the project
          required: true