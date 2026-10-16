# DSWB External Webinar - Open Science and Capacity Building Working Group  

**Webinar Topic:** Metadata standards

**Date:** 15th October 2026


### 🌍 Icebreaker question

*Name (or pseudonym or emoji) /  Organisation / One thing you hope to learn or take away from this session?*

   * Dr Erin
   * Nyasita
   * Michael
   * Precious
   * Charlotte
   * Duncan (Interpreter) 
   * Elizabeth
   * Sylvia
   * David M.
   * David Z.
   * Lauren 
   * Nyirimana
   * Rambhujun
   * Amira
   * Antidius
   * David A.
   * Ibrahim
   * Michael Y.

     

## Speaker - Dr. Erin M. Buchanan

### Speaker bio

Dr. Erin M. Buchanan received her Ph.D. from Texas Tech University in computational linguistics with a focus on statistics after attending Texas A\&M University for her undergraduate degree. In her spare time, she likes to watch sports, play video games, go to National Parks, and travel the globe.

Dr. Erin M. Buchanan’s research focuses on modelling semantic memory and the underlying language network by creating better measures of relationships between concepts. She also examines statistical practices and how we can improve those practices through enhanced methodology and teaching. Last, she collaborates with other investigators to improve their statistics and develop psychometrically sound measures of their concepts.

## Notes

Link to slides: [https://doomlab.quarto.pub/metadata-standards](https://doomlab.quarto.pub/metadata-standards) 

Resources: [https://marker.staplescience](https://marker.staplescience)

   * Metadata is structured context. The definition of "data about data" misses the point. 
   * **Three kinds of metadata:**
       * Descriptive
       * Structural
       * Administrative
   * **Metadata has different levels:**
       * Variable: Example is milliseconds, response time, etc.
       * File: Example is trials.csv
       * Dataset: Behavioural data from Study2.
       * Method: 
       * Project
   * **Who is metadata for?** 
       * **People:**
           * Future you
           * Collaborators and new lab members
           * Reviewers and replicators
           * Secondary analysts
       * **Machines:**
           * Search engines and repositories
           * Citation and indexing services
           * Pipelines and validators
           * AI tools and data discovery systems
   * **What is metadata used for? Consider the FAIR principles.**
       * ﻿﻿﻿Discovery: Can anyone find it? 
       * Interpretation: Can they understand it correctly?
       * Citation and credit: Can they cite it and credit the right people?
       * Governance: Can they tell what they're allowed to do with it?
       * Validation: Can software check it is complete and well-formed?
       * Integration: Can it be combined with other data?
       * Preservation: Will it still make sense in 10 years?
   * **FAIR depends on metadata**
       * Most of the FAIR principles are in practice statements about metadata
   * There's more to data than just 1s and 0s.
   * **In data, there's a lot of context:** geographically, formats, etc. This is Metadata standards come in:
       * A metadata standard is a shared agreement about:
           * ﻿﻿Which information to record (fields / elements)
           * ﻿﻿What each field means (definitions)
           * ﻿﻿How values are expressed (formats, units, allowed values)
           * ﻿﻿Which fields are required, recommended, or optional
           * ﻿﻿How the record is serialized (JSON, XML, CSV, RDF...)
   * **Specification vs. practice:** Having a standard on paper is not the same as using it.
       * ﻿﻿Validation: can software check a record against the rules?
       * ﻿﻿Tooling: are there forms, editors, and libraries?
       * ﻿﻿Adoption: do repositories and journals accept it?
       * ﻿﻿Documentation and examples: can a newcomer get started in an afternoon?
       * ﻿﻿Governance: who updates it, and how are changes versioned?
   * **There are different layers to a standard:**
       * Schema: the fields, types, and rules
       * Vocabulary/ontology: the allowed values and what terms mean
       * Serialization/format: how a record is written down
       * Reporting guideline: a checklist of what to report
       * Identifier system: persistent, unambiguous names
       * Profile: a schema constrained for a community
   * **Data Structure Standards:**
       * Frictionless data package/table schema
       * CSVW
   * **Metadata works best when you start early:** do the research as you go, and document along the way. 
   * **Make it part of the workflow**
       * **Practical habits that make metadata sustainable:**
           * ﻿﻿Templates: start every project from a standard README, codebook, and metadata file
           * ﻿﻿Version control: metadata files live next to the code and data
           * ﻿﻿Validation in CI: automatically check records on every change
           * ﻿﻿Generate, don't retype: derive metadata from data and code where possible
           * ﻿﻿Assign ownership: someone is responsible for keeping it current
           * ﻿﻿Review it: have a colleague try to use your data from the metadata alone
       * **Common pitfalls**
           * ﻿﻿Free text where a controlled value belongs: "Yes", "yes", "Y", "TRUE"
           * ﻿﻿Ambiguous dates, units, and missing-value codes
           * ﻿﻿Metadata separate from the data, so they drift out of sync
           * ﻿﻿Documenting once, never updating
           * ﻿﻿Over-engineering: a 200-field template nobody completes
           * ﻿﻿Picking the standard first and the questions second
           * ﻿﻿Treating compliance as quality: a valid record can still be uninformative
       * **Sometimes the standard doesn't exist. You may find:**
           * ﻿﻿A standard exists, but it is too heavy for everyday use
           * ﻿﻿A standard exists for the data, but not for the method or materials
           * ﻿﻿Your subfield has conventions but nothing formal
           * ﻿﻿Existing standards cover outputs but not the research process
       * **Key ideas**
           * Metadata is structured context, and context is what makes data reusable
           * A standard is a shared agreement on fields, meanings, values, and format
           * Distinguish schemas, vocabularies, identifiers, formats, and guidelines
           * The best designs are a small general core plus domain extensions
           * Reuse before you build; when you build, start from information needs
           * Capture metadata early and continuously, not at the end
           * Aim for enough: required core small, optional depth available
  
### Ending notes:
- You can watch the webinar [here](n/a).
- Previous webinar notes on From Openness to Impact: Measuring the Value of Open Data in African Health Systems can be found [here](https://github.com/aphrc-dswb/dswb-open-science-capacity-wg/blob/main/project-management/wg-meetings/20260917-oscb-wg-notes.md). 
