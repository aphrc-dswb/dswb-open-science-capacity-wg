## Welcome to Journal Club - Led by Fikregabriel Aberra (PhD), AHRI Team!

Date: April 1st, 2026

**Attendees:**
   * Laurah
   * Yordanos
   * Fikregabrail
   * Miranda
   * Domian
   * Precious
   * David
   * Belayneh
   * Brenda B.
   * Reinpeter
   * Cyrille
   * Abdoulaye
   * Daffe
   * Joshua M.
   * Ousmane
   * Sington
     
**Apologies**

   * N/A

## Notes

Journal Club Material:

**Title:** *WorkflowHub: a registry for computational workflows* 

**Citation:** Gustafsson OJR et al., *Scientific Data* 12, 837 (2025). [https://doi.org/10.1038/s41597-025-04786-3](https://doi.org/10.1038/s41597-025-04786-3)

**Technical Stack:** 

   * FAIRDOM-SEEK Platform
       * Built on FAIRDOM-SEEK, a data-management platform generalised from systems biology. Hosted on University of Manchester Research IT cloud infrastructure.
   * RO-Crate Standard
       * Research Object Crate is the primary exchange format, auto-built on registration. Packages workflow + test data + diagrams + publications + SOPs as a FAIR Digital Object.
   * GA4GH TRS API
       * GA4GH Tools Registry Service API enables Galaxy, Sapporo, and WfExS to search, retrieve, and execute workflows directly from WorkflowHub without custom integration.
   * Bioschemas + EDAM
       * Three Bioschemas profiles (Computational Tool, ComputationalWorkflow, FormalParameter) combined with EDAM ontology for Topics \& Operations. Abstract CWL captures semantic annotations.
   * LS-Login / OAuth2
       * EOSC federated Authentication via Life Science Login + OAuth2. Supports GitHub, Google, Apple, ORCID, and institutional single sign-on. Enables cross-platform user identity.
   * DataCite DOl Minting
       * Persistent DOls minted per workflow version via DataCite. CITATION.cff parsed to auto-populate creator/ORCID metadata.
       * Workflows linked to the DataCite PID Knowledge Graph.

**The WorkflowHub Stats:**

   * 860+ workflows registered
   * 958 registered users
   * 266 organisations adopted
   * 36 countries
   * **Key use cases:**
       * 67 COVID-19 workflows for ongoing SARS-CoV-2 intra-host variation analysis
       * BGE (Biodiversity Genomics Europe) - consortium genomics pipelines across institutes
       * VGP (Vertebrate Genomes Project) - large-scale assembly workflow registry
       * Australian BioCommons — adopted WorkflowHub as its national workflow registry
   * **Platforms, services, and standards that are used by, or integrate with, WorkflowHub**
       * GitHub/GitLab
       * bio.tools
       * Common Workflow Language
   * **What WorkflowHub Brings to the Field**
       * Domain-Agnostic Registry: First unified registry for any workflow type, language, or scientific domain. Life sciences, earth sciences, engineering, and climate science — all accepted irrespective of workflow maturity.
       * Workflow-RO-Crate Profile: Novel Workflow-RO-Crate profile packages workflows with metadata, diagrams, test data, SOPs, and publications as machine-readable FAIR Digital Objects exportable to Zenodo and other platforms.
       * Persistent Credit \& DOls: One-click DataCite DOl minting per workflow version with ORCID-linked authorship and CITATION.cff auto-import. WorkflowHub citations already appear in peer-reviewed publications (e.g. GigaScience).
       * Community Governance: Open fortnightly WorkflowHub Club meetings. 60+ contributors from ELIXIR, WCI, and Australian BioCommons. Open roadmap and GitHub-managed documentation that evolves with community needs.
       * Full Life-Cycle Hub: Integrates GitHub/GitLab (development), LifeMonitor (Cl testing), Zenodo (archival), and Galaxy/Sapporo/WfExS (execution) into a single registry spanning the entire workflow lifecycle.
       * FAIR-by-Design Wizard: Step-by-step registration wizard enforces FAIR best practices: bio.tools identifiers, EDAM ontology annotations, license selection, version history, and granular contributor attribution.
   * **Strengths:**
       * Open \& Inclusive Design: Accepts all workflow types, maturity levels, and domains. Work-in-progress workflows are explicitly encouraged. No barriers to contribution regardless of WMS, programming language, or domain expertise.
       * Standards-Driven Interoperability: Uses internationally recognised open standards: RO-Crate, Bioschemas, EDAM, GA4GH TRS, and FAIR Signposting. Avoids proprietary lock-in and supports machine actionability as required by FAIR principles.
       * Validated at Scale with Real Use Cases: Adoption demonstrated through EOSC-Life, Biodiversity Genomics Europe, Australian BioCommons, and COVID-19 pandemic response. 860+ workflows from 266 organisations across 36 countries provides strong evidence of impact.
       * Scholarly Credit Infrastructure: Treats workflows as citable scholarly artefacts. DOl minting, ORCID integration, and CITATION.cff support mean workflow contributions are now traceable in the academic literature.
       * Sustainability \& Governance: Backed by ELIXIR (UK and Belgium nodes) and Australian BioCommons with Horizon Europe funding. End-of-life policy ensures archived RO-Crates on Zenodo with DOl persistence if the service is discontinued.
       * Community-Driven Feature Evolution: Biweekly open WorkflowHub Club drives the feature roadmap Galaxy IWC and nf-core integrations were developed in direct partnership with those communities. Setup guides co-created with major consortia.

   * **WorkflowHub User Interface:**
       * ﻿﻿﻿A workflow diagram
       * ﻿﻿﻿Parsed workflow inputs, outputs and steps for the registered
       * Galaxy workflow
       * ﻿﻿﻿Different citation format options for the workflow
       * ﻿﻿﻿Custom tags
       * ﻿﻿﻿Collections that include the current workflow entry
       * ﻿﻿﻿A button for launching the workflow on Galaxy
   * **Limitations:**
       * No Guaranteed Re-Executability - WorkflowHub is a registry, not an execution environment. Long-term re-executability depends entirely on external systems (containers, execution platforms). Registered workflows may become non-functional over time even while remaining discoverable.
       * Metadata Quality Depends on Users - Only workflow Title and Team affiliation are mandatory fields. Rich metadata features — Git integration, CITATION.cff, EDAM annotations, data linking — are optional and frequently omitted, limiting FAIR potential.
       * Life Sciences Dominance - Despite being explicitly domain-agnostic, the vast majority of contributions originate from life and health sciences. Meaningful adoption beyond bioinformatics remains limited and largely aspirational at the time of publication.
       * Scalability \& Automation Gaps - No automated Git-to-WorkflowHub synchronisation exists yet. Manual curation creates a bottleneck for large consortia. LLM-assisted metadata annotation and automated reporting are stated aspirations, not current features.
       * No Formal FAIR Metrics Benchmark - The paper describes FAIR support qualitatively. There is no large-scale quantitative benchmarking of workflow FAlRness scores before and after registration using tools such as FAIR-checker or FAIRsoft.
   * **Broader Significance for Science**
       * For Researchers: Reduces workflow reinvention. Non-experts can access best-practice analyses directly. Enables workflow discovery via standard search engines, within Galaxy's interface, and through programmatic API queries — meeting users where they already work.
       * For Publishers \& Journals: WorkflowHub citations already appear in GigaScience publications. An active publisher forum is working to establish WorkflowHub as a recommended registry for workflows in peer-reviewed literature, analogous to GenBank for sequences.
       * For Funders \& Policy: Directly addresses Open Science mandates, including the US Nelson Memo and NASA SPD-41a. Provides practical, funded infrastructure for publicly funded research to comply with data and software sharing requirements.
       * For the FAIR Movement: Provides the most comprehensive practical implementation of FAIRARS and FAIR Computational Workflows principles to date. WorkflowHub is a central platform of the FAIR Computational Workflows working group within the Workflows Community Initiative.
       * For Public Health \& Big Science: Demonstrated critical value during the COVID-19 pandemic — 67 SARS-CoV-2 workflows registered for global, ongoing intra-host variation
   * **The Workflowhub Roadmap**
       * **Near term priorities:**
           * Automated Git Synchronisation — native bidirectional sync between GitHub/GitLab releases and WorkflowHub entries, eliminating manual update burden
           * Snakemake Community Onboarding - semi-automated ingestion pipeline analogous to the existing Galaxy IWC and Nextflow nf-core integrations.
           * OpenEBench Benchmarking - integration with workflow benchmarking service to add performance and quality scores to registry entries.
           * Enhanced Search \& Faceting - improved multi-value domain/subdomain tagging (e.g., primary: biology; secondary: genomics) and smarter faceted browsing.
       * **Longer-term vision:**
           * LLM-Assisted Metadata - Al-powered annotation suggestions using Large Language Models, reviewed by creators before publication to improve metadata completeness 
           * BioConda/BioContainers Links — connect workflow registrations to containerised tool repositories for  improved dependency tracking and container reproducibility.
           * Journal Recommended Registry — active publisher forum to make WorkflowHub the preferred, peer-reviewed recommended registry for computational workflows.
           * Cross-Domain Expansion — targeted onboarding of earth sciences, physics, climate, and engineering communities to move beyond life science dominance.
       * Training: WorkflowHub being added to Software Carpentry lessons for Nextflow \& Snakemake (Edinburgh Ed-DaSH programme) and Galaxy. Training Network Smörgasbord events.

**Questions**

   * Does workflow hub actually solve the fragmentation problem, or rearranges it?  - Laurah
       * Workflowhub actually has these workflows in the system, the connection to other platforms is just an added feature.
   * How can we adopt this within the DSWB project? What are some use cases the pathfinder teams can apply it to?
       * It can be adopted to AI workflows. This is currently not available, but it can be explored.
       * The no-code platform can be hosted there, but more for visibility purposes as the Workflowhub is a registry and the program cannot be run. 
       * Some use cases would be an example of the AI workflow. 
   * Can the workflow be run separately from the metadata? 
       * The metadata is separate from the workflow. The metadata is separate data you submit with your workflow, and the workflow can be run without it.
    
## General Note

   * This is the first Journal Club of the DSWB community in 2026. Please find the previous notes for the past year and 2024, [here](https://github.com/aphrc-dswb/dswb-open-science-capacity-wg/tree/main/project-management/coworking-calls).
