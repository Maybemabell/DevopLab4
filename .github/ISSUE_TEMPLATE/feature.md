---
name: Feature
about: Describe this issue template's purpose here.
title: ''
labels: ''
assignees: ''

---

name: Feature Request
description: Suggest an idea for this project
title: "Feature: "
labels: ["enhancement"]
body:
  - type: input
    id: contact
    attributes:
      label: Contact Details
      description: What is your name?
      placeholder: ex. Sretha Thavisin
    validations:
      required: true
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this bug report!
  - type: dropdown
    id: request-type
    attributes:
      label: Type of request?
      description: Select the type of your request
      options:
        - New Feature
        - Improvement
        - UI/UX
    validations:
      required: true
  - type: dropdown
    id: os
    attributes:
      label: What is the OS which you want to suggest?
      multiple: true
      options:
        - Windows
        - MacOS
        - Linux
        - iOS
        - Android
  - type: textarea
    id: details
    attributes:
      label: What are the details of your suggestion?
      description: Explain what do you want
      placeholder: Feature details!
    validations:
      required: true
