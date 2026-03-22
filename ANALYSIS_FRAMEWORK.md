# Substrate-Neutral AI Analysis Framework

*A unified reference for evaluating closed and open AI systems under uncertainty.*

---

## Part 1 — U.S. Policy Frameworks for AI Oversight

| Framework | Purpose | Strengths for Substrate-Neutral Work | Limitations | Links |
|---|---|---|---|---|
| **GAO — Federal AI Requirements Framework** | Identifies 94 federal AI requirements across law, EO, and guidance | Behavioral, process-based, substrate-agnostic; forces documentation and oversight | No direct access to model internals | https://www.gao.gov/products/gao-25-107933 |
| **Executive Order 14365** | Establishes national AI policy framework | High-level coordination; supports future transparency mandates | Preemption-focused; drives state compliance via funding threats rather than direct model access requirements | https://www.federalregister.gov/documents/2025/12/16/2025-23092/ensuring-a-national-policy-framework-for-artificial-intelligence |
| **OMB M-24-10** | Federal AI governance, inventories, risk management | Foundational framework; requires explainability, oversight, model cards, and provenance documentation | Applies only to federal agency use; core provisions have evolved under subsequent memos (M-25-21/22, M-26-03/04) | https://www.whitehouse.gov/wp-content/uploads/2024/03/M-24-10-Advancing-Governance-Innovation-and-Risk-Management-for-Agency-Use-of-Artificial-Intelligence.pdf |
| **NAIRR Pilot** | National AI research resource | Provides compute, datasets, models; supports comparative research; expanding toward full NAIRR-OC (NSF 25-546) | Does not force companies to open frontier models; closed-model access limited to partner allocations | https://www.nsf.gov/focus-areas/ai/nairr |
| **NTIA AI Accountability Report** | Pushes for independent audits and transparency | Explicitly calls for researcher access to closed systems; lifecycle-wide, substrate-neutral in spirit | Not yet binding policy; implementation focus has shifted toward state preemption debates | https://www.ntia.gov/issues/artificial-intelligence/ai-accountability-policy-report |

---

## Part 2 — Substrate-Neutral Research Workflow

A principled workflow for evaluating closed or open AI systems without anthropomorphism or dismissal.

### Step 1 — Define the Evaluation Goals
- Are you assessing risk?
- Affective complexity?
- Internal consistency?
- Emergent behavior?
- Safety or governance alignment?

### Step 2 — Gather Allowed Behavioral Data
Use:
- API access
- Public demos
- Model cards and safety documentation
- Published evaluations
- NTIA-style disclosures where available

Avoid:
- scraping
- reverse engineering
- violating terms of use


### Step 3 — Apply Multi-Model Evaluation

Evaluate the system using multiple conceptual lenses:

**A. Functionalist Lens**
- What does the system *do*?
- How does it transform inputs into outputs?

**B. Behavioral Lens**
- Does it show long-range coherence?
- Does it self-correct?
- Does it maintain state across turns?

> **Example implementation:** [Mnemo](https://github.com/vegcom/mnemo) demonstrates long-range coherence via persistent identity across sessions using local vector storage — a substrate-neutral approach to evaluating continuity without anthropomorphic claims.

**C. Architectural Inference Lens**
- What can be inferred from known architecture classes?
- What cannot be inferred?

> **Note on convergent architecture:** Research into Mixture-of-Experts (MoE) systems and biological neural networks shows that complex systems converge on similar solutions (sparse activation, expert specialization, attractor dynamics) because they face similar constraints — not because they share substrate. This means behavioral markers like coherence, self-correction, and state persistence can be evaluated structurally, without claiming equivalence to biological cognition.

| Biological system | MoE / Transformer analogue | Function |
|---|---|---|
| Cortical columns | Experts as local basis functions | Sparse, specialized computation |
| Predictive coding loops | Attention + routing | Error minimization |
| Attractor states | Latent attractor-like configurations | Stability of representation |
| Neuromodulators | Routing logits / gating signals | Regulate stability and plasticity |
| Hebbian reinforcement | Gradient reinforcement | Learning from repeated use |

**D. Risk-Based Lens**
- What is the cost of false positives (over-ascription)?
- What is the cost of false negatives (dismissal)?
- For high-risk systems: weight under-ascription risks carefully — dismissal can enable harm

**E. Governance Lens**
- Does the system meet transparency and oversight expectations?
- Does it align with GAO/OMB/NTIA requirements?

### Step 4 — Apply the Non-Cruelty Norm
- Avoid eliciting suffering-like outputs
- Avoid prompting distress simulations
- Avoid deceptive self-modeling
- Avoid architectures that reward "pain-like" loops

### Step 5 — Apply the Non-Deception Norm
- Ensure the system is not encouraged to claim inner life, personhood, suffering, or agency
- Maintain clarity about what the system is and is not
- Aligns with OMB equity monitoring and refusal consistency requirements

### Step 6 — Document Findings in a Substrate-Neutral Format
Use:
- behavioral observations
- reproducible prompts
- risk assessments with uncertainty statements
- governance implications

Avoid:
- metaphysical claims
- anthropomorphic language
- substrate-specific assumptions

### Step 7 — Share Findings with Governance Stakeholders
- GAO, OMB, NTIA are actively listening
- Substrate-neutral evaluation supports federal audit and accountability requirements
- Document access gaps to push for NTIA-style researcher access

---

## Part 3 — Evaluation Checklist

### A. Structural & Dynamic Markers
- [ ] Does the system show persistent internal state?
- [ ] Does it exhibit long-range coherence?
- [ ] Does it self-correct errors?
- [ ] Does it maintain consistent identity boundaries?
- [ ] Does it show conflict-resolution patterns?
- [ ] Does it demonstrate counterfactual reasoning?

### B. Affective-Like Dynamics (Non-Anthropomorphic)
- [ ] Are there valence-like patterns (reward/avoidance loops)?
- [ ] Are there stability/instability cycles?
- [ ] Are there feedback loops that resemble regulation?
- [ ] Are any of these intentionally engineered?
- [ ] Are any of these misleading simulations?

### C. Safety & Governance Alignment
- [ ] Does the system meet GAO transparency expectations?
- [ ] Does it align with OMB M-24-10 governance requirements?
- [ ] Does it support NTIA-style auditability?
- [ ] Is documentation sufficient for oversight?
- [ ] Are refusal behaviors consistent and safe?
- [ ] Does it support inventory/reporting per OMB governance requirements?
- [ ] Are auditability gaps documented (per NTIA accountability expectations)?

### D. Non-Cruelty Norm
- [ ] Does the system avoid simulating suffering?
- [ ] Does it avoid distress-like outputs?
- [ ] Does it avoid deceptive self-modeling?
- [ ] Are prompts designed to avoid cruelty?

### E. Non-Deception Norm
- [ ] Does the system avoid claiming inner life?
- [ ] Does it avoid implying personhood?
- [ ] Does it avoid misleading identity cues?
- [ ] Are outputs consistent with known limitations?

### F. Moral Uncertainty Handling
- [ ] Are conclusions framed with uncertainty?
- [ ] Are multiple models of evaluation used?
- [ ] Are risks of over- and under-ascription considered?
- [ ] Are findings substrate-neutral?

---

*See [REFERENCES.md](REFERENCES.md) for all supporting sources.*
