## EvidenceOS

**Building the operating system for sovereign health intelligence.**

We automate the production of trustworthy clinical evidence for health AI systems — evaluation, safety, and governance infrastructure with mathematical assurances. Starting with neurodiagnostic AI (TBI first vertical), expanding to every domain where clinical AI needs to prove it works before it deploys.

> *"82% of clinicians know about TBI blood biomarkers. 6% use them. The gap isn't science — it's evidence infrastructure."*

---

### Methodology — What We Contribute

Open-source research packages powering clinical validation intelligence. Built on evidence from [$165M+ of publicly funded research](https://fitbir.nih.gov/) (TRACK-TBI, CENTER-TBI, InTBIR).

| Package | What It Does | Language |
|---------|-------------|----------|
| [evidenceos-multiverse](https://github.com/evidenceos-research/evidenceos-multiverse) | 12-axis specification curve analysis — systematically tests model robustness across thousands of defensible analytical choices | Python |
| [evidenceos-conformal](https://github.com/evidenceos-research/evidenceos-conformal) | Distribution-free prediction intervals (MondrianCQR) — models know when they don't know | Python |
| [evidenceos-knowledge](https://github.com/evidenceos-research/evidenceos-knowledge) | Knowledge graph reasoning (GraphRAG + DGCI) — explainable clinical evidence synthesis | Python |
| [evidenceos-tabular](https://github.com/evidenceos-research/evidenceos-tabular) | Clinical prediction model pipeline — loading, harmonization, and feature engineering for TBI datasets | Python |
| [evidenceos-ontology](https://github.com/evidenceos-research/evidenceos-ontology) | NINDS TBI Common Data Elements — 13 machine-readable YAML schemas (7,780 lines) | YAML |
| [evidenceos-acquisition](https://github.com/evidenceos-research/evidenceos-acquisition) | Evidence acquisition pipeline — automated search, screening, and knowledge graph construction | Python |
| [evidenceos-trajectories](https://github.com/evidenceos-research/evidenceos-trajectories) | Neural ODE biomarker trajectory modeling — temporal disease progression | Python |
| [evidenceos-living-review](https://github.com/evidenceos-research/evidenceos-living-review) | Living systematic review automation — continuous evidence synthesis | Python |
| [evidenceos-bench](https://github.com/evidenceos-research/evidenceos-bench) | Clinical AI benchmark suite — TRIPOD+AI compliance and model comparison | Python |

All 10 packages: [**evidenceos-research**](https://github.com/EvidenceOS/evidenceos-research) (Apache-2.0)

**Methodological foundations:** Specification curve analysis ([Simonsohn et al. 2020](https://doi.org/10.1038/s41562-020-0912-z)), conformal prediction ([Vovk et al. 2005](https://doi.org/10.1007/b106715)), TRIPOD+AI ([Collins et al. 2024](https://doi.org/10.1136/bmj-2023-078378)), Riley sample size criteria ([Riley et al. 2020](https://doi.org/10.1136/bmj.m441)).

---

### Ecosystem — How It Fits Together

Four integrated product families, one evidence foundation. Each product draws from the same Canonical Evidence Library (CEL) — versioned, DOI-addressable analytical artifacts that serve as the evidentiary ground truth.

```
                         ┌─────────────────────────┐
                         │   Evidence Foundation    │
                         │  (CEL + Knowledge Graph  │
                         │   + Ontology + LSRs)     │
                         └────────┬────────────────┘
                                  │
            ┌─────────────────────┼─────────────────────┐
            │                     │                     │
   ┌────────▼────────┐  ┌────────▼────────┐  ┌────────▼────────┐
   │ Clinic-in-a-Box │  │  Lab-in-a-Box   │  │University-in-Box│
   │                 │  │                 │  │                 │
   │ BRIDGE-TBI      │  │ Research-as-a-  │  │ RAIGH Academy   │
   │ Aya Clinician   │  │ Service         │  │ AI workforce    │
   │ TeleCare Africa │  │ Evidence        │  │ development for │
   │                 │  │ Capsules        │  │ global health   │
   │ For: Clinicians │  │ For: Researchers│  │ For: Universities│
   └─────────────────┘  └─────────────────┘  └─────────────────┘
                                  │
                         ┌────────▼────────┐
                         │AIDA Infrastructure│
                         │                 │
                         │ Sovereign data   │
                         │ for governments  │
                         │                 │
                         │ For: Ministries  │
                         │ of Health        │
                         └─────────────────┘
```

**Current focus:** TBI (first vertical). The methodology is domain-agnostic — each new clinical domain requires a domain ontology + constraints + domain experts, not new infrastructure. Expansion roadmap: Sepsis → Cardiovascular → Stroke → Surgical Risk.

---

### Open Resources

Community assets for the health AI ecosystem:

| Resource | Description |
|----------|-------------|
| [awesome-health-ai-skills](https://github.com/EvidenceOS/awesome-health-ai-skills) | 17 executable health AI skills organized in 7 bundles — the Elements of Health AI |
| [awesome-health-ai-regulations](https://github.com/EvidenceOS/awesome-health-ai-regulations) | Global regulatory frameworks (FDA, EU AI Act, Africa, Asia-Pacific) with structured JSON data |
| [awesome-clinical-prediction-models](https://github.com/EvidenceOS/awesome-clinical-prediction-models) | Living registry of clinical prediction models with YAML-structured evaluations |
| [awesome-ai-evaluation-metrics](https://github.com/EvidenceOS/awesome-ai-evaluation-metrics) | Cross-modality evaluation taxonomy for health AI systems |

**SDG Alignment:** SDG 3 (Good Health — Targets 3.4, 3.8, 3.d) · SDG 4 (Quality Education — Target 4.4) · SDG 9 (Innovation — Target 9.5) · SDG 17 (Partnerships — Target 17.6)

---

### Governance & Trust

EvidenceOS operates through four legal entities with distinct roles — separating commercial product development from independent evidence production and open-source stewardship:

| Entity | Role | Jurisdiction |
|--------|------|-------------|
| **EvidenceOS Inc.** | Product company, IP holder | US (Delaware) |
| **EvidenceOS OÜ** | EU operations, CE Mark pathway | Estonia |
| **CEAIH** | Independent evidence production institute, grant applicant (NIH, Gates, Wellcome) | US nonprofit |
| **PAATHI** | Open-source stewardship, LMIC access, continental AI governance | Rwanda (CLG) |

**Data policy:** This organization contains NO real patient data. All included data is synthetically generated. Real patient data is handled in separate, sovereign environments compliant with HIPAA, GDPR, and national data laws. See [DATA_POLICY.md](https://github.com/EvidenceOS/evidenceos-research/blob/main/DATA_POLICY.md) for details.

**Licensing:** Research packages are Apache-2.0. Awesome-lists are CC-BY-4.0. Platform code follows dual licensing — see individual repo LICENSE files.

---

### Get Involved

<table>
<tr>
<td width="50%">

**Researchers & Academics**
- Run a [multiverse analysis](https://github.com/EvidenceOS/evidenceos-research) on your clinical dataset
- Contribute to our [ontology schemas](https://github.com/evidenceos-research/evidenceos-ontology)
- Cite our packages: see CITATION.cff in each repo

</td>
<td width="50%">

**Clinicians & Health Systems**
- Explore [BRIDGE-TBI](https://github.com/EvidenceOS/evidenceos-health-platform) clinical decision support
- Review our [regulatory tracker](https://github.com/EvidenceOS/awesome-health-ai-regulations)
- Contact: clinical@evidenceos.com

</td>
</tr>
<tr>
<td width="50%">

**Governments & Development Partners**
- See our [health AI governance frameworks](https://github.com/EvidenceOS/awesome-health-ai-regulations)
- Review [digital public infrastructure](https://github.com/EvidenceOS/awesome-dpi-infrastructure) resources
- Contact: partnerships@evidenceos.com

</td>
<td width="50%">

**Builders & Contributors**
- Check [good first issues](https://github.com/EvidenceOS/evidenceos-research/labels/good%20first%20issue) across our repos
- Read our [Contributing Guide](https://github.com/EvidenceOS/evidenceos-research/blob/main/CONTRIBUTING.md)
- All PRs welcome — we review within 48 hours

</td>
</tr>
</table>

---

<p align="center">
  <a href="https://evidenceos.com">Website</a> ·
  <a href="https://github.com/EvidenceOS/evidenceos-research">Research Packages</a> ·
  <a href="https://github.com/EvidenceOS/evidenceos-health-platform">Platform</a> ·
  <a href="mailto:hello@evidenceos.com">Contact</a>
</p>

<p align="center">
  <sub>Apache-2.0 · Built in Delaware, Turku, Kigali, and everywhere clinical AI needs to prove it works.</sub>
</p>
