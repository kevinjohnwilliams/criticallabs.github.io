# Safety Critical Labs — Master Strategy

> **This document is the north star. It lives here, gets updated here, and governs what gets built next.**  
> Private. Internal only. Not for distribution.

---

## What We Are Building

Safety Critical Labs is a **certification authority** — not a consulting firm, not a services shop.

The product is the **mark**. The mark is only valuable if:
1. The standard behind it is rigorous, transparent, and domain-grounded
2. The authority behind the mark is trusted

Every decision — what to build, what to publish, who to hire, who to partner with — should be evaluated against those two criteria. If it strengthens the standard or the authority, do it. If it doesn't, defer it.

The closest analogies are **UL** (product safety), **DNV** (maritime/energy assurance), and **ISO registrar bodies** (quality management). Not McKinsey. Not an engineering firm. A certification authority with a mark that means something.

---

## The Three-Layer Architecture

### Layer 1 — The Standard (Public)

The AI Requirements Framework is the foundation. It must be:

- **Open** — publicly available on GitHub, readable by anyone, auditable by anyone
- **Versioned** — every release is numbered, dated, and immutable once published
- **Citable** — formally published in a venue that creates a persistent, referenceable record
- **Domain-grounded** — every requirement traces to a real failure mode in a real system, not a theoretical concern from a standards committee

The standard being open is a feature, not a vulnerability. No one can accuse us of certifying against a black box. Transparency is the foundation of trust.

**Current state:** Framework v1.0 published February 2025. Nine requirement areas (AI-1 through AI-9). Algorithm-agnostic. Domain-applicable beyond spaceflight.

**What "citable" means in practice:**
- Conference paper submission (AIAA, IEEE, INCOSE are the right venues)
- NASA Technical Report (explore whether JSC can publish as a contractor contribution)
- Peer-reviewed journal (longer timeline but highest authority)
- At minimum: Zenodo DOI for the GitHub release (do this now — it takes 10 minutes)

### Layer 2 — The Mark and Methodology (Proprietary)

The certification mark is what we protect aggressively. The methodology is how audits are conducted — what evidence packages look like, how findings are graded, what remediation paths exist.

**The mark is the business.** Everything else supports it.

