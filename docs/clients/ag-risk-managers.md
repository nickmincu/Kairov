# Client: AG Risk Managers

## Overview
- **Industry:** Insurance — broker, underwriting, claims, niche agri-insurance
- **Profile:** SMB insurance operation with high document, approval, and reconciliation volume
- **Key pain points:** Paper-era inefficiencies, manual triage, re-keying, chasing, and reconciling across fragmented tools

## Vertical context
- Poultry Insurance Exchange serves Canadian poultry risks where the primary market was absent
- Broader P&C carriers struggle with paper-era inefficiencies and pressure for faster real-time service
- High regulatory burden — audit trails, compliance gates, and human checkpoints are non-negotiable

## Guardrails (insurance-specific)
- Never automate a final regulated decision without a human checkpoint
- Preserve an audit trail for inputs, outputs, approvals, and overrides
- Separate recommendation from decision
- Surface confidence, assumptions, and missing data
- Fail safely to human review when uncertainty is material
- Prefer deterministic rules for eligibility, routing, and compliance gates

## Target workflows
- Intake and triage automation for new policy applications
- Document extraction and normalization (certificates, endorsements, loss runs)
- Underwriting approval orchestration
- Claims triage and routing
- Broker/agent communication automation
- Renewal reminders and follow-up sequences
- Compliance reporting and audit log generation

## Systems likely involved
- Policy management system
- Claims system
- Email / document intake
- CRM
- Accounting / reconciliation tools
- Regulatory filing systems

## Value metrics
- Hours saved per week on manual data entry and re-keying
- Turnaround time reduced on policy issuance and claims processing
- Error rate reduced on data handoffs between systems
- Compliance audit preparation time reduced
