---
title: "🔧 Maintenance Task"
labels: ["maintenance", "needs-triage"]
assignees: []
body:
  - type: markdown
    attributes:
      value: |
        ## 🔧 Maintenance Guidelines
        
        Thank you for contributing to the maintenance of this repository! This issue type is for:
        - Code cleanup and refactoring
        - Documentation updates
        - Dependency upgrades
        - Performance improvements
        - Technical debt reduction
        - Housekeeping tasks
        
        #### 📋 Maintenance Guidelines
        
        1. **Clear Title**: Use a descriptive title that indicates the maintenance type
        2. **Description**: Provide context on why this maintenance is needed
        3. **Scope**: Define what areas will be affected
        4. **Impact**: Explain the expected benefits of this maintenance
        5. **Testing**: Consider what tests might be relevant
        
        ### Types of Maintenance
        
        - **Code Health**: Removing dead code, improving code quality
        - **Documentation**: Updating README, comments, or API docs
        - **Performance**: Optimizing slow code or memory usage
        - **Dependencies**: Updating npm packages, modernizing versions
        - **Reliability**: Adding error handling, improving robustness
        - **Security**: Patching vulnerabilities, improving security practices
        
  - type: textarea
    id: description
    attributes:
      label: Maintenance Task Description
      description: A clear description of the maintenance task
      placeholder: "Describe the maintenance task and its purpose..."
    validations:
      required: true
  - type: textarea
    id: scope
    attributes:
      label: Scope
      description: Which areas will be affected by this maintenance?
      placeholder: |
        Areas to be modified:
        1. 
        2. 
        3. 
        
        Areas to remain unchanged:
        1. 
---
  - type: textarea
    id: motivation
    attributes:
      label: Motivation
      description: Why is this maintenance needed? What problem will it solve?
      placeholder: "This maintenance is needed because..."
    validations:
      required: true
  - type: textarea
    id: impact
    attributes:
      label: Expected Impact
      description: What are the expected benefits of this maintenance?
      placeholder: |
        
        - **Performance**: Expected improvement of...
        - **Readability**: Code will be more readable because...
        - **Maintainability**: Future changes will be easier because...
        - **Security**: Vulnerabilities addressed...
        
        
        
  - type: dropdown
    id: maintenance-type
    attributes:
      label: Maintenance Type
      description: What type of maintenance is this?
      options:
        - "Code Health - Cleanup/refactor code"
        - "Documentation - Update docs/readme"
        - "Performance - Optimize speed/memory"
        - "Dependencies - Update packages/versions"
        - "Reliability - Improve error handling"
        - "Security - Address vulnerabilities"
        - "Technical Debt - Reduce debt/patterns"
        - "Other"
      default: "Other"
      required: true
  - type: textarea
    id: approach
    attributes:
      label: Proposed Approach (Optional)
      description: How do you plan to approach this maintenance task?
      placeholder: "Approach:
    
    1. 
    2. 
    3. "
  - type: dropdown
    id: effort
    attributes:
      label: Effort Level
      description: Approximate effort required
      options:
        - "Minor - Small change, quick fix"
        - "Moderate - Requires planning and testing"
        - "Significant - Large undertaking"
        - "Ongoing - Part of a longer-term effort"
      default: "Moderate"
      required: true
---