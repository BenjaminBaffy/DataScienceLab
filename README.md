Short description: Implement a different baseline and/or novel algorithms for (offline) customer profiling (i.e. clustering) based on customer behavior in financial systems. Customers are small and medium enterprises with behavior descriptors: logins in certain banking systems, transfers to partners, invoices issued.

Instructions: Download the dataset from Teams. Get familiar with the dataset which contins diverse data about companies. Select the categorical features. Peform feature selection. Cluster the company descriptions by utilizing the Gower distance, DBSCAN and at least one more applicable clustering algorithm (e.g., agglomerative Hierarchical Cluster Analysis (HCA)). Measure and compare the performance of the clustering approaches - note that silhouette is not appropriate for all clustering algos.

Note: Do not share the dataset with anybody as it is a private dataset generated based on real-life company information.

Report length: 6-7 pages, LNCS format

Initial references:
https://towardsdatascience.com/clustering-on-numerical-and-categorical-features-6e0ebcf1cbad


1. Imre Lendak will share a dataset and a bit more detailed task description.
2. We have hard milestones meet them in all cases.
3. Next milestone is March 31. Put together an Overleaf report with literature review and initial data analysis. Create a Jupyter with initial analytics and modeling as well.
4. We expect to see 10+ days put into the DS Lab. We do not accept 5-line solutions submitted at the very end of the semester.
5. We will have bi-weekly meetings. I will send out a Doodle to choose a timeslot suitable for everybody.
6. If urgent and absolutely necessary, we will be able to schedule additional 1-to-1 meetings.


March 31. Deadline
  - Overleaf report
  - Data description (0.5 page)
  - References
  - Initial analytics

May 15. Deadline
  - Data understanding
  - Sound methodology chosen
  - Initial documentation
  - Github repo for data pre-processing and maybe method implementation as well

June 10. Deadline
  - Experiments and tests 
  - Final report 

&nbsp; 
---

Final sumary

- Task - Clustering of costumer data
  - Mixed data
  - Gower distance
    - Different similarity measure per type of data
  - DBSCAN and Agglomerative clustering
  - Silhouette score

- Dataset - Costumers (companies) of a bank
  - Columns
    - About the costumer
    - About the service
    - Numerical, categorical and date type
  - Unique values
  - Missing values

- Cleaning and transformation
  - Removed almost empty rows and columns
  - Removed unique or almost unique columns
  - Transformed date types
    - Numerical 0-1 range
    - Binary (older than 1 year)
    - Multiple bins
  - Post-code to county
  - Normalising numerical data
    - Sensitive to outliers
  - Removing outliers (numerical)
  - Standardising numerical data
    - Robust to outliers

- Feature selection
  - Based on variance
  - Using a wrapper method
    - with DBSCAN and the silhouette score
  - Feature subset suggested by Prof. Lendák

- Clustering
  - DBSCAN - Best
    - Wrapper method with standardised numerical: 
      - 2 clusters
      - Probably based on the date of account creation (within one year or older)
  - Agglomerative - Best
    - Suggested feature set
      - 3 clusters
      - Based on the last activity date (within one month, 3 months or older)

