### **Project: Clustering-Analysis-of-Earthquake-and-Weather-Datasets**  

![image](https://github.com/user-attachments/assets/11eeb600-0ad4-4c0b-9734-e7af42027395)

![image](https://github.com/user-attachments/assets/d5e85edc-9529-4e70-9e8e-f392f5d7ad80)

![image](https://github.com/user-attachments/assets/e477123d-896b-43d1-8764-f9b421a14017)

![image](https://github.com/user-attachments/assets/00524bd6-3dc6-4076-8ad4-58080173e234)

![image](https://github.com/user-attachments/assets/57dae949-0710-46cc-a803-5808416ae099)

![image](https://github.com/user-attachments/assets/a1f53942-7347-41df-8b20-49755affbbbb)

![image](https://github.com/user-attachments/assets/872c3b85-458b-474c-adfd-afa73fec8efb)


In the project we will use the  Earthquake  dataset, EQ dataset for short and the Houston Weather Dataset, or HWD for short. The first and last attribute of the HWD should be ignored when clustering this data set; the last attributes denotes a class variable which will be used in the post analysis of the clusters generated by running K-means, and DBSCAN.

The tasks are as follows:  

Task 1. **Purity Function Implementation:** A `purity()` function is developed to compute the purity of clustering results using ground truth class labels. The function accounts for outliers and returns either a single purity value or a vector of purity and the percentage of outliers when specified.  

Task 2. **Average Sum of Square Error (ASSE) Function:** A `asse()` function is written to calculate the average sum of squared differences between object attribute values and cluster means. This function evaluates clustering quality, excluding outliers when applicable.  

Task 3. **Cluster Visualization for the EQ Dataset:** A visualization procedure is created to map EQ dataset clusters using latitude and longitude, including plotting cluster boundaries for clarity.  

Task 4. **K-means Clustering for EQ Dataset:** K-means clustering is performed on the EQ dataset with values of k set to 5, 9, 13, and 17, using latitude and longitude attributes. The ASSE values for magnitude and depth are computed for each clustering and visualize the clusterings with the best results for each attribute.  

Task 5. **K-means Clustering for HWD Dataset:** K-means clustering with k=3 is applied on the HWD dataset 10 times, excluding the `Date` and `Class` attributes. Purity score is computed using the `purity()` function, then we create boxplots for cluster attributes (e.g., temperature, rainfall, humidity), and interpret the clusters based on centroids and attribute distributions.  

Task 6. **DBSCAN Clustering for HWD Dataset:** DBSCAN clustering is performed on the HWD dataset to generate between 2 and 15 clusters while maintaining outliers below 20%. The purity score is then computed and results are compared with the K-means clustering from task 5.  

Task 7. **Optimized DBSCAN Clustering for EQ Dataset:** A search procedure is created to identify optimal `MINPOINTS` and `epsilon` parameters for DBSCAN clustering on the EQ dataset, minimizing ASSE for the depth attribute. We then visualize the best clustering, report its ASSE score, and compare it with the K-means results for k=5, 9, 13, and 17.  

