## Welcome to Journal Club - Led by Dr. Luc, DGH!

Date: August 5th, 2026

**Attendees:**
   * Luc
   * Precious
   * Deo
   * Brenda
   * Anicet
   * Winston
   * Habib
     
**Apologies**

   * N/A

## Notes

Journal Club Material:

Wang, P., Xu, N., Wu, L., Hong, Y., Qu, Y., Ren, Z., Luo, Q., \& Cai, K. (2024). *Construction and application of machine learning models for predicting intradialytic hypotension*. *PLOS ONE, 19*(6), e0305720. [https://doi.org/10.1371/journal.pone.0305720](https://doi.org/10.1371/journal.pone.0305720)

   * IDH is a blood-pressure drop during a dialysis session.
       * It is a frequent complication, but its estimated incidence depends strongly on the definition used.
       * It can lead to discomfort, premature termination of dialysis, under-dialysis, cardiovascular events and mortality.
       * Bedside prediction still relies largely on clinical experience rather than validated decision-support tools.
   * Practical question: 
   * Can we anticipate IDH risk before or at the beginning of a dialysis session using routinely available variables?
   * FIVE DEFINITIONS OF IDH
       * Definition - Criterion Used - Clinical Logic
           * D1 - Intradialytic SBP < 90 mmHg  -  Absolute pressure threshold
           * D2  - SBP drop ≥ 20 mmHg vs pre-dialysis  -  Moderate systolic drop
           * D3  - SBP drop ≥ 30 mmHg vs pre-dialysis  -  More severe systolic drop
           * D4  - SBP drop ≥ 20 mmHg or MAP drop ≥ 10 mmHg  - Broader definition
           * D5  - SBP drop ≥ 30 mmHg or MAP drop ≥ 10 mmHg  -  Balanced SBP/MAP drop
       * Why several definitions?
           * Guidelines and studies do not converge on a single IDH definition.
           * A model may perform well for one definition but be less clinically relevant for another.
           * The final definition should match the bedside intervention strategy.
       * IDH INCIDENCE BY DEFINITION
           * Clinical reading
               * D1 is rare: a strict SBP <90 mmHg event.
               * D4 is the most frequent definition because it combines SBP or MAP decline.
               * Frequencies are very similar between the training/testing and temporal validation cohorts.
           * Critical point
               * The chosen definition strongly changes prevalence, model difficulty, performance metrics and clinical use.
       * RESULT 1: CATBOOST DOMINATED
           * Key result
           * Test ROC-AUC ranged from 0.838 to 0.874 across definitions.
           * Performance was highest for D3, but all definitions remained in a clinically useful range.


       * RESULT 2: SHAP-BASED INTERPRETATION
           * Recurring variables in the top 20
           * Top 5: age, SBP, HR.
           * Top 10: + height, BMI, DBP, calcium.
           * Top 15: + ejection fraction.
           * Top 20: + dialysis vintage, WBC, LVMI
       * Major clinical insight
           * LVMI appeared as an important predictor, especially for definitions D2-D5. The authors suggest that cardiac remodeling should be integrated more explicitly into IDH risk prediction.
       * RESULT 3: SIMPLIFIED MODEL
           * 11 variables were almost enough:
               * Age • SBP. HR • Height • BMI • DBP • Calcium • EF • Dialysis vintage • WBC • LVMIR
           * Interpretation
               * The simplified model reduces data-collection burden while maintaining performance close to the full model.
               * This is a strong point for future clinical implementation
       * RESULT 4: TEMPORAL VALIDATION
           * Critical reading
               * Performance decreased in temporal validation but remained acceptable.
               * Validation was conducted in the same center: stronger than a random split, but not a true external validation.
               * Among the 15 newly recruited patients only, AUCs were more modest: a caution signal.
       * APPLICATION: A WEB-BASED PREDICTION TOOL
           * What the app does
               * The user selects an IDH definition.
               * The user enters the 11 simplified variables.
               * The app returns an IDH probability and a local SHAP plot.
               * A composite "overlapping definitions" model reached ROC-AUC 0.835.
           * Open Science value
               * The article does not stop at model development: it provides a reusable interface that supports discussion, reproduction and clinical evaluation.
           * LIMITATIONS AND CAUTION POINTS
               * Single-center study: limited generalizability beyond Ningbo
               * No.2 Hospital.
               * Temporal validation partly included patients already present in the initial cohort.
               * Large exclusion of sessions with missing data: possible selection bias.
               * Symptoms were not included in the IDH definitions, although clinical guidance often considers them useful.
               * Hyperparameters were not extensively optimized; no calibration or prospective decision-curve analysis was shown.
               * No impact evaluation: we do not know whether the model reduces IDH episodes or improves patient outcomes.
           * Questions for discussion
               * ﻿﻿﻿Which definition should be used at the bedside?
               * ﻿﻿﻿At what risk threshold should clinicians intervene?
               * ﻿﻿﻿What if echocardiography variables are missing?
               * ﻿﻿﻿Is the model robust enough for sub-Saharan African dialysis units?
           * RELEVANCE FOR DOUALA GENERAL HOSPITAL
               * A possible local roadmap: 
                   * Structure routine hemodialysis data: sessions, pre/intra/post BP, UFV/UFR, symptoms and nursing interventions.
                   * Define a local IDH outcome aligned with clinical practice and patient safety.
                   * Build an OMOP/DHIS2 cohort or dedicated registry to support audits, dashboards and predictive models.
                   * Validate prospectively before any clinical integration.
               * Take-home
               * The paper points in the right direction: a useful model should not only predict. It should be simple, interpretable, locally validated and integrated into the clinical workflow

    
## General Note

   * Kindly find previous journal club notes here: https://github.com/aphrc-dswb/dswb-open-science-capacity-wg/blob/main/project-management/coworking-calls/20260708-coworking-call-notes.md
