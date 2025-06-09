# Data Science Without Borders Coworking Call - Welcome to journal club: Daffe and Moctar!

Date: June 4th, 2025

_Paper selected for discussion: Frévent, C., Ahmed, M.-S., Dabo-Niang, S., \& Genin, M. (2023). Investigating spatial scan statistics for multivariate functional data. Journal of the Royal Statistical Society Series C: Applied Statistics, 72(2), 450–475. doi: 10.1093/jrsssc/qlad017_

**Attendees:**
   * Moctar
   * Daffe
   * Malvika
   * Agnes
   * Miranda
   * Anicet
   * Joseph
   * Mulugeta
   * Fikregabrail
   * Yordanos
   * Valentine
   * Cyrille
   * Jay
   * Belayneh
   * Winston
   * Melissa
   * Raissa
     
**Apologies**
   * Precious - on leave

**Notes from paper presentation:**

   * Air pollution can lead to pre-mature death (WHO - 3 mio)
   * People closer to factories have more exposure to harmful air pollutant
   * The paper uses spatial scan statistics (spatial analysis - SA) to explore this theme
   * Progress in sensing and data storage: Emergence of functional data analysis (FDA) - led to functional data analysis in environmental research
       * new clustering methods for spatial functional data (FDA+ SA)
           * Can't be used for detecting pollution clusters or test cluster's statistical significance
       * This led to emerggence of Spatial Scan statistics (SCS)
   * Data used: Daily averae concentration nitrogen dioxide, ozone and particulate matter (data provided by PREV AIR french national air wuality forecastim system)
   * Data analysis shows the distributions of these particles tend to be similar except for ozone
       * NO2 and O3 distribution were diametrically opposed
       * High concentration of O3 in some areas
   * SCS might be of value for detecting spatial cluster of pollutant concentrations over a period of a month (october 2021 data)
   * They developed three new functional SCS (FSS)
       * MDS-FSS (multivariate distribution free)
       * MP-FSS (multivariate parametric)
       * MRB-FSS (multivariate rank based)
   * All methids detetcted statistically significant cluster (p< 0.001)
       * MDS performs best of Gaissian data
       * MPB has greater robustness to non gaussian data
       * MP os sonservative, detects few false posutive but detects few cluster overall/0
   * Application in DSWB
       * Precitive AI model to forecast air pollution levels
       * Map pollution level over different areas of Dakar
       * Air pollution based health risk assessment

**Notes from discussion**

   * How do we bring this closer to DSWB
   * We heard about air pollution models, but we also heard about the implication of air pollution in health - how do we combine this study in DSWB?
       * Do we need to do similar study parallel in different countries to find correlation?
       * The data is for 1 month in October in France -- how do we replicate this study in DGH? Is this a good enough timeframe or we thinkabout a longer time points?
           * How does country-level cluster show across different countries in Africa
           * How do we account for differentd
       * Can we have parallel analysis with emdemiology to see correlatioon of air pollution on health impact?
   * Daffe and Winston are working on this proposal in DGH and have already found some indicators that they are working on
       * Modeling air quality in Duala and Dakar - have looked into the data collected
           * Some particulate matters are similar (matter 1 and 2)
           * Some matters are different in different location
           * How would you superimpose the climate data, since the admissions due to respiratory infections might also be driven by seasonality
               * Air data trend look different in day and night, as well as season (like during rainy season air quality is better, during rush hour - quality is bad)
                   * We augment the data collection using satellite data
                   * We will begin with descriptive analysis - correlate with hospital admission
               * Estimating the health impact of air quality - we can use some estimators that we can look in literature related to epidemeology studies with related risk
                   * Can be estimated to hospital admission, reporting of a disease
       * Can we use the statistical method explained in the paper for our study?
           * We can explore if spatial scan method for data from Cameroon
           * Can continue to discuss this - Anicet will look at the method in details
       * Note from Jay (CODATA): APHRC is conducting a study on climate change and HIV incidence that use satellite data from Copernicus.
           * The spatial resolution in a 31 km grid. The temporal resolution starts in the 1990s (hourly data that can be aggregated in different ways).
       * Do we have real-time data collection on health data?
           * EPI data will come from DHIS2: [https://docs.dhis2.org/en/implement/maintenance-and-use/tracker-and-aggregate-data-integration.html](https://docs.dhis2.org/en/implement/maintenance-and-use/tracker-and-aggregate-data-integration.html) (covers all partnering countries) - monthly aggregated data.
               * Cause of dealth, hospitalisation, type of diseases.
               * DGH's HIV + other data can also be integrated. Their hospital data can also be looked into.
               * Can look at wider scope of what happening in hospital and their correlation with air quality.
               * Africa CDC data won't be available for individual-level data
                   * not openly available (may exist in EHR)
           * In DGH, DAMA tool is used for extracting data from journal 
               * Takes a lot of time and depends
       * A previous study related to water sanitation: [https://iwaponline.com/jwh/article/20/11/1654/91574/Water-sanitation-and-hygiene-access-in-Senegal-and](https://iwaponline.com/jwh/article/20/11/1654/91574/Water-sanitation-and-hygiene-access-in-Senegal-and)
           * Explored predictive factor of diarrhea for children under 5 in Senegal 
           * Identified specific factor in data that can be used to predict occurance in children
           * Also explored sanitation and hygiene in terms of access
               * identified that the risk factors - closeness to water source was correlated to diarrhea - indicating closeness to human-activity led contamination
