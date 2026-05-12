---
title: "💡 Feature Request"
labels: ["enhancement", "needs-triage"]
assignees: []
body:
  - type: markdown
    attributes:
      value: |
        ## ✨ Feature Request Process
        
        Thank you for sharing your feature suggestion! Before submitting, please review these guidelines:
        
        ### Before Submitting
        - [ ] I have checked the [existing issues](../../issues?q=is%3Aissue) to avoid duplicates
        - [ ] This is not a simple question (please use [ discussions ](../../discussions))
        - [ ] I have thought about how this could be implemented
        
        #### 📋 Feature Request Process
        
        1. **Clear Title**: Use a descriptive title in the form "Feature: [Feature Name]"
        2. **Problem Statement**: Describe the problem this feature would solve
        3. **Proposed Solution**: Explain your solution in detail
        4. **Use Case**: Describe how you would use this feature
        5. **Alternatives**: Have you considered alternatives?
        6. **Implementation Idea**: If you have technical ideas about implementation, share them
        
        ### Epic Requirements
        
        If this is a large feature that will require multiple sub-tasks, please describe:
        - Breaking down into smaller features or tasks
        - Dependencies between features
        - Consider sending multiple related feature request issues
        
  - type: textarea
    id: description
    attributes:
      label: Feature Description
      description: A clear description of what feature you're requesting
      placeholder: "Describe the feature you would like to see implemented..."
    validations:
      required: true
  - type: textarea
    id: problem
    attributes:
      label: Problem Statement
      description: What problem does this feature solve? Why is it needed?
      placeholder: "Currently, there is no way to... This is a problem because..."
    validations:
      required: true
  - type: textarea
    id: solution
    attributes:
      label: Proposed Solution
      description: Describe your solution in detail. How would this feature work?
      placeholder: |-
        One possible solution:
        
        1. Add a new endpoint/API endpoint
        2. Modify the UI to include...
        3. Update the database schema...
        
        The flow would be:
        1. User triggers action
        2. System processes...
        3. Returns result to user
    validations:
      required: true
  - type: textarea
    id: use-case
    attributes:
      label: Use Case
      description: How would this feature be used? Please provide examples
      placeholder: |
        Example usage:
        
        ```javascript
        // Example code showing how to use the feature
        const result = await someFeature.start();
        ```
    validations:
      required: false
  - type: textarea
    id: alternatives
    attributes:
      label: Alternative Solutions
      description: Have you considered any alternatives? Or how do you imagine this feature could be solved?
      placeholder: "I've thought about implementing it via..."
    validations:
      required: false
  - type: textarea
    id: implementation
    attributes:
      label: Implementation Ideas (Optional)
      description: Any technical ideas or concerns about the implementation?
      placeholder: "Potential technical approaches:"
  - type: dropdown
    id: priority
    attributes:
      label: Priority
      description: How important is this feature?
      options:
        - "Must Have - Critical for core functionality"
        - "Should Have - Important but not blocking"
        - "Nice to Have - Adds value but not essential"
        - "Future Consideration - Could be implemented later"
      default: "Nice to Have"
      required: true
  - type: checkbox
    attributes:
      label: "Does this include breaking changes?"
      description: "Is this feature a breaking change from existing functionality?"
    required: false
  - type: textarea
    id: files
    attributes:
      label: Related Files (Optional)
      description: If you know which files might be affected, please list them
      placeholder: "src/components/ExampleComponent.js, src/utils/helpers.js"
---