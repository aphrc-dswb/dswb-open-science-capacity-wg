
# External Webinar - Open Science and Capacity Building Working Group  

**Date:** August 21st, 2025


## 🗣️Welcome!

#### Introduction 

**Host:** Michael Landi (Precious + Nyasita)

00:05 - 00:06 [⏰ 1min]  Welcoming note

***
* We have a code of conduct - [https://aphrc-dswb.github.io/dswb-open-science-capacity-wg/coc](https://aphrc-dswb.github.io/dswb-open-science-capacity-wg/coc)
  * If you experience or witness unacceptable behaviour, or have any other concerns, please report it by contacting the organisers - Michael, Nyasita, and Precious. (**osponow.dswb@gmail.com**).
* This call is being recorded.
  * The video may be shared with others
  * Turn on your webcam if you don't mind sharing your face (or off if you do)

* All notes will be taken in Framapad and archived on the public DSWB GitHub, including your name and response. You may use a pseudonym or add an emoji 🤫 if you don’t want to be included. To request removal, email **precious@osponow.com** or **osponow.dswb@gmail.com**

* AI notetakers would also be removed from the call for privacy and safety reasons. You will get the recording and the notes of this session after the call .

## 👋 Icebreaker

**_Name (or pseudonym or emoji) / What role do you play in the data ecosystem — collector, user, curator, policymaker / One thing you hope to learn or take away from this session?_**

(Use this Etherpad for getting to know each other and for collaborative notes)
   * Pauline / user\&curator / getting around the socio-technical barriers that prevent the use of synthetic data
   * BM /collector, user \& creator / Learning more techniques for synthetic data creation and interacting with the community
   * Clifford /user \&curator/Get an answer to the question: Is synthetic data really valid and reliable in the public health research space?
   * EW / user \& curator / with the advent of sharing data, how can we ensure user privacy considering data protections like the European privacy user data protection
   * MKL / user 
   * Faith/User
   * Luc /User\&curator/ Hope to learn how synthetic data can enhance Research in Low and middle income settings
   * David /Collector \& User \& Curator/ Where we are at in Africa with regards to Synthetic data and how to overcome our challenges with regards to perceptions and receptions as a source of real research questions 
   * Mulugeta/I am early career researcher working at AHRI and I am a medical Dr and pursuing my masters in public health data science and I am working my thesis on prediction modeling of cervical cancer in hiv patients and I believe I will contribute to the data ecosystem by providing data analysis output from the big data which is generated in the health ecosystem and also contribute to generated evidence for policy makers and to contribute on the establishment of warehouse for African data set 
   * Iyanu /Collector and user/ Learn how to use Synthetic Data ethically and get accurate results
   * FOMAZOU/User/Which to know how synthetic data can be used in the context of Medical image (such as malaria microscopies cells) analysis when expert labeled are unavailable
   * Bryan / data user, although I do a bit of collection and curation.
   * Shegaw/ data curator, and I hope to learn how synthetic data can be applied in AFRICAN contexts while ensuring privacy, accuracy...
   * Kennedy, I play multiple roles, a user and curator. I want to learn if and how to use synthetic data to bridge the small-sample/data problem we have, especially in social sciences Africa
   *  👋 I play the role of collector, user, and curator. 😁
   *  Lorine /Data curator and user
   *  Olive / Data collector, user and curator
  
## 📣 Agenda
00:15 - 00:55: [⏰ 40min]

## Presentation - Dr Bryan Shepherd.

**Speaker Bio**

Bryan Shepherd is Professor and Vice Chair for Faculty Affairs in the Department of Biostatistics at Vanderbilt University. 
Dr. Shepherd received his PhD in Biostatistics at the University of Washington in 2005, and he has been a faculty member at Vanderbilt since then. Dr. Shepherd’s 
research interests include developing and applying novel statistical methods to studies of HIV and other global health diseases. 
He has been the lead statistician for the Vanderbilt Institute for Global Health; the Caribbean, Central and South America network 
for HIV epidemiology (CCASAnet); and the Tennessee Center for AIDS Research. His statistical methodology research is in areas of causal inference, 
statistical methods for error-prone data, ordinal/rank-based statistical methods, and, most recently, synthetic data generation. 
He has mentored many PhD students both at Vanderbilt and internationally. Dr. Shepherd directs the Vanderbilt-Nigeria Biostatistics Training Program. 
Dr. Shepherd is a fellow of the American Statistical Association.


**Notes:**

   * **What is synthetic data?**
       * Artificially generated data meant to reflect real data, but not actually real data.
       * ﻿﻿Is adding noise creating synthetic data?
           * ﻿﻿No, at least not for this talk.
           * ﻿﻿We will consider synthetic data as being generated by sampling from an underlying distribution.
           * ﻿﻿No 1:1 mapping to original data.
   * **Why Would Anyone Want Synthetic HIV Data?**
       * ﻿﻿Because it is getting harder to share HIV data.
           * ﻿﻿International laws are getting more stringent
           * ﻿﻿Privacy concerns
           * ﻿﻿Ethical agreements
       * ﻿﻿There are great benefits to sharing data
           * ﻿﻿Open science leads to increased collaboration, efficiency, higher quality, and innovation
           * ﻿﻿Funding agencies and journals are pushing for more open science
           * ﻿﻿Synthetic data are perhaps a pragmatic way forward, as these data are more easily shared
   * **Use of Synthetic data**
       * Quasi-Reproducible Research
           * Published papers include
               * code used for published analyses
               * synthetic data
               * results applying code to the synthetic data
           * Others know exactly how the analyses were performed.
           * A scientific paper from the
       * Facilitating education
       * Headstart developing analysis code
           * ﻿﻿While waiting to receive permission for the original data
           * ﻿﻿Or researchers may never receive original data - analyses run by data owners or remotely using computational tools
           * ﻿﻿Some Examples: 
               * ﻿﻿Scottish Longitudinal Study
               * ﻿﻿N3C Covid Enclave Data
               * ﻿﻿Agency for Healthcare Research and Quality (AHRQ)
               * ﻿﻿All of Us
               * ﻿﻿UK Biobank: [https://biobank.ndph.ox.ac.uk/synthetic\_dataset/](https://biobank.ndph.ox.ac.uk/synthetic\_dataset/)
       * Augmentation to Address Health Disparities
           * ﻿﻿Prediction models often perform poorly for underrepresented groups because models were built using data with few from these groups.
           * ﻿﻿Synthetic data for underrepresented groups may be added to real data, thus making models fit to augmented data more representative.
           * ﻿﻿This seems to work for images, including medical imaging.
           * There is some skepticism about using this in synthetic HIV data, but some groups have seen beneficial results.
       * Hypothesis Generation Hypothesis Testing (HGHT)
       * ﻿﻿Hypothesis Generation:
           * ﻿﻿Investigators unaffiliated with HIV research networks can perform exploratory analyses with synthetic data.
       * ﻿﻿Hypothesis Testing:
           * ﻿﻿They can then approach the research network to perform similar analyses on the original data when there is evidence suggesting an important discovery.
           * ﻿﻿It is the grail of synthetic data.
           * ﻿﻿Open HIV research to the masses to generate more ideas and findings.
   * **Tradeoffs/Utility Tradeoffs**
       * Synthetic data must preserve privacy and be useful.
       * The better the privacy, often the worse the utility.
       * There is the question of measuring privacy and utility?
   * **How to Generate Synthetic HIV Data?**
       * Statistical models - based on multiple imputation ideas
   * **Limitations of Statistical Models:**
       * Works well for a single study with not too many variables - about an approximate of 10.
       * ﻿﻿Becomes unwieldy with lots of variables
       * ﻿﻿CCASAnet has somewhere around 200 variables in multiple tables
       * ﻿﻿The longitudinal structure of the data complicates things
       * ﻿﻿Non-linearities and interactions can be included in statistical models, but difficult to sufficiently explore the space.
       * ﻿﻿Simulating from statistical models is simulating from something that you know. It's not good for generating new hypotheses because you are generating data from things you already know. 
   * **How does this work with AI:**
       * AI has different facets: Machine learning, Neural networks, and Deep learning. Most of what we know as AI is the deep learning aspect.
           * regression learning: Fewer parameters
           * Neural networks: more parameters than a regression learning
           * Deep learning: More parameters than regression learning and neural networks.
               * Deep learning has lots of parameters, so it requires lots of data. Even with lots of data, overfitting is possible. Over-fitting is avoided with the use of validation datasets. 
   * **AI for Synthetic Data**
       * Variational Auto-Encoder (VAE)
           * Output that looks like the original data, but is not the original data.
       * Generative Adversarial Networks (GAN)
           * Two neural networks, one of them predicts what data is fake, and which is real. The generator learns from that and gives that information to the discriminator until the generator is able to create fake data that the discriminator is not able to detect.
       * Large Language Models
           * LLM is an autoregressive model that predicts one word at a time, given the context
           * We can "translate" a patient history into a "long sentence" and generate the patient history as a sentence.
       * A recent concept is diffusion models. Deep learners sequentially find the noise vs. the truth and generate new data from these models

       * Generating data:
           * Binary data enables you to see something happen in the real data set and the synthetic data set.
           * Map the real data with the test data to generate synthetic data.
           * The different approaches: MeLD, HALO, Timeautodiff, SynTEG
           * These can also be used for other health data, like Tuberculosis and Cancer: 
               * Prediction AUCs, means (standard deviations), for models trained on synthetic data and tested on real data for predicting tuberculosis and cancer ≥6 months after enrolment.
       * Ways of measuring privacy risks of synthetic data:
           * Good privacy protection should have a score close to 0
           * Attribution Disclosure: If the attacker has partial information on patients in the training dataset, then the release of data allows learning more about the patients.
           * Membership Inference: Attacker has information about a set of patients and can make an inference about whether their data is in the training data.
           * NNAA: Measures overfitting by comparing how often a patient's nearest neighbor comes from the training set versus an external set.
       * **Challenges:**
           * ﻿﻿It's difficult to get associations between derived variables to closely resemble the original data. ﻿﻿e.g., time from ART initiation to death
           * ﻿﻿Incorporating time, especially if there is a wide variety in the number of visits in the datasets
           * ﻿﻿Continuous data: Models chasing outliers vs. failing to capture the range of data
           * ﻿﻿Sparse data, censored data, missing data - the goal is to create data close to the original data, and so even missing data is generated.
       * **Ethical Concerns:**
           * What are the incentives for medical institutions / principal investigators to share synthetic data?
               * Open Science.
               * Will good, publicly available synthetic data diminish value of the original data? - Personal thought is that original data would always be important.
           * ﻿﻿Could synthetic data expose a site's dirty laundry?
           * ﻿﻿Could synthetic data be used by bad actors in a harmful manner?
           * ﻿﻿How should we share synthetic HIV data?
               * ﻿﻿Freely downloadable to anyone, or tiered levels of access?
               * At CASS, users should submit concept notes so the use of data can be known, before shared.
           * ﻿﻿How do data privacy laws apply to synthetic data?
           * ﻿﻿What do people living with HIV think about synthetic data?
               * These are ongoing conversations.
           * Synthetic data:
               * May be useful for hypothesis generation. It needs to be high quality to do this, and the goal is to get here.

  **Questions (Open to the audience)**

   * Can we ensure synthetic datasets are accurate and representative of Africa's realities while addressing issues like privacy and bias?+1
       * Answer: That's the goal of synthetic data, but also the challenge. In our work, we're getting closer to generating synthetic datasets that are accurate, representative of our Latin American HIV research network, and preserve privacy. But these datasets may still not be accurate enough to use for hypothesis generation / hypothesis testing that I spoke about today.
   * How can synthetic data balance the need for open science and data sharing with the protection of patient confidentiality?
       * Answer: It's kind of a compromise. You're not sharing real data, so protection of patient confidentiality is good. But synthetic data are not as good as the original data.
   * In what ways can synthetic data accelerate HIV research and improve clinical trial design in African contexts?
       * Answer: I'm not sure about clinical trial design (although there is some interesting work being done with digital twins for clinical trials). With general HIV research, I feel that synthetic data allows more people to have access to data, and the more eyes on data, the more research progress.
   * How can we use AI and synthetic data to answer questions that we haven't yet thought about?
       * Answer: Possibly. That's kind of one of the goals of this work.
   * How do you ensure variability of data with synthetic generation? Sometimes when I do it at least with one distribution things for example with a dirichlet distribution get a bit stale?
       * Answer: I'm not sure I completely understand this question. We generate data from models fit to the original data but in a random manner, which ensures variability across replications. Dirichlet distributions are often used as priors for multinomial distributions, and I would expect you'd see good variability across replications. But perhaps if all of your data are assumed to follow multinomial distributions, then your simulated synthetic data could be limited.
   * I have question its good insight to use synthetic data specifically for sensitive issues like HIV to preserve privacy but here in ahri we are working on HIV data set which is available in large amount but with many missing values but with regard to the privacy we are planning to anonymize and it is longitudinal data and some variables are not filled as part of missing, is it right using synthetic data and generalizing to predict diseases conditions associated with HIV and any treatment failures,,,and is it right to use it for academic purpose (thesis)
       * Answer: People have been replacing missing data with "synthetic" data for many years using multiple imputation techniques, which have been well-accepted. So if I understand this question correctly, I think it is fine to do this.
   * With the challenges with generating survival synthetic data, are there good methods for generating longitudinal data beyond just crossectional data?
       * Answer: Yes, they are getting better, and we;re hoping to publish some of the methods currently being developed. MeLD is the approach that's currently best, based on our experience at least.
   * Given that synthetic data is generated rather than observed, how reliable are conclusions drawn from it when applied to real-world scenarios, particularly in critical areas like health, agriculture, or policy-making? What validation strategies do you recommend to ensure these conclusions are trustworthy?
       * Answer: This is what we are currently investigating in our HIV context. Is our synthetic data reliable enough to be used by others to generate hypotheses that are worth studying using the real data? I don't think synthetic data will ever replace real data, but as synthetic data become more reliable, they will be more useful. 
   * Can I reproduce the same data over and over again? 
       * Answer: You would have to generate a random seed and preserve it to use over and over again.


00:55-00:60[⏰ 5min] Closing remarks - Michael












