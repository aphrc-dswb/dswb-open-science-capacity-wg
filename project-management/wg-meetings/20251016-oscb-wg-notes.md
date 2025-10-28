# Open Science and Capacity Building Working Group Meeting
 
Date: October 16th, 2025 
 
## 👋  Icebreaker 
 
*(Getting to know each other and this Etherpad for collaborative notes)*
 
**Name** 

   * Rachel
   * Precious
   * Oumou - Speaker
   * Moctar
   * Yaa
   * Belayneh
   * Daffe
   * Gadiaga - Ministry of Health
   * Joshua
   * Winston
   * Ousmane
   * Shamsdine
   * Magatte
   * Interpreters: Vincent/Gumba
   
## 📣 Agenda:

**Before this meeting:**

   * We are hosting coworking calls every week on Wednesdays: https://annuel2.framapad.org/p/dswb-coworking-calls

**During this meeting: Agenda**

   * As a result of the upcoming hackathon, which the IRESSEF team is partnering with the Senegalese Ministry of Health, some representatives
     will be leading a session on the DHIS2 tool to be used during the hackathon. The session is to be led by Madame Gueye from the Senegalese Ministry of Health.

### Notes

  - Dr Gadiaga: Head of Public Health Dept in Ministry of Health
    - Did a brief vote of thanks to the technical partners.
  - Dr Oumou
    - Is doing a demo of the DHIS2 tool.
    - A platform in use by the ministry since 2012
      - A data entry option is available.
      - Controls are also set to enable the data put in place to a high quality.
      - The various datasets collected are categorised according to location, and type of data collected.
        - Only aggregated data are collected.
      - The dashboard enables you see the data submitter, the time submitted, and other details regarding the data. There is also a limit Min-Max option, which enables the team to continue improving data quality.
      - The platform enables reports to be generated automatically: you can use tables, or graphs, etc
  - Shamsudeen: Head of IT
    - Technology used:
      - It is managed by Java
      - PostGreSQL is what handles the database
      - API RESTFul has been integrated for extensions
      - Architecture:
        - 3-tier Architecture: Web Client - Tomcat Sever - Base PostGreSQL
        - Apache/Nginx as a reverse proxy
        - Horizontal scalability (load balancing, replication)
        - Deployment on physical, virtual, or cloud servers
      - Authentication
        - Authentication: Username/password, OAuth2, OpenlD Connect
        - HTTPS communication required
        - Detailed role and permission management
        - Audit logs and access monitoring
        - Possible integration with a VPN or firewall
      - Interoperability
        - Complete RESTful API (JSON, XML)
        - Access to entities: dataElements, datasets, indicators, events, etc.
        - Integration with OpenMRS, DME, and other DHIS2
        - Automation via scripts Python/Airflow
      - Performance and Scalability
        - PostgreSQL optimization (index, vacuum, memory tuning)
        - Apache proxy cache
        - Monitoring: Grafana, Prometheus, DHIS2 Monitoring App
        - Deployment via Docker (advised to use in developer mode) or DHIS2 Tools NG
      - Customization and extensions
        - React application development via DHIS2 App Platform
        - Adding forms, QR codes, and custom dashboards
        - Configurable validation rules and program indicators
      - Deployment and Maintenance
        - Environment: Ubuntu LTS, Tomcat 9/10, PostgreSQL 14+
        - Tomcat memory and log configuration
        - Automatic backups and regular updates
        - Deployment on LXC, Docker, Cloud (AWS, Azure, GCP)
      - Conclusion
        - DHIS2: A robust, interoperable, and scalable platform
        - Adapted to national digital health needs
        - A strategic tool for data-driven decision-making

### Notes from previous meeting

   * We had an external webinar, on FAIR Data Sharing and Federated Analysis.  

More details can be found [here](https://github.com/aphrc-dswb/dswb-open-science-capacity-wg/blob/main/project-management/wg-meetings/20251002-oscb-wg-notes.md). 
