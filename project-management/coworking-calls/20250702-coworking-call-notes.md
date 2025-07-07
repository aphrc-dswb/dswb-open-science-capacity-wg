# Data Science Without Borders Coworking Call - Welcome to Journal Club: Brenda, DGH Team 

Date: July 2nd, 2025

**Attendees:**
   * Precious
   * Brenda
   * Anicet
   * Malvika 
   * Belayneh
   * Laurah
   * Jay
   * Daffe
   * Cyrille
   * Lifafa
   * Mary
   * Miranda
   * Moctar
   * Winston
   * Serena
   * Sington
   * Yordanos
   * Gumba - Interpreter
   * Vincent - Interpreter
   * Ousmane
   * Magette
   * Raissa
     
**Apologies**

   * N/A

## Notes

   * **Reason for article:**
       * Data science related, and helps us figure out what machine learning algorithms can be used to predict sepsis, and other diseases we have data for. 
       * We can explore systematic and meta-analysis amongst the pathfinders. 
   * **Background:**
       * Sepsis is a life-threatening condition requiring early detection and treatment to reduce morbidity and mortality. 
       * Early identification is important. 
       * ML algorithms are a technology branch that has shown the ability to predict 
   * **Purpose:**
       * Compare the most effective algorithm. 
   * **Inclusion Criteria:**
       * PICO; Original research studies in English (excluding letters, editorials, etc.), case-control or cohort designs with control groups.
           * • Population: Patients with no limitations on age, gender, race, or duration of illness.
           * • Intervention: Use of a different machine model to predict sepsis occurrence.
       * • Comparison: Studies with control groups.
       * • Outcome: Reported Sensitivity (Se), Specificity (Sp), True Positive (TP), True Negative (TN), False Positive (FP), False Negative (FN), and sample size.
   * **Machine Learning Algorithms used:**
       * 16 different algorithms
   * **Data extraction and quality assessment:**
       * Independently performed by three review authors.
       * Conducted independently by two review authors using the Quality Assessment of Diagnostic Accuracy Studies (QUADAS)-2 tool.
       * Stata 17.0 software. NMA was performed.
       * Measurements were expressed as relative risk (RR) and 95% Cl.
   * **Data Analysis:**
       * Inconsistency Testing:
           * Overall consistency between direct and indirect evidence was analysed using the inconsistency test (P > 0.05 indicated no inconsistency).
           * Local inconsistency tests also performed (P < 0.05 indicated inconsistency).
           * Results showed consistency, allowing for consistency modeling analysis.
           * Ranking of interventions under the subsurface cumulative ranking (SUCRA), and a higher SUCRA indicates better accuracy.
   * **Results**
       * NMA consistency
           * The network evidence plots for sensitivity, specificity, and predictive accuracy showed that different ML algorithms met the basic conditions for NMA. This shows the acceptance of heterogenuity.
           * Global and local inconsistency tests indicated no statistically significant difference (P > 0.05), allowing for consistent modeling analysis.
       * Performance comparison: SUCRA scores
           * Sensitivity: DSPA (77.0%), Imbalance-XGBoost (72.9%).
           * Specificity: CNN (78.3%), CNN+Bi-LSTM (77.6%).
           * Predictive Accuracy: DSPA (85.9%), CNN+Bi-LSTM (82.6%).
           * SVM and Bi-LSTM performed poorly in all metrics.
   * **Discussion**
       * Strengths of DSPA and CNN
           * Advanced architectures allow superior learning from complex clinical data.
       * Clinical Implications
           * ML models can support early detection and timely treatment, reducing mortality. Due to data imbalance and complexity, traditional ML, such as SVM and NB, may be insufficient.
   * **Limitations**
       * Only 7 cohort studies included.
       * Varied sample sizes; 211 to 22,314 may introduce bias.
       * The study did not account for differences in data sources, model training, validation, and implementation across included
   * **Conclusions**
       * DSPA is the most effective ML algorithm for sepsis prediction in terms of sensitivity and predictive accuracy.
       * CNN is the most effective ML algorithm for sepsis prediction in terms of specificity.
       * Network meta-analysis provides robust comparative insights.
       * Imbalance-XGBoost excels among traditional ML algorithms for sensitivity and predictive accuracy, particularly for imbalanced
       * The study explored 16 different ML algorithms, with varying specificity, which can be importan to the work of DSWB, and is open to consoderation relative to the dataset we currrently jave available. We can explore the article to understand the methodolodies used, and chances for collavoration to perform systematic reviews and meta-analysis. We can explore other aspects of data science using the datasets available to us. 
   * **Questions:**
       * What are some ML algorithms we can explore with respect to the DSWB project?
           * The disease being worked on determines what algorithm would better fit the criteria. 
       * What are the benefits we would have from this? What is its peculiarity compared to other MLs currently being worked on? 
           * It was a comparative study, so the different algorithms were comapred to show what their strengths are in differnt environments.
           * However, in your own project, you can compare and explore the relativity to what you're working on with respect to traditional projects, and come up with your own analysis for what would work. 
       * Under what circumstances would we use MNA across DSWB as opposed to federated learning or other methods of model aggregation or can MNA somehow be used with FL or other aggregation algorithms together?
           * Open question...
           * Thought: 
               * When working with FL, it means that certain analysis are explored and datasets are gotten from various locations. To work properly, it would be great to understand what others are working on, and build upon existing knowledge. 
       * What are some challenges/concerns you identified with respect to these studies and how can we work around them? What are some areas where issues can be experienced?
           * Limited sample size.
           * They considered a study on sepsis, so it is important to ensure that the algorithms used can be applied to the sample size, else it would be doing ML for the sake of it, without results.
       * After reading this article, are you not tempted to change your methodology when you see how well the algorithms shown in the study perform?
           * No, but I am tempted to explore all possible algorithms that can be incorporated into the study that I am currently working on. 

## Previous Notes

### Things we worked on

   * We did an upload-a-thon for Zenodo and shared guidelines for content to upload on Zenodo.
      
See [previous meeting note](https://github.com/aphrc-dswb/dswb-open-science-capacity-wg/blob/main/project-management/coworking-calls/20250625-coworking-call-notes.md) for more information.
