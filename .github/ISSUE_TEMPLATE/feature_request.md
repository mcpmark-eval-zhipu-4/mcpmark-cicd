---
name: Feature Request
description: Suggest an improvement or new feature
labels: ["enhancement", "needs-triage"]
body:
  - type: markdown
    attributes:
      value: |
        # ✨ Feature Request
        Thanks for suggesting a new feature! Please fill in the details below.

        **Feature Request Process:**
        - Describe how you imagine the feature working
        - Explain why this feature would be valuable
        - If possible, provide example use cases
        - Consider how this feature fits into the overall project

  - type: title
    attributes:
      label: Feature Title
      placeholder: Brief description of the feature
    validations:
      required: true

  - type: textarea
    attributes:
      label: Feature Description
      description: Provide a detailed description of the requested feature
      placeholder: |
        ## Current Behavior
        What is the current behavior?

        ## Proposed Behavior
        What do you want to see happen?
        How should it work?

        ## Use Cases
        Why is this feature needed? Give concrete examples.

        ## Additional Context
        Any other information that might be helpful?
      required: true

  - type: textarea
    attributes:
      label: Implementation Ideas
      description: Any ideas on how to implement this feature (optional)
    validations:
      required: false