---
name: Maintenance Report
description: Report maintenance tasks, cleanup, or housekeeping requests
labels: ['maintenance', 'needs-triage']
body:
  - type: markdown
    attributes:
      value: |
        Thanks for contributing to maintenance! 🔧
        
        Please use the **Maintenance Guidelines**: https://github.com/[REPO]/blob/main/CONTRIBUTING.md#maintenance
        
        Before creating a maintenance report, please check if:
        - The task has already been logged
        - It is an item on the current maintenance backlog
  - type: textarea
    id: description
    attributes:
      label: Maintenance Description
      description: A clear and concise description of the maintenance task
      placeholder: "Example: Remove deprecated dependencies and update to latest versions"
      value: |
        **What is the maintenance task?**
        *Please describe the current state and the action needed.*
    validations:
      required: true
  - type: textarea
    id: current-state
    attributes:
      label: Current State
      description: What is the current state of the issue?
      placeholder: "NPM audit shows 5 outdated packages and 2 security vulnerabilities"
      value: |
        **Current state:** *What problems exist now?*
  - type: textarea
    id: proposed-action
    attributes:
      label: Proposed Action
      description: What action would you like to take?
      placeholder: "Update all outdated packages and add patches for security vulnerabilities"
      value: |
        **Proposed action:** *What needs to be done? How should it be done?*
    validations:
      required: true
  - type: textarea
    id: impact
    attributes:
      label: Impact
      description: What is the impact of this maintenance task?
      placeholder: "Medium impact - improves code quality and security but may require testing"
      value: |
        **Impact:** *What are the consequences of this task?*
  - type: input
    id: estimated-effort
    attributes:
      label: Estimated Effort
      description: Rough estimate of time required (optional)
      placeholder: "2-4 hours"
  - type: checkboxes
    id: tasks
    attributes:
      label: Specific Tasks (if applicable)
      description: Break down into smaller tasks if helpful
      options:
        - label: Update package.json dependencies
        - label: Run npm audit to check for vulnerabilities
        - label: Create PR for dependency updates
        - label: Test updated dependencies
        - label: Update documentation
        - label: Other: ____________
  - type: checkboxes
    id: confirmation
    attributes:
      label: Confirmation
      description: Please confirm the following
      options:
        - label: I have checked that similar tasks are not already logged
          required: true
        - label: This task aligns with the projects maintenance goals
          required: true