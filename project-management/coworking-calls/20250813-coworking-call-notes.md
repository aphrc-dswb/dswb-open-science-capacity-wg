# Data Science Without Borders Coworking Call - Journal Club

## Welcome to Journal Club - Rachel, APHRC Team!

Date: August 13th, 2025

**Attendees:**
   * Laurah
   * Frank
   * Daffe
   * Magatte
   * Moctar
   * Yordanos
   * Miranda
   * Anicet
   * Serena
   * Belayneh
   * Mulugeta
   * Precious
     
**Apologies**

   * N/A

## Notes

**Journal Club Material:**

_Ng’etich, M., Odhiambo, R., Cygu, S., Nabukeera, B., Dube, A., Butichi, B., Mclean, E., Ziraba, A., Kadengye, D., Kajungu, D., \& Kiragga, A. (n.d.). *The burden of death from vaccine preventable diseases in Africa: Evidence from health demographic surveillance sites in Eastern and Southern Africa.*_
  
   * **Background:**
       * Vaccine-preventable diseases (VPDs) remain a significant cause of morbidity and mortality in many low- and middle-income countries.
       * Understanding the age, gender, and site-specific distribution of VPD-related deaths helps inform targeted public health interventions.
       * This study uses verbal autopsy (VA) data from three Health and Demographic
       * Surveillance System (HDSS) sites: NUHDSS (Kenya), Iganga-Mayuge (Uganda) and Karonga HDSS(Malawi).
       * The goal is to describe mortality patterns and explore potential differences in disease burden across demographic groups.
   * Study design: Descriptive cross-sectional analysis.
   * ﻿﻿Data source: VA data from NUHDSS (Kenya), Karonga(Malawi) \&
   * Iganga-Mayuge (Uganda).
   * ﻿﻿Timeframe: 2002-2022.
   * ﻿﻿ICD-10 Classification of VPDs
       * Analysis variables: Cause of death, age group, HDSS Site.
       * Classification: Causes mapped to VPD categories.
   * Data was cleaned and processed using R
   * Epidemiological variability: VPD burden differs sharply between sites analysed.
   * ﻿﻿Pneumonia & meningitis remain universal threats
   * Localized peaks: 
       * TB is more prominent in the urban areas, 
       * Diarrheal diseases are more prominent in the rural areas, dengue (select sites)
   * ﻿﻿Age-gender nuances critical for targeting interventions
       * Infants are  more prone to oral diseases
       * Adults are more prone to TB
   * ﻿﻿Implications for vaccine strategy and surveillance systems
       * There has to be a strategy for vaccinations. People do not get vaccinated due to the infrastructure. 
   * Strengths:
       * ﻿﻿Multi-site, multi-year dataset
       * ﻿﻿Verbal Autopsy data enables cause-of-death insights in low-certification settings
           * You just need to interview the family members, they let you know the systems the individual had, and you can attribute a cause.
       * Gender- and age-stratified analysis enabled the trend to be viewed from various angles.
   * Limitations:
       * ﻿﻿Verbal autopsy (VA) data prone to misclassification
           * Due to verbal autopsy, it is possible to add a cause that is not true to a symptom.
       * ﻿﻿Variable years of data across sites
           * Some sites had unavailable datasets.
       * Possible under-reporting of some VPDs
       * Limited lab confirmation for diagnoses
           * Since the cause were given due to the verbal autopsy (VA) gotten from the family members, diagnoses could have been inaccurate or wrongly identified.
           * Was a standard tool for verbal autopsy (VA) used across the different sites (i may have missed this during your presentation).

* **Recommendations:**

   * ﻿﻿Pneumonia \& meningitis: consistent high-burden diseases
   * ﻿﻿Disease profiles vary by site, age, and gender
   * ﻿﻿Strengthen site-specific immunization \& surveillance
   * ﻿﻿Integrate gender- and age-responsive approaches
   * ﻿﻿Sustain multi-site VPD monitoring for early detection


* **Questions:**

   * How did you account for the different time periods during your analysis? - Miranda
   * Was a standard tool for VA used across the different sites - Miranda
      * Response: Yes, both InterVA and InsiliocoVA
   * Why was R your language of choice over Python?
      * Response: R is known to give good visual and is easier to use for analysis
   * What is the vaccination coverage rate in these régions? Are there any national vaccination programmes or campaigns? What about vaccine coverage for children Under 0-5? - Moctar
     * Response: Vaccine coverage in the countries where the sites are is generally less than 90%. The countries have several vaccination campaign programs, and I have it all documented in the paper I can share.
   * Is there any plan for the prediction of the vaccination coverage? It would be interesting- Moctar.
     * Response: I think this would be interesting to model the impact that campaigns would have on the vaccine coverage- agree 100%
   * Daffe: Meningitis often has symptoms that may look like malaria, so early diagnosis often rarely works and all these diseases still exist even despite the strides that have been made mainly because of vaccine hesitancy, also most of these HDSS sites are either located in rural areas or informal urban that are clearly known for their limited infrastructure.


## Previous Notes

   * Briefing for the external webinar.
   * Mulugeta and Belayneh worked on their presentation for the Platform and Data Harmonization WG meeting.
      
See [previous meeting note](https://github.com/aphrc-dswb/dswb-open-science-capacity-wg/blob/main/project-management/coworking-calls/20250730-coworking-call-notes.md) for more information.
