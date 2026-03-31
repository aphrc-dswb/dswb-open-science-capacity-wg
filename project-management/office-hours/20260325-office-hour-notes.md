# Welcome to Data Science Without Borders Office Hour Call - AHRI Team with Steve Cygu

Date: March 25th, 2026

**Office Hour Challenge:**
- Presenting Team: AHRI
- Technical Lead: Steve Bicko Cygu
The AHRI team has presented the following challenges faced during the deployment of their hackathon
products:
1. Evaluation of unsupervised models
2. Best deployment strategies of applications between local machines and subdomains hosting on cPanel
Request: Share or demonstrate an effective method of addressing this topic.

**Attendees** 

- Betty
- Steve
- Yordanos
- Precious
- Domian
- Reinpeter
- Daffe
- Sington
- Abdoulaye
- Ousmane
- Belayneh
- Mulugeta
- Anicet
- Miranda
- Serena
- Michael O
- Martha
- Brenda
- Resa
- Mane
- Bash
- Valentine
- Rosa
- Yishak

## Notes

### 1. Evaluating Unsupervised Learning Models  

**Context (Betty):**  
- Team is already using unsupervised learning models across products  
- Current evaluation is indirect (e.g., “this % effective”)  
- Need for more **technical, reliable evaluation approaches**  

**Core challenge**  
- No labeled outcomes → cannot evaluate like supervised models  
- Focus shifts to:
  - Cluster quality  
  - Structure in the data  
  - Variance explained  

**Steve's Suggestions:**

**Silhouette Coefficient**  
- Measures how similar data points are within a cluster vs. other clusters  
- Range: **-1 to +1**  
  - Close to **+1** → strong, well-separated clusters  
  - Around **0** → random clustering  
  - Close to **-1** → poor clustering (wrong assignments)  
- What to aim for:
  - Values **greater than 0 and close to 1**  

**Elbow Method (K-means)**  
- Used to determine the **optimal number of clusters (K)**  
- Process:
  - Train model across multiple K values  
  - Compute **within-cluster variation** at each step  
- What to look for:
  - The point where there is the **largest drop (“jump”) in variation**  
  - That point = optimal number of clusters  

**PCA (Principal Component Analysis)**  
- Used for **dimensionality reduction**  
- Focus on:
  - **Cumulative explained variance**  
- Approach:
  - Reduce many variables → fewer components  
  - Check how much variation is retained  
- Rule of thumb:
  - ~**70%+ explained variance** is usually sufficient  

**Other mentions**  
- Davies–Bouldin Index (not deeply explored)  
- Method choice depends on:
  - Algorithm  
  - Data type  
  - Use case

 -------------

### 2. Deployment Challenges (Local + cPanel Setup)  

**Context (Betty):**  
- Frontend → hosted on **cPanel subdomain (shared hosting)**  
- Backend → running locally (Dockerized)  
- Issues:
  - No auto-sync between environments  
  - Manual uploads required for updates  
  - Limited access (depends on IT team)  
  - cPanel **does not support Docker**  

**Key limitation**  
- Shared hosting = no root access  
- Cannot install Docker  
- Cannot fully automate deployment  

### Recommended Deployment Flow (Ideal Setup)  - Steve

**General architecture**  
- Codebase → GitHub  
- Separate layers:
  - Application code  
  - DevOps (build + images)  
  - Production (deployment)  

**Typical workflow**  
- Build Docker image locally  
- Test locally  
- Push to Docker Hub  
- Pull image on server  
- Run container  

**Docker Hub**  
- Acts like GitHub for Docker images  
- Stores:
  - Versions  
  - History  
- Benefits:
  - Easy rollback  
  - Consistent deployments  
  - Centralized source of truth  

**Automation**  
- Can be done using:
  - Bash scripts / Makefiles  
  - GitHub Actions / Jenkins  
- Enables:
  - Auto-build  
  - Auto-deploy  
  - Reduced manual work  

### Workaround for cPanel (NGINX Approach) - Steve

**Suggested approach**  
- Run Dockerized app **outside cPanel**  
- Use **NGINX reverse proxy** to:  
  - Map app to subdomain  
  - Route traffic from cPanel → external server  

**How it works**  
- Application runs on a server (local, VPS, or cloud)  
- Exposed via a port (e.g., `localhost:8088`)  
- NGINX maps:
  - Subdomain → application endpoint
    
**Why this helps**  
- Avoids Docker limitation in cPanel  
- Keeps existing domain setup  
- Enables more flexible deployment  

### Observations from Current Setup  

- Manual frontend deployment  
- No CI/CD pipeline  
- Dependency on IT team slows iteration  
- Frontend and backend not synchronized  

## Next Steps  

- **Betty and AHRI Team:**  
  Explore using **NGINX reverse proxy** to map Dockerized applications running on another server to the current subdomain  

- **Betty / RE Team:**  
  Evaluate moving to a **VPS**, considering cost and long-term sustainability  

- **Steve:**  
  Share code/examples for:
  - Silhouette Coefficient  
  - Elbow Method  
  (if needed by the team)  

---

## Key Takeaway  

- Unsupervised models are evaluated through **structure and clustering quality**, not accuracy  
- Current deployment issues are due to **shared hosting constraints**  
- A more scalable setup = **Docker + Docker Hub + NGINX (or VPS)**  

**Notes:** 
- This was our first iteration of the DSWB Office Hours.
- ChatGPT was used to summarise notes and improve sentence structure.
