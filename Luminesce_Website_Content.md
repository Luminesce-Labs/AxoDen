# Luminesce Limited website content

Canonical copy for the company site at luminescelimited.com. Updated 20 October 2026 from the investor introduction of 19 October 2026 and Profile Reference v2.4 of 20 October 2026.

AxoDen is the platform in development at axoden.io. Luminesce Limited is the company. This repository is the company site.

Primary navigation: Home, Dossier, Kernel, Applications, Research, About, Contact.

`defence.html` and `forensic-intelligence.html` remain as short entry points for old URLs. They are `noindex`, and their canonical target is `applications.html`. `grid-flight-recorder.html` is a research-concept note and is omitted from the sitemap. `privacy.html` is omitted from the sitemap and disallowed in `robots.txt`.

## Homepage

### Hero

Computational assurance for decisions that have to be examined.

Luminesce Limited · Guildford, UK · founded 2023

Luminesce Limited develops AxoDen. AxoDen examines whether the evidence and assumptions behind a decision still hold, and what should follow when they fail.

The programme has two engineering strands: a computational assurance harness around AI, and modular software for supplier-evidence review, digital forensics and RF-to-AI middleware. Dossier Intelligence is the current commercial focus.

AxoDen, the platform, is in development at axoden.io. This website is the company, Luminesce Limited.

Primary call to action: Read Dossier Intelligence

Secondary call to action: See the kernel

### Founder card

Erkan Yalcinkaya

Founder and Principal Systems Architect. Engineering physicist.

### Evidence strip

2023: Luminesce founded

Jan 2026: full-time on AxoDen

4: experts evaluating the Dossier MVP

23: Zenodo records on 19 Oct 2026

ORCID: 0009-0008-6435-3530

The Zenodo count is 21 publications and two models. The publications include a book. Deposit is not peer review.

### The problem

Convincing output is an incomplete basis for trust.

An answer can be persuasive while the basis for relying on it stays difficult to inspect. In a consequential system, that basis decides whether the answer can justify action.

What has to be inspectable: which claims have support; which assumptions carry the conclusion; where the knowledge has contradictions or gaps; what should happen when that support changes.

AxoDen specifies an explainable assurance harness: evidence, reasoning structure and the conditions governing action become objects that can be examined, checked and recorded. Its scope is the represented evidence and control structure. Recovering a model's hidden internal reasoning is a separate problem.

### What is built

Selected methods and controls are carried into a maths and assurance kernel, a graph layer and domain applications. Each application keeps its own implementation and evaluation status.

- Kernel: evidence identity, ordered decision gates, session-bound checks, domain profiles, append-only records and replay. Coverage is narrower than the full research operator set.
- Applications: supplier-evidence review, a forensic intelligence prototype, and Spectrum Bridge, pilot-stage RF-to-AI middleware.
- Dossier Intelligence: the current commercial focus. Supplier-evidence review for quality and compliance teams in aerospace and defence.

### Where the work stands

Expert evaluation. Four subject-matter experts at a prospective defence and aerospace manufacturer are evaluating the Dossier Intelligence MVP. A contract and a formal pilot remain to be established.

Erkan Yalcinkaya founded Luminesce and has worked on it full-time since January 2026. The enterprise record runs through Unilever, Accenture, Infosys, GSK, Virgin Media O2 and Fresenius.

Dates kept separate: Luminesce dates from 2023. The mathematical work began in early 2024. Full-time work on Luminesce began in January 2026.

### Evidence handling

Engagements can involve sensitive technical, commercial, regulated or security-relevant evidence. Work can begin under NDA. Engagement data stays in the agreed working environment. Closeout should state what was received, what was produced, what must be returned or deleted, and which claims still depend on source review, integration testing or external validation.

### Contact

Discuss a defined Dossier trial.

The next commercial step is a defined trial: representative evidence, a trial sponsor, a purchasing decision-maker and acceptance criteria covering review quality, reviewer effort, traceability, failure cases and integration.

Forensic intelligence and Spectrum Bridge can be discussed as evaluation settings, each inside its recorded scope.

Email: contact@luminescelimited.com

Founder: yalcinkaya@luminescelimited.com

LinkedIn: linkedin.com/in/eyk

Platform: axoden.io

Location: Guildford, Surrey, United Kingdom.

## Dossier Intelligence

Supplier-evidence review for aerospace and defence.

Dossier Intelligence connects suppliers and parts to qualification requirements and supporting documents. The intended value is a traceable basis for review, with less avoidable manual investigation.

Expert evaluation. Four subject-matter experts at a prospective defence and aerospace manufacturer are evaluating the MVP, as reported in October 2026. A contract and a formal pilot remain to be established. The manufacturer is unnamed on the public site.

### What a reviewer can inspect

The backend keeps source evidence, accepted records, review decisions and audit runs distinct.

