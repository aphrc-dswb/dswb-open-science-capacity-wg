## Welcome to Journal Club - Led by Nael and Pape Malick, IRESSEF Team!

Date: May 6th, 2026

**Attendees:**
   * Pape
   * Michael L.
   * Samba
   * Precious
   * Daffe
   * Akililu
   * David
   * Michael
   * Yordanos
   * Nael
   * Michael O.
   * Domian 
   * Mane
     
**Apologies**

   * N/A

## Notes

Journal Club Material:

Xiao, Y., Wang, Y., Yuan, Q., He, J., \& Zhang, L. (2023). Generating a long-term (2003–2020) hourly 0.25° global PM2.5 dataset via spatiotemporal downscaling of CAMS with deep learning (DeepCAMS). Environmental Pollution, 328, 121622. [https://doi.org/10.1016/j.envpol.2023.121622](https://doi.org/10.1016/j.envpol.2023.121622)



## Presentation 1:

   * Challenges:
       * Organise 133+ variables around 4 dimensions. Historically applied to criminological investigations.
           * Person - who is concerned?
               * Confirmed cases by sex (F/M)
               * Pregnant women IPT 1-> 4
               * ACT by age group
               * Deaths by sex
           * Object
               * What inputs?
                   * ACT stocks (4 formulas)
                   * Artesunate, Quinine 200/400
                   * Primaquine, SP
                   * RDT (stock \& utilization)
           * Location
               * HRD (Health regional directorate)
               * Health district
               * PERIOD (month/year)
               * Care level (inpat./outpat.)
           * Event
               * RDT/BS tests performed
               * Suspected and confirmed cases
               * Hospitalization and deaths 
               * Stockouts


Question and Answer:

   * Question: Do you want to share what led to it?
       * Answer: We have a huge amount of variables, and mapping them into those four dimensions reveal very similar patterns amongst the phenomena. 


## Presentation 2: Paper



Challenges:

   * Air pollution exposure varies strongly in space and time.
   * ﻿﻿Long-term reanalysis products are globally consistent, but too coarse for fine-scale studies.
   * ﻿﻿Running high-resolution chemistry models globally is computationally expensive.
   * ﻿﻿Deep learning can learn a statistical mapping from coarse to fine products.


Data Sources used:

   * CAMS: long term product to downscale 2003 - 2010| 0.75 degrees
   * GEOS-CF: High resolution reference for learning 2018-2020
   * OpenAQ: Ground station observations for validation 2017-2019


Spatial Downscaling with ABPN:

   * Input GEOS-CF HR data are degraded to build LR/HR training pairs.
   * ﻿﻿ABPN learns recurrent up-down sampling back-projection.
   * ﻿﻿EUBP and EDBP blocks model nonlinear LR→HR mapping.
   * ﻿﻿Spatial Attention Blocks capture cross-feature correlations.
   * ﻿﻿Loss: L1 distance between super-resolved and ground-truth PM2.5 maps.


Experimental Design: Train on 2018-2019 GEOS-CF and test on 2020.



**Potential role in DSWB**

• Builds on ongoing air quality activities led by Dr. Daffe and partners.

• Use CAMS / DeepCAMS as a continuous background exposure modelling field.

• Calibrate locally with Dakar CGQA stations and Douala low-cost sensors

• Integrate meteorological variables: wind, humidity, shema org ISON 200 temperature.

• Produce daily exposure indicators and WHO threshold exceedances.

• Feed exposure variables into OMOP CDM / health-risk assessment workflows.



**Key position**

DeepCAMS is a methodological baseline, not a city-scale final solution. The local model should add ground sensors and context-specific covariates.



Strengths: 

   * Directly addresses spatiotemporal downscaling of CAMS
   * ﻿﻿Uses GEOS-CF creatively to learn fine-scale patterns.
   * ﻿﻿Combines temporal and spatial deep learning methods.
   * Produces a long-term global PM2.5 dataset.
   * Maintains spatial consistency and temporal continuity.


**Limitations**

   * 0.25° is still coarse for intra-urban analysis in Dakar or Douala.
   * ﻿﻿Training target is GEOS-CF, not direct ground truth.
   * ﻿﻿Multi-step pipeline may accumulate errors.
   * ﻿﻿No auxiliary variables are used: wind, temperature, humidity, land use, traffic, etc.
   * 

   * Focused only on PM2.5






**Recommended adaptation roadmap**



**A pragmatic way to move from DeepCAMS to Dakar/Douala**



- Baseline: Download CAMS / DeepCAMS and assess PM2.5 consistency over Dakar and Douala.

- Local calibration: Use stations and low-cost sensors to correct bias and account for local variability.

- Covariates: Add meteorology, land use, road density, industrial areas, population, dust seasonality. 

- Model comparison: Benchmark kriging, RF/GBoost, Bayesian models, and lightweight deep learning.

- Health exposure: Generate daily exposure features for OMOP CDM and health-risk assessment.





Scientific questions to discuss: 

- Which pollutant first? What target resolution? What validation strategy with few stations? How to represent uncertainty?


**Key Takeaways:**

   * DeepCAMS is highly relevant because it directly downscales CAMS PM2.5 using deep learning. 
   * Its architecture combines video frame interpolation and image super-resolution.
   * It improves resolution from 0.75° / 3h to 0.25° / 1h while preserving CAMS-level accuracy. 
   * For DSWB, the strongest value is as a baseline to combine with local sensors and meteorological covariates.


Questions:

- Using the timeline of the datasets shared, it was COVID season. Do you think that the different timelines could affect the results of the variables? 



Resources:

   * [https://github.com/XY-boy/DeepCAMS](https://github.com/XY-boy/DeepCAMS) 
    
## General Note

   * Please find the notes for the previous Journal Club, here: https://github.com/aphrc-dswb/dswb-open-science-capacity-wg/blob/main/project-management/coworking-calls/20260401-coworking-call-notes.md
