# Iteration Notes — Parent/Guardian Letter Generation

This document records known failure modes observed or anticipated in the initial system prompt (v1), and the rationale for changes introduced in v2.

The goal of iteration is improved instruction-following reliability, not stylistic preference.

---

## Observed / Anticipated Failure Modes in v1

The following issues were identified as likely under v1:

- **Soft speculation**  
  Outputs sometimes included phrases such as “this may indicate” or “could suggest,” introducing unsupported inference.

- **Implied causality**  
  Relationships between attendance, performance, or behavior were occasionally framed as causal without supporting data.

- **Overgeneralized next steps**  
  The “Next Steps” section sometimes included vague future-oriented statements not grounded in input information.

- **Incomplete handling of missing data**  
  Missing fields were sometimes implied rather than explicitly acknowledged as unavailable.

These issues do not represent model malfunction, but expected behavior under insufficiently strict constraints.

---

## Changes Introduced in v2

To address the above, v2 introduces the following adjustments:

- Explicit sentence-level grounding requirements for factual claims.
- Clearer instructions for handling missing or conflicting inputs without inference.
- Tighter guidance on the “Next Steps” section to prevent invented plans or commitments.
- Stronger prohibitions against speculative or causal language.

---

## Evaluation Impact

These changes are intended to:
- reduce hallucinated or inferred content,
- improve consistency across outputs,
- and increase pass rates under the evaluation rubric without relaxing constraints.

Iteration success is measured by rubric compliance, not perceived writing quality.