- Immutable evidence intake, deterministic CSV mapping, field-level provenance.
- Human review and promotion, frozen audit runs, PostgreSQL persistence and durable jobs.
- Versioned Neo4j projections. Linked supplier, part, requirement and document views. Provenance, support, contradiction and dependency through the domain schema.

### Why the relationships matter

Consider an expired supplier document. It supported a qualification claim relevant to a part. That claim helped satisfy a requirement. A reviewer relied on its validity. The useful question goes past the expired file: which claims and decisions depended on it, and does other current evidence still support them?

Current software provides evidence intake, provenance, review records, frozen audit runs and graph projections. Implementing and validating the automatic path from expiry to a revised decision is further work, together with general document extraction, production connectors and measured operating capacity.

### From expert evaluation to a defined trial

Agree representative evidence, a trial sponsor, a purchasing decision-maker and acceptance criteria. Assess review quality, reviewer effort, traceability, failure cases and integration needs. Pricing and repeatable customer value remain to be established.

## Kernel

A control core for evidence and recorded decisions.

The shared kernel implements evidence identity, ordered decision gates, session-bound checks, configurable domain profiles, append-only records and replay mechanisms for inspecting recorded decisions. Domain applications supply ingestion, domain logic, interfaces and human review.

The software architecture shows where broader mathematical operators and verification contracts can enter. The current kernel covers a narrower set. Attestation-record verification, Goodhart detection and the full research operator set sit outside the current kernel. The Attested Epistemic Integrity Plane specifies the composed assurance architecture. Implementation and deployment validation of that complete runtime plane remain outstanding.

The graph layer represents provenance, support, contradiction and dependency through domain schemas and queries. How far the same runtime is reused across domains still needs evaluation.

APASES is the research environment. The research documents specify concepts and results. The kernel enforces selected controls. Domain applications supply operational workflows.

## Applications

Three applications, three evaluation states.

Supplier documents, security events and RF-derived inputs mean different things in their own domains. Support, dependence, provenance, contradiction and freshness recur across them.

On this page, pilot-stage means internal development short of production. That is a separate state from a contracted customer pilot.

### Dossier Intelligence

Supplier-evidence review for aerospace and defence. The MVP is in expert evaluation by four subject-matter experts. A contract and a formal pilot remain to be established.

### Forensic intelligence

The prototype ingests evidence and constructs and analyses graphs linking events, processes, systems and investigative claims. Selected kernel controls govern admission and recorded outcomes.

Testing has included Mordor adversary-emulation telemetry and confidential alert data supplied under non-disclosure agreements. These are distinct test sources. The provider of the confidential data is unnamed. Operational deployment and customer benefit require an evaluation of this application on its own.

### Spectrum Bridge

Pilot-stage assurance middleware between RF-derived inputs and an onboard edge AI computer. It applies declared admission and refusal rules to control what reaches the AI, and records the inputs, checks and decisions in an append-only evidence ledger for audit and replay. Session-bound controls address the risk of recovered communications or persisted instructions being treated as sufficient current authority.

Recorded local verification covers replay and shared-kernel compatibility within a defined host, profile and fixture scope. Calibrated physical performance, operational session management and enforcement through the complete action path remain integration and evaluation work.

The priorities beyond the current applications are a defined Dossier trial, broader operator coverage, application integration and composed assurance-architecture validation, including the outstanding evaluator-independence and data-provenance obligations.

## Research

Research that states what can be checked.

The research asks how a system can represent the basis for a conclusion, identify weaknesses in that basis, and govern the consequences. The public deposit records the work. It does not, by itself, establish peer review or the proof status of any single result.

Zenodo author-search facets checked on 19 October 2026: 23 records, comprising 21 publications and two models. The publication category includes the book. Mathematical work began in early 2024.

| Research area | Question | Methods |
|---|---|---|
| Reasoning and verification | Which structural claims about reasoning can be checked independently? | Topology of Reasoning; certificate and verifier architecture |
| Assumptions and structural risk | What supports reasoning, where is it vulnerable, and what follows when support fails? | Reflexive Epistemic Fabric |
| Knowledge structure and discovery | What is missing, contradictory or outdated? Does the knowledge model need revision? | Epistemic Fabric; structural gaps, evidence decay and schema analysis |
| Objectives and metric integrity | Does a measure still represent its intended objective? | Goodhart-collapse detection and classification. Masking and confounding remain open. |
| Information bounds and composition | How do local uncertainty and model-influence limits combine across a pipeline? | Entropy-Bounded Data Pipelines; Entropy-Frugal Intelligence |
| Independence and execution trust | Can safeguards share a failure source? What evidence supports their separation? | Coprime-Factor Security; ASIL-M multi-root attestation |
| Execution assurance | How should evidence, policy and current authority govern action and recovery? | Monitoring Quad; Admission Resilience Validator; action contracts and session-bound controls |

