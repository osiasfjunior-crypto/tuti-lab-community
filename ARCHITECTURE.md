# Architecture — Public Collaboration Boundary

## This repository is not the production system
`tuti-lab-community` is a public space for documentation, sanitized experiments, and collaboration. It does not contain production Workers, live databases, deployment configuration, guest records, credentials, or private operational code.

## Collaboration model
- **Public lab:** ideas, research questions, synthetic test fixtures, documentation, and reviewed examples.
- **Private implementation:** production code, operational infrastructure, secrets, customer data, and deployment workflows remain in private repositories and authorized systems.
- **Review boundary:** public suggestions are inputs for review, not authorization to change production.

## Conceptual memory lifecycle
This is a research model, not a verified description of the production implementation:
1. Capture an information item.
2. Preserve its source and timestamp.
3. Assign context and access scope.
4. Add structured attributes and classifications.
5. Retrieve candidate records for a query.
6. Enforce all mandatory constraints, including scope, time, and required attributes.
7. Resolve links and corrections without erasing history.
8. Return evidence, or state that evidence is insufficient.

## Evidence labels
- **Verified:** supported by code inspection or reproducible test.
- **Observed:** seen in a specific run with conditions recorded.
- **Hypothesis:** plausible explanation requiring validation.
- **Proposal:** suggested future behavior or design.
- **Unknown:** not yet established.

## Security
Never commit API keys, passwords, tokens, cookies, private keys, environment files, real guest/customer data, personal identifiers, private conversations, production database exports, or unredacted logs. Use synthetic examples and scrub logs before sharing. If a secret is published, revoke or rotate it; deleting the visible file alone may not remove it from Git history.
