---
name: Feature Request
description: Suggest a new feature or improvement
labels: ['epic', 'enhancement', 'needs-triage']
body:
  - type: markdown
    attributes:
      value: |
        Thanks for suggesting a feature! 🎉
        
        Please use the Feature Request Process: https://github.com/[REPO]/blob/main/CONTRIBUTING.md#feature-requests
        
        Before creating a feature request, please check if:
        - The feature has already been requested
        - There's an open issue addressing this feature
  - type: textarea
    id: description
    attributes:
      label: Feature Description
      description: A clear and concise description of the feature you'd like to see
      placeholder: "Example: Add dark mode support to the application interface"
    validations:
      required: true
  - type: textarea
    id: use-case
    attributes:
      label: Use Case
      description: Why is this feature needed? What problem does it solve?
      placeholder: "Current users prefer dark mode for better visibility in low-light environments"
    validations:
      required: true
  - type: textarea
    id: proposed-solution
    attributes:
      label: Proposed Solution
      description: Describe your proposed solution (optional)
      placeholder: "Implement a theme toggle in the settings, with system preference detection"
  - type: textarea
    id: alternatives
    attributes:
      label: Alternative Solutions
      description: Have you considered any alternative solutions?
      placeholder: "Users could use browser extensions, but that's not native to the application"
  - type: input
    id: impact
    attributes:
      label: Impact
      description: How significant would this feature be?
      placeholder: "Medium impact - nice to have but not blocking"
  - type: checkboxes
    id: acceptance-criteria
    attributes:
      label: Acceptance Criteria (Optional)
      description: What criteria would make this feature a success?
      options:
        - label: Dark mode toggle in settings
        - label: Automatic system theme detection
        - label: User preference persistence across sessions
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