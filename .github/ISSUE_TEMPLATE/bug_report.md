name: Bug Report
description: Meld een bug
title: "[BUG]: "
labels: ["bug", "new"]
body:
  - type: markdown
    attributes:
      value: |
        Vul de onderstaande vragen in om ons op de hoogte te stellen van de bug
  - type: input
    id: contact
    attributes:
      label: Contact Details
      description: Wat is je discord ID. Het kan zijn dat we om extra informatie vragen.
      placeholder: ex. King Kai#4248
    validations:
      required: false
  - type: textarea
    id: what-happened
    attributes:
      label: Beschrijf de bug?
      description: Een duidelijke en beknopte beschrijving van wat de bug is.
      placeholder: |
    validations:
      required: true
  - type: textarea
    id: what-should-happen
    attributes:
      label: Te reproduceren
      description: Stappen om het probleem te reproduceren.
      placeholder: Stap 1 ... Stap 2...
  - type: dropdown
    id: frequency
    attributes:
      description: "Hoevaak komt deze bug voor?"
      label: "Frequentie van de bug"
      options:
        - Continue
        - vaker per dag
        - Eens in de week
        - Heel soms
    validations:
      required: true
  - type: dropdown
    id: impact
    attributes:
      description: "Hoog wanneer iedereen er last van heeft"
      label: "Wat is de impact van deze bug?"
      options:
        - hoog
        - laag
        - geen
