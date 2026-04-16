# DSWB External Webinar - Open Science and Capacity Building Working Group  

**Webinar Topic:** Reproducibility in the age of AI

**Date:** 19th March, 2026


### 🌍 Icebreaker Question

**Name (or pseudonym or emoji) /  Organisation / One thing you hope to learn or take away from this session?**

- LNO/IITA/code+LLMs and their contribution to reproducibility in this AI boom
- Precious/DSWB/How can we make AI systems more reproducible? 
- Winston/DSWB-DGH/Applications for AI systems 
- Ousmanz/IRESSEF

# Speaker - Albert Kahira

### Speaker bio

Albert Njoroge Kahira is an AI engineer working at the intersection of artificial intelligence, data, and infrastructure. 
He focuses on building and evaluating real-world AI systems, with particular attention to reproducibility, dataset quality, and the integrity 
of end-to-end machine learning workflows. He regularly advises on data systems and open practices in AI, and is interested in how technical 
infrastructure shapes trust, accountability, and who ultimately has the power to build and audit intelligent systems.

## Notes

* Talk Focus: The Usage of AI for Science
   * If you cannot reproduce a system, you cannot debug it, learn from it, or reuse it. 
   * With AI, Everything changes:
       * Al systems introduce:
           * Non-deterministic behaviour
           * Large-scale pipelines
           * Heavy dependence on data
           * Complex model architectures 
       * You can conduct an experiment with AI, and end up with two different results. AI changes a lot with how we do science.
   * The Core Shift: We have moved from:
       * Experiments
       * Controlled and repeatable
   * to: 
       * Pipelines
       * Multi step, distributed, data driven, complex and evolving
       * Reproducibility now spans entire systems
   * Reproducibility means something else:
       * We are producing an enormous amount of data.
       * The cost of experimentation is lower, but it also increases the cost of verification. 
   * What Reproducibility Means:
       * We are producing results faster than we can validate them.
           * More results
           * Less certainty
       * Al lowers the cost of experimentation, but increases the complexity of verification
           * Reproducibility today means
               * Reconstructing the full workflow
               * Not rerunning code
           * These are not trivial, neither are they cheap.
       * Reproducibility means reconstructing the entire outcome that produced the result. 
       * Reproducibility is not cheap: the tools, or the labour.
       * THE AI research workflow:
           * Reproducibility depends on:
               * Data
               * Code
               * Model
               * Inference
               * Evalutation
           * However, reproducibility is really important, and we need to think about how these challenges can be solved.
           * Where Reproducibility Breaks: Data
               * Versioning: without correct versioning, we cannot have correct data because we can't really tell what happened in the previous version.
               * Preprocessing
               * Provenance
           * Where Reproducibility Breaks: Models
               * Training Data opacity: we see in open source, that both the models, and the data used to train them are requested for. This helps to detect biases in the data, etc.
               * Model updates: Models have various versions, and we may not be able to tell the information in previous models
               * Lack of version control
           * Where Reproducibility Breaks: Evaluation
               * Metrics
               * Benchmarks
               * Experimental Setup
           * **The Real Problem**
           * Reproducibility does not fail because systems are complex. It fails because decisions across the pipeline are not documented. (Reproducibility is an Engineering problem - personal quote)
               * ﻿﻿Data selection and filtering
               * ﻿﻿Preprocessing steps
               * ﻿﻿Model choices and configurations
               * ﻿﻿Prompt design and inference settings
               * ﻿﻿Evaluation setup and metrics
           * **What is not recorded cannot be reproduced.**
               * The same principles in the various lab sciences can be transferred and implemented in AI systems. 
           * **Reproducibility should be added to the engineering cycle.**
               * The processes should be logged.
               * It should be versioned.
               * It should be traceable.
               * There should be a system design. 
           * Reproducibility should be an engineering requirement, not just an afterthought or a documentation exercise. 
           * Reproducibility must be engineered into the workflow. 
           * 

       * Solutions
           * **Open Workflows as Engineering Infrastructure**
           * Open workflows = systems where every step can be seen, traced, and reconstructed
               * Making pipelines observable
               * Making decisions explicit
               * Making systems auditable
           * Open workflows really means :
               * Versioned datasets
               * Logged experiments
               * Transparent preprocessing with very good explanations of why these happen. 
               * Documented prompts
               * Reproducible evaluation
           * Practical Minimum Standard
           * A reproducible workflow should include at minimum:
               * Data snapshot or access protocol
               * Code version (repository + commit)
               * Environment specification
               * Model version or reference
               * Inference logs (inputs and settings)
               * Evaluation pipeline and metrics

       * Limits
           * Reproducibility is not always fully achievable
               * Models are closed
               * Data is hidden
               * Systems evolve
           * However, we can still aim for minimums.
               * Maximum transparency
               * Clear documentation
               * Reproducible evaluation

       * Why It Matters
           * If it cannot be reproduced:
               * ﻿﻿It cannot be verified
               * ﻿﻿It cannot be trusted
               * ﻿﻿It should not be used
               
Reproducibility is the foundation of trust. It is the only way we can keep science and systems honest.

### Ending notes:
- You can watch the webinar here: https://youtu.be/ZyUdLx1LF6A?si=vcbood_nOVBAJov2.
- Previous webinar notes on Digital Public Goods Alliance (DPGA) Framework and Its Relevance in Africa can be found [here](https://github.com/aphrc-dswb/dswb-open-science-capacity-wg/blob/main/project-management/wg-meetings/20260219-oscb-wg-notes.md).