A method in that table is a research position. Software coverage is stated on the kernel and application pages.

The classical global composition theorem for Entropy-Bounded Data Pipelines has a machine-checked proof in Lean 4 with Mathlib, for finite discrete variables. It establishes the stated composition bound inside that scope. Entropy-Frugal Intelligence composition remains an analytical argument under functional-stage and model-state independence assumptions.

The graph-based contributions share the AxoDen Evidence Graph. Geometry of Epistemic Integrity treats reasoning structure, live assumptions and knowledge over time as connected views of that graph. The Attested Epistemic Integrity Plane specifies how independence, attestation, reasoning structure, live assumptions and proxy validity come together around a decision. Implementation of the complete runtime plane remains outstanding.

APASES connects task routing, source retrieval, methodology selection, tool access, computation, counterexample search, verification and claim records. On this site it appears only as that internal research environment.

Grid Flight Recorder, paper 203, is a research concept for replayable evidence around cyber-physical control events.

A theorem, paper or benchmark can support a pilot hypothesis. It still has to be translated into a scoped question, a dataset, an acceptance test and a decision about weak evidence.

Useful links: ORCID `https://orcid.org/0009-0008-6435-3530`; Zenodo search for that ORCID; kernel page; contact.

## About

Erkan Yalcinkaya is an engineering physicist and systems architect. At Luminesce he originates the research, designs the architecture and builds the AxoDen software.

The work connects a computational assurance harness around AI with modular applications for supplier-evidence review, forensic intelligence and RF-to-AI admission. Dossier Intelligence is in expert evaluation and is the current commercial focus. The complete assurance plane remains an architecture, with implementation and validation still outstanding.

Luminesce Limited is the company, at luminescelimited.com. AxoDen is the platform in development at axoden.io.

Luminesce dates from 2023. Erkan has worked on it full-time since January 2026. Essays on cognition and reasoning were written in 2023 and published in 2024 as *In the Labyrinth of a Curious Mind*. The mathematical work began in early 2024, after that manuscript was finished.

Education: Engineering Physics, Istanbul Technical University. Base: Guildford, Surrey.

### Delivery record

These are career facts. The acquisition value and the programme value are the environments he worked in. They are separate from the budget he controlled.

- GSK: led technical integration planning and delivery for a £9 billion acquisition. Migrated 200 TB+ of GxP-regulated data. The £9 billion figure is the acquisition value.
- Virgin Media O2: owned the data workstream of a £200 million transformation and joint venture, directing an 85-person organisation against an £8 million annual budget.
- Fresenius: led IT separation workstreams for a €250 million pharmaceutical carve-out across four countries, owning the TSA framework and the cutover controls.
- Unilever: designed and wrote the Türkiye mobile sales and distribution system, later customised for 17 further countries. Virtual warehousing is recorded with lower fleet investment, and a global best-practice award is recorded.
- The same career includes architecture and delivery work at Accenture and Infosys.

The company priority is to turn the Dossier Intelligence expert evaluation into a defined customer trial, and to keep developing the shared components that can support further applications.

## Grid Flight Recorder

Grid Flight Recorder is a concept for replayable evidence around cyber-physical control events, recorded as paper 203. Its recorded status is a research concept.

The AxoDen applications in current development are Dossier Intelligence, forensic intelligence and Spectrum Bridge.

## Privacy

Luminesce Limited is a UK company developing AxoDen, a computational assurance platform. This website is the company site. The platform is at axoden.io.

Enquiry data may include name, email address, organisation, role, message content and any files or context the sender chooses to provide. It is used to respond, assess whether Luminesce can help, provide requested information and manage a potential or active working relationship.

Luminesce does not sell personal data. Information may be shared with professional advisers, service providers or authorities where needed for lawful business operation or legal compliance.

Engagement-specific material is handled under the agreed NDA, scope and working environment. Closeout should identify what was received, what was produced, and whether engagement data should be retained, returned or deleted.

Enquiry and client information is kept only for as long as needed for the purpose collected, legitimate business records or legal obligations. Access, correction and deletion requests are handled subject to applicable law and any lawful retention requirements.

Privacy contact: contact@luminescelimited.com

Last updated: 20 October 2026.

## Footer

Luminesce Limited develops AxoDen. The platform is at axoden.io.

## Claims kept off these pages

Customer name. Owner-reported test-case counts. Salary and day rate. Phone number. Availability for hire. Test-suite counts that lack a current primary-source check. Theorem totals from the May 2026 website register. SEM DEFENDER. A closed defence threat register. Jam-tolerant flight, mission control, or refusal-capable autonomy as a product description. GxP or pharma as a current Dossier wedge. APASES as a service sold to clients. Grid Flight Recorder as a pilot offer. Automatic expiry-to-decision reassessment as a built feature.