**What needs to exist for the mark to mean something:**
- Documented audit methodology (not public)
- Standardized evidence package templates (not public)
- Finding grading rubric with consistent pass/fail criteria (not public)
- Remediation and re-assessment process (not public)
- Certificate format and issuance process (partially public — customers need to know what they're getting)

**What needs to exist for the mark to be protected:**
- Trademark registration — "Safety Critical Labs" and the certification mark/logo
- In every relevant Nice class (primarily Class 42: scientific and technological services)
- File in USPTO first, then Madrid Protocol for international coverage when ready

### Layer 3 — Accreditation (Long-term)

Long-term, Safety Critical Labs must itself be accredited — meaning a recognized national body has validated that our certification process meets defined quality standards.

In the US: **ANAB** (ANSI National Accreditation Board) or **A2LA**  
In Europe: National accreditation bodies under EA (European co-operation for Accreditation)  
ISO standard governing certification bodies: **ISO/IEC 17065**

This is a multi-year play. It requires:
- Documented quality management system for the certification process itself
- Demonstrated independence and impartiality
- Competency records for all personnel conducting assessments
- External audit by the accreditation body

**Why this matters:** Accreditation transforms the SCL mark from "credible third party" to "regulatory instrument." It's the difference between a certificate that customers want and a certificate that regulators require.

---

## Business Model

### Revenue Streams (in build order)

**1. Initial Certification Assessments**  
Client goes through the four-phase process and receives a certificate. This is the primary product.

The four phases:
1. Applicability determination — classify the AI system, establish which requirements apply
2. Evidence package review — documentation, test reports, verification matrices
3. Technical assessment — structured audit against framework requirements
4. Certification issuance — formal determination document with requirement set, classification level, and framework version

**2. Surveillance Audits**  
Recurring revenue. Required to maintain certificate validity. Frequency TBD by classification — Safety-Critical likely annual, Mission-Critical biennial.

The framework already mandates this technically (AI-4: Continuous Validation). We've built the business model into the technical standard.

**3. Readiness Assessment (Pre-Certification)**  
Organizations that aren't ready to certify but want to know where they stand. Lower-margin, high-volume, feeds the certification pipeline. Also protects the certification pass rate — clients who certify should be clients who are ready.

**4. Framework Licensing**  
Regulatory bodies, large primes, or government agencies that want to adopt the framework internally or reference it in procurement requirements. The most scalable revenue stream long-term and the least labor-intensive.

**5. Training Programs**  
Teaching organizations to understand and implement the framework requirements. Creates pipeline. Builds ecosystem familiarity with the standard.

### Pricing Philosophy

Pricing should reflect the value of the mark, not the cost of the audit labor. A UL listing isn't priced at "hours spent testing." It's priced at the value of the assurance it provides and the liability it allocates.

---

## The Credibility Arc

### Now — Personal Credentials

Authority currently rests on Kevin Williams' direct experience:
- Developed AI certification requirements for NPR 7150.2D (NASA's human-rated software standard)
- NASA Silver Bear Award for this work
- Barrios Technology / NASA Johnson Space Center
- M.S. AI, University of Michigan (in progress)
- Published research (electrochemical THC detection — demonstrates rigorous scientific methodology)
- Prior: Ford Motor Company, materials labs

This is enough to get the first customers. The goal is to transfer credibility from the person to the institution.

### Near-term — Institutional Credibility

- **Advisory board** — recruit domain experts from aerospace, automotive, medical, defense. Even 3-4 names with the right backgrounds changes how the company is perceived.
- **Framework publication** — formal citation record (see Layer 1 above)
- **Regulatory engagement** — submit the framework as a comment to FAA, FDA, or DoD AI policy processes where they're soliciting input. Being in the public record of a regulatory process is significant.
- **First certification case study** — even one organization going through the process creates a reference. Pilot assessments at reduced cost are research, not charity.

### Long-term — Institutional Authority

- Technical committee structure — external experts contribute to framework evolution, the way ISO standards develop. Removes the "one person's opinion" vulnerability.
- ANAB/A2LA accreditation (see Layer 3)
- Regulatory adoption — framework referenced in agency guidance, procurement requirements, or ATC/airworthiness criteria
- Academic partnerships — university research programs using the framework

---

## IP Strategy

### What We Protect and How

| Asset | Protection Mechanism | Priority | Status |
|---|---|---|---|
| "Safety Critical Labs" name | Trademark (USPTO Class 42) | **Critical** | To do |
| SCL certification mark/logo | Trademark (USPTO Class 42) | **Critical** | To do |
| Framework document text | Copyright (automatic) | Done | ✓ |
| Audit methodology | Trade secret | High | In progress |
| Evidence templates | Trade secret + Copyright | High | To do |
| Finding rubrics | Trade secret | High | To do |
| "SCL Certified" mark | Trademark | Critical | To do |

### What We Do Not Try to Patent

Requirements frameworks, certification processes, and audit methodologies are not patentable subject matter. The ISO 9001 analogy is correct — the standard is open, the mark is protected, the methodology is proprietary, and the accreditation is the authority.

### What Counts as a Trade Secret

For something to qualify as a trade secret, it must:
1. Derive independent economic value from not being generally known
2. Be subject to reasonable steps to maintain its secrecy

This means the audit methodology, grading rubrics, and internal evidence templates should be:
- Stored in this private repo
- Covered by NDA before sharing with any external party
- Referenced in client contracts as proprietary

---

## Build Sequence

### Phase 0 — Foundation (Now)
- [ ] Register trademark: "Safety Critical Labs" (USPTO, Class 42)
- [ ] Register trademark: SCL certification mark/logo (design the logo first)
- [ ] Create Zenodo DOI for Framework v1.0 (10 minutes, do this now)
- [ ] Make this repo private, establish clean folder structure
- [ ] Draft NDA template for any external sharing

### Phase 1 — First Assessments (Months 1-6)
- [ ] Operationalize the audit methodology — document how an actual assessment runs
- [ ] Build evidence package templates (Appendix C of the framework is the starting point)
- [ ] Build finding grading rubric — what does "pass," "conditional pass," "fail" look like with specificity
- [ ] Identify 2-3 pilot assessment candidates (aerospace startups, defense contractors, medical device AI companies)
- [ ] Run first assessment — document everything, treat it as research
- [ ] Draft certificate format
- [ ] Identify 3-4 advisory board candidates — reach out

### Phase 2 — Formal Publication and Regulatory Engagement (Months 6-18)
- [ ] Submit framework as conference paper (AIAA Digital Avionics, IEEE DASC, or INCOSE IS)
- [ ] Submit public comment to at least one regulatory AI policy process (FAA AI Roadmap, DoD AI policy)
- [ ] Publish case study from first assessment (sanitized, with client permission)
- [ ] Advisory board formalized — at least 3 members, documented
- [ ] Begin ISO/IEC 17065 gap assessment (understand what accreditation requires)

### Phase 3 — Scale and Accreditation Path (Months 18-36)
- [ ] Hire or contract first additional assessor — build auditor training program
- [ ] Framework v2.0 — incorporate learning from first assessments, technical committee input
- [ ] Initiate ANAB or A2LA pre-assessment inquiry
- [ ] International trademark filing (Madrid Protocol) for key markets
- [ ] Framework referenced in at least one regulatory document or procurement requirement

### Phase 4 — Authority (Year 3+)
- [ ] ANAB/A2LA accreditation achieved
- [ ] SCL mark recognized by at least one regulatory body
- [ ] Technical committee formalized — external experts contributing to framework evolution
- [ ] Framework v3.0 under committee governance
- [ ] Licensing agreements with primes or government agencies

---

## Target Markets

### Primary (Near-term)
- **Aerospace and defense** — AI systems in human-rated vehicles, autonomous systems, mission-critical decision support. Highest bar, highest credibility signal.
- **Aviation** — FAA AI Safety Roadmap creates near-term regulatory demand. DO-178C ecosystem has established certification culture.

### Secondary (Medium-term)
- **Medical devices** — FDA AI/ML-based Software as a Medical Device (SaMD) guidance creates demand. High regulatory pressure, established certification culture.
- **Automotive** — ISO 26262 / SOTIF ecosystem. Large market, mature safety culture.

### Tertiary (Long-term)
- **Industrial / critical infrastructure** — power grid, water, nuclear. Slower-moving but enormous.
- **Defense primes** — internal AI system certification for DoD programs.

### Domain-Agnostic Positioning
The framework is explicitly domain-agnostic. This is both technically true and strategically important — it means the SCL mark can follow AI wherever AI goes into critical systems, without rebuilding the standard from scratch for each domain.

---

## What the Certificate Says

A Safety Critical Labs certificate is a **formal determination** — not a recommendation, not a risk assessment, not a safety claim.

It states:
- This system was assessed against the SCL AI Requirements Framework, version X.X
- At the [Safety-Critical / Mission-Critical / Mission Support] classification level
- The following requirement sets were assessed: [AI-1 through AI-N]
- The following findings were made: [summary]
- The certificate is valid as of [date] and subject to surveillance per Section [X]

**What it does not say:**
- This system is safe
- This system will not fail
- This system is approved for any specific regulatory purpose

This framing protects against liability while remaining maximally useful. It's exactly how UL listings work — UL doesn't say a product is safe, it says the product was tested against a defined standard and met the requirements.

---

## Competitive Landscape

### Current State
There is no direct competitor doing what Safety Critical Labs is doing. This is both an opportunity and a risk — the market has to be educated as it is captured.

### Adjacent Players
- **Certification bodies (BSI, Bureau Veritas, SGS)** — large, general-purpose, not AI-specific. Could move into this space but are slow and lack domain depth.
- **AI auditing firms (KPMG, Deloitte AI practices)** — advisory and assessment, not certification. No mark, no standard.
- **Standards bodies (ISO, IEEE, SAE)** — produce standards, do not certify against them. Potential partners, not competitors.
- **Government labs (NIST, DLR)** — produce frameworks (NIST AI RMF), do not certify. Potential for framework adoption.

### Defensibility
The moat is not the framework document — anyone can read it. The moat is:
1. The mark, once it carries regulatory recognition
2. The institutional credibility built through first-mover presence in regulatory processes
3. The auditor competency and methodology built through real assessments
4. The origin story — framework built from inside the operational environment, not from a committee

---

## Working Principles

**The standard before the business.** Shortcuts in the framework undermine the mark. The mark is the business.

**Determinations, not recommendations.** Every output is a formal finding, not an opinion. This protects us and creates value for clients who need something to show regulators.

**Continuous validation is non-negotiable.** We built it into the technical standard because it's true. A certificate issued at deployment is not a certificate valid at month six. We don't issue certificates that pretend otherwise.

**Open standard, proprietary methodology.** The standard is public — we certify against something anyone can read. The methodology for how we assess is ours.

**First-mover means first writer.** Being in the regulatory record early — as a commenter, as a reference, as a cited source — is how standards get adopted. Write things down. Publish them. Engage every open comment period.

---

## Folder Structure (This Repo)

```
/
├── README.md                        ← This document
├── framework/
│   ├── v1.0/                        ← Published framework (frozen)
│   │   └── AI_Requirements_Framework_v1.0.md
│   └── drafts/                      ← Working drafts for v2.0
├── methodology/                     ← PROPRIETARY — audit process
│   ├── assessment-process.md
│   ├── evidence-package-guide.md
│   └── finding-grading-rubric.md
├── templates/                       ← PROPRIETARY — client-facing templates
│   ├── applicability-determination.md
│   ├── evidence-package-checklist.md
│   ├── test-report-template.md
│   └── certificate-template.md
├── legal/                           ← IP and legal documents
│   ├── trademark-filings/
│   ├── nda-template.md
│   └── certificate-disclaimer.md
├── business/                        ← Business development
│   ├── pricing-model.md
│   ├── target-clients.md
│   └── advisory-board-candidates.md
└── regulatory/                      ← Regulatory engagement
    ├── faa-ai-roadmap-response.md
    └── submissions/
```

---

## Current Priorities

> Updated as we work. Top of list = next thing to do.

1. **Trademark filing** — "Safety Critical Labs" and the mark. Do not pass go.
2. **Zenodo DOI** — 10 minutes, makes v1.0 formally citable right now.
3. **Audit methodology draft** — what does Phase 3 of the assessment actually look like in practice?
4. **Logo / mark design** — needed before trademark filing on the design mark.
5. **NDA template** — needed before any external conversations about methodology.

---

*Last updated: 2025*  
*Author: K. Williams*  
*Classification: Private — Internal only*
