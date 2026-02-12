---
name: Waterfall Task
about: Describe this issue template's purpose here.
title: ''
labels: ''
assignees: ''

---

name: Waterfall Task
description: Create a structured task for Waterfall project execution
title: "[PHASE] Task name"
labels: ["waterfall-task"]

body:
  - type: dropdown
    id: phase
    attributes:
      label: Project Phase
      options:
        - Initiation
        - Design
        - Development
        - Testing
        - Deployment
    validations:
      required: true

  - type: input
    id: planned_start
    attributes:
      label: Planned Start Date
      placeholder: YYYY-MM-DD
    validations:
      required: true

  - type: input
    id: planned_end
    attributes:
      label: Planned End Date
      placeholder: YYYY-MM-DD
    validations:
      required: true

  - type: input
    id: duration
    attributes:
      label: Planned Duration (days)
      placeholder: e.g. 5
    validations:
      required: true

  - type: dropdown
    id: status
    attributes:
      label: Task Status
      options:
        - Not Started
        - In Progress
        - Blocked
        - Completed
    validations:
      required: true

  - type: dropdown
    id: risk
    attributes:
      label: Risk Level
      options:
        - Low
        - Medium
        - High
    validations:
      required: true

  - type: textarea
    id: dependencies
    attributes:
      label: Dependencies
      description: List tasks or approvals this task depends on

  - type: textarea
    id: notes
    attributes:
      label: Notes / Comments
