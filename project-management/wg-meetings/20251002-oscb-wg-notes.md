
# External Webinar - Open Science and Capacity Building Working Group  

**Date:** October 2nd, 2025


## 🗣️Welcome!

#### Introduction 

**Host:** Nyasita Ondari (Precious + Michael)

00:05 - 00:06 [⏰ 1min]  Welcoming note

***
We have a code of conduct - [https://aphrc-dswb.github.io/dswb-open-science-capacity-wg/coc](https://aphrc-dswb.github.io/dswb-open-science-capacity-wg/coc)

       * If you experience or witness unacceptable behaviour, or have any other concerns, please report it by contacting the organisers - Nyasita, and Precious. (osponow.dswb@gmail.com).

This call is being recorded.

       * The video may be shared with others
       * Turn on your webcam if you don't mind sharing your face (or off if you do)

All notes will be taken in Framapad and archived on the public DSWB GitHub, including your name and response. You may use a pseudonym or add an emoji 🤫 if you don’t want to be included. To request removal, email precious@osponow.com or osponow.dswb@gmail.com

AI notetakers will also be removed from the call for privacy and safety reasons. You will get the recording and the notes of this session after the call.

## 👋 Icebreaker

**Name (or pseudonym or emoji) / One value you think is most important in data sharing (e.g., trust, equity, speed, access)/ One thing you hope to learn or take away from this session?**

   * P Karega / Trust/data sharing policies 
   * Moctar/
   * Precious/ Safety
   * James: speed
   * Shamim/Access/Ethics aspect 
   * David Amadi: Balance between technical requirement and community rights /trust/equity
   * Ahmed Unshur / trust
   * Ousmane /
   * Maureen/ Trust/ Access
   * Gabi / as open as possible \& as closed as necessary
  
## 📣 Agenda
**00:15 - 00:55: [⏰ 40min]**

## 🖥 Presentation - Dr Gabriele Rinck

**Speaker Bio**

Dr Gabriele Rinck worked on a molecular epidemiology study on drug-resistant HIV, at Public Health 
England early in her career, after a PhD in virology. After a decade in the molecular diagnostics industry, 
leading the development of diagnostics and coordinating testing services for clinical trials, she joined the Wellcome Sanger Institute, 
where she managed a UK-wide genomics study focused on prenatal diagnosis of rare diseases. Since 2020, she has been at EMBL-EBI, 
initially as part of the European Nucleotide Archive (ENA) team. Her role revolved around COVID-19-related cohort data and 
integrating multi-omics datasets. Last year, she transitioned to the European Genome-phenome Archive (EGA) team, as Project Lead for federated EGA.

**Notes:**

   * Data Integration
     * EMC Pilot Data
     * Viral Data
     * Antibody, Profiles, B-cell \& T-cell data
     * Other human data
   * A cohort browser is used to give metadata about the various cohorts within a pilot study
   * BioSamples archives are used to navigate linked data
       * It lists the data points for a patient
       * Relevant data for the cohorts
   * **Contagio - a tool**
       * Establishing a cohort warmbase for a quick response to future outbreaks.
       * WP1: Cohort Preparedness Platform
       * WP2: Harmonized approach to data collection and analysis
       * WP3: Ethics, legal, regulatory, and governance
       * WP4: Virtual Biorepository
           * Establish a sustainable and equitable grass-roots system for the timely sharing of specimens for future outbreaks
           * Access to more representative samples that reflect global diversity, with a focus on populations from low and middle-income countries
           * Represent a distributed system with local management of specimens, following common standards of quality and equitable accessibility
   * **European Genome-phenome Archive (EGA) manages sensitive human data**
       * It was first established in 2008
       * Mission: Permanent archiving and sharing of personally identifiable genetic, phenotypic, and clinical data generated for the purposes of biomedical research projects or in the context of research-focused healthcare systems. Drive development of and implement community standards for supporting FAIR data sharing
       * Federated EGA - European by name, Global by nature
           * 9 national nodes
           * 5 nodes with data available
           * 50 datasets
               * Cancer
               * Autoimmune
               * Development
               * Synthetic
           * 5 more nodes preparing to join
   * **Flexible Model - Accommodating National Requirements**
       * To ensure compliance with national regulations/legislation each FEGA node is responsible for establishing:
           * The appropriate governance and legal frameworks,
           * ﻿﻿Data protection policies,
           * ﻿﻿Necessary legal agreements, signed by the relevant parties (e.g. Data Processing Agreements for data submissions).
       * Additional variability in node operations may also depend on aspects such as:
           * ﻿﻿Existing infrastructure/processes (e.g. availability of TRE),
           * ﻿﻿Funding \& sustainability model,
           * ﻿﻿Central vs federated system within the country
       * Federated EGA - Node Types
           * Central EGA Nodes - Committed Globally
               * ﻿﻿Hosts data
               * ﻿﻿Facilitates global discovery of shared metadata
               * ﻿﻿Accepts data from all around the world
               * ﻿﻿Has helpdesk
           * Federated EGA Node - Committed Locally
               * Hosts and/or owns data
               * ﻿﻿Shares metadata to allow global discovery
               * ﻿﻿Accepts 3rd party data from jurisdiction
               * ﻿﻿Has Helpdesk been responsible for own data/jusridiction
           * Community Node - Committed to a project
               * Hosts/owns data
               * ﻿﻿Shares metadata to allow global discovery
               * ﻿﻿Doesn't accept 3a party data
               * ﻿﻿Minimal Helpdesk (distribution only)
           * Conversations are ongoing to set up an African Community Node within the FEGA network
  **Questions (Open to the audience)**
   * How do you navigate the governance aspect and consideration of the sensitivity of the data?
       * I think I have answered this question after my talk; please get in touch if you have any additional questions
   * Does the EGA network support a different type of data apart from genomic data for instance population health data
       * we are aiming to support any sensitive human data, this could be phenotypic, clinical, epidemiological data; this could also be population health data, some of the FEGA datasets are in the area for population genetics. 
   * What is the underlying software architecture supporting this Federated EGA
       * you can find further information about the technical details here: [https://ega-archive.github.io/FEGA-onboarding/topics/technical-operational/](https://ega-archive.github.io/FEGA-onboarding/topics/technical-operational/)
   * Will EGA be able to support linking data with other environmental data; meteorological data, satellite data and the likes?
       * Great question, yes, there have been discussions in the context of exposome research. We have the FEGA-Connect Project which is looking at linking FEGA records to other non-genomic data types (but currently mainly proteomics or similar). One of our onboarding FEGA node is also looking into linking to exposome data (like metabolites). We are also working on a new metadata model which should make linking to other data types easier
   * Also, inetersting comment on the establishmnt of Trusted Research Environments to allow data access. Are there any functional within the partners you have so far, and how are you finding their use in the regions?
       * A number of FEGA nodes are planning to set up TREs, especially those involved in the GDI project, the Finnish node gave a short demo earlier this year \& the new Suisse node are also progressing with setting up their TRE. But it's not fully operational yet, to my knowledge
   * Any in the GS countries?
       * We are looking at TRE in the context of federated EGA, so far we don't have any GS nodes yet, unfortunately
   * How can an organisation apply to participate in the data discovery and compute network?
       * Any organisation can submit data to EGA (human data) or ENA (non-human sequences), then your data will be discoverable through our archives. Also any organisation can access data on ENA which is an open archive - data can just be downloaded; for accessing EGA/FEGA data you would have to apply for access (explain what you're planning to do with the data etc, by completing a data request form) \& the data provider (ie their data access committee will review \& decide about the access). In terms of analysis compute, if its about pathogen (non-human) data you could request a Data Hub from the ENA Pathogens team, where you could share data privately with your collaborators and run some analysis.
   * How an institution with genomic data can join your network and may be sharing data ?
       * An institution that already has their own data hub (for sharing data) could join FEGA as a community node, for example. Metadata would be made discoverable through the central catalogue for greater findability \& the sharing would be managed through the local hub (Community Node). There is an onboarding process make sure it's all set up correctly.

**00:55 - 01:30: [⏰ 40min]**

## 🖥 Presentation - Dr Sumir Panji

**Speaker Bio**

Dr Sumir Panji is the Program Manager of the eLwazi Open Data Science Platform and the
H3Africa Bioinformatics Network, with a strong background in bioinformatics and data science.
Holding a PhD in Bioinformatics, Sumir has been instrumental in the planning, development,
and implementation of significant research programs focused on building human and
computational infrastructure, capacity, resources, and tools for bioinformatics, genomics, and
data science within Africa.

**Notes:**

   * **HABioNet and summary of H3Africa Data**
       * H3ABioNet: Pan African Bioinformatics Network to develop bioinformatics capacity in Africa and support the H3Africa research projects. It has a presence in 28 institutions, and 16 African countries.
       * Types of datasets collected:
           * Phenotype data (associated with genotype data)
           * Genetic Variation data human and pathogen
           * Genotyping chip array data
           * Microbiome sequence data
   * **FAIR: Findable, Accessible, Interoperable, Re-usable**
   * **Origins and definitions of FAIR**
       * It has long been recognised that it is not sufficient simply to post data and other research-related materials onto the web and hope that the motivation and skill of the potential user would be sufficient to enable reuse.
       * Primary Recommendations and Actions
           * Step 1: Define and apply FAIR appropriately
       * Why is FAIR Important?
           * It saves time, and provides a variety of resources that reseachers can make use of.
       * FAIR guiding principles - DATA Centric
           * Findability
           * Accessibility
           * Interoperability
           * Reproducability
   * **Conclusions**
       * ﻿﻿Limiting factor in genomics is not data generation, increasingly multi-dimensional data - data analysis O and interpretation are bottlenecks
       * ﻿﻿To apply tools and techniques such as ML, well labelled data is required
       * ﻿﻿Curation of data / good dataset stewardship is essential towards adding value for data to enable findability and re-usability
       * ﻿﻿The FAIR landscape has changed from policy discussion to implementation with better metrics and tools now available for assessing FAIR-ness of different resources and infrastructures
       * ﻿﻿Better understanding and guidance on implementing FAIR and its metrics for a range of outputs now
       * available
       * Skills and knowledge on FAIR gained within HABioNet over this period - moving from making outputs
       * FAIR to now creating "born-FAIR" outputs
       * ﻿﻿Knowledge, skills and experience gained being applied within other African data health research projects e.g. eLwazi Open Data Science Platform ([https://elwazi.org/)](https://elwazi.org/)), as part of the The Data Science for Health Discovery and Innovation in Africa (DS-I Africa) Initiative (httos://dsi-africa.ora/
    
  ### PART 2

   * **NIH DS-I Africa**
       * Harnessing Data Science for Health Discovery and Innovation in Africa
           * Research Hubs: Advance and demonstrate feasibility of data science research and innovation to improve health in Africa Training: Increase capacity for data science research in Africa
           * ELSI Research: Explore Ethical, Legal, and Social Implications of data science research from an African perspective and contribute to policy discussion on the continent
           * Open Data Science Platform \& Coordination Center: Facilitate the development of a trans-African network of data scientists
   * **eLwazi**
       * Aim: To develop an African Open Data Science Platform and associated resources, to support the Harnessing Data Science for Health Discovery and Innovation in Africa (DS-I Africa) consortium and beyond
       * The solution needs to be feasible in the African context
           * Aims to be a flexible, scalable platform enabling the implementation of data science for health, that is relevant to the African
       * FAIRPlus Data Set Maturity Model:  [https://fairplus.github.io/Data-Maturity](https://fairplus.github.io/Data-Maturity)
           * 5 - Managed Data Assets: Enterprise Level. Data at this level is optimally managed at the most granular level in an environment offering data governance, master data management and reference data management capabilities.
           * 4 - Semantically Typed Data: Cross-community Level. This level focuses on cross-domain interoperability and is meant to be the level required for larger harmonization and integration projects
           * 3 - Standardised Data: Community Level. Data at this level complies with community standard domain models, terminologies and formats, and is hosted in an environment offering searching and retrieval capabilities.
           * 2- Described Data: Project Level. All datasets generated within a project are consistently described against a locally defined schema, controlled terminologies, and hosted in an environment offering data catalogue level searching
           * 1 - Identifiable Data: Data Object level. Data at this level is identifiable as individual generic data objects and described by generic metadata elements. Hosting environment offers limited retrieval capabilities.
           * 0 - Single Use Data: No potential for re-use beyond lifetime of the research project

**00:55-00:60[⏰ 5min] Closing remarks**

  * We had an external webinar session on Visual Architecture for Research Communication: Making Complex Studies Crystal Clear. 
More details can be found [here](https://github.com/aphrc-dswb/dswb-open-science-capacity-wg/blob/main/project-management/wg-meetings/20250918-oscb-wg-notes.md).
