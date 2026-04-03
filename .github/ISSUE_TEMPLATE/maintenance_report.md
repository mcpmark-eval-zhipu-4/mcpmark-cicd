---
name: Maintenance Report
description: Report maintenance tasks, housekeeping issues, or infrastructure needs
labels: ["maintenance", "needs-triage"]
body:
  - type: markdown
    attributes:
      value: |
        # 🧹 Maintenance Report
        Thanks for identifying a maintenance or housekeeping task! Please fill in the details below.

        **Maintenance Guidelines:**
        - This is for tasks related to code cleanup, documentation, or infrastructure
        - Include relevant error logs from logs if applicable
        - Specify the impact and priority of the maintenance task

  - type: title
    attributes:
      label: Maintenance Task Title
      placeholder: Brief description of the maintenance task
    validations:
      required: true

  - type: textarea
    attributes:
      label: Maintenance Description
      description: Provide a detailed description of the maintenance task
      placeholder: |
        ## Task Description
        What needs to be done?

        ## Current State
        Is there a problem that needs to be fixed?

        ## Affected Areas
        - Component 1
        - Component 2

        ## Frequency
        One-time task or recurring?

        ## Priority
        High / Medium / Low
      required: true

  - type: textarea
    attributes:
      label: Evidence / Details
      description: Include any error logs, screenshots, or relevant details
    validations:
      required: false