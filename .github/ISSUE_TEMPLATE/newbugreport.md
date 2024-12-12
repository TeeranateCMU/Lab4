---
name: NewBugReport
description: File a bug report
about: Describe this issue template's purpose here.
title: "[Bug]: "
labels: ["bug", "triage"]
projects: ["octo-org/1", "octo-org/44"]
assignees:
    - octocat
body:
    - type: markdown
    attributes:
        value: |
            Thanks for taking the time to fill out this bug report!
    - type: input
    id: contact
    attributes:
        label: Contact Details
        description: How can we get in touch with you if we need more info?
        placeholder: ex. email@example.com
    validations:
        required: false
    - type: textarea
        id: what-happend?
        attributes:
        label: What happended?
        description: Also tell us, what did you expect to happend?
        placeholder: Tell us what you see!
        value: "A bug happended!"
    validations: 
        required: true
    - type: dropdown
        id: browsers
        attributes:
        label: What browsers are you seeing the problem on?
        multiple: true
        options:
            - Firefox
            - Chrome
            - Safari
            - Microsoft Edge
    - type : textarea
        id: logs
        attributes: 
            label: Relevant log output
            description: Please copy and paste any relevent log output. This will 
            be automatically formatted into code, so no need for backticks.
            render: shell
    - type: checkboxes
    id: terms
    attributes:
        label: Code of Conduct
        description: By submitting this issue, you agree to follow our [Code of Conduct] (https://example.com)
        options:
            - label: I agree to follow this project's Code of Conduct
                required: true
---

