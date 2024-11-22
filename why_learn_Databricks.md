In this blog, I will talk about what are Spark Platforms and why they are completing Spark and why you should learn one ?

### What Are Spark Platforms?  

- Cloudera Hadoop Platform  
- Amazon EMR  
- Azure HDInsight  
- Google Dataproc  
- Databricks Platform  

To fully understand these platforms and why they were created, it is important to recognize that **Spark is just a compute engine**, which means it only performs computations. Many additional components are required to build a complete solution.  

### What Is Missing?  

1. **Data Storage Infrastructure**:  
   Spark can read and write data, but it does not store data. It interacts with external storage systems like HDFS, S3, Oracle databases, or Postgres databases, but does not provide its own storage system.  

2. **Metadata Catalog**:  
   Spark includes a basic metadata catalog, but it is neither robust nor practical for large-scale enterprise use.  

3. **Cluster Management**:  
   Spark does not manage the nodes in a cluster. The user should setup the whole cluster all alone. 

4. **Automation APIs and Tools**:  
   In enterprise environments, automation is crucial, but Spark does not offer built-in tools or APIs for automating workflows or ETL pipelines.  

### Why Spark Platforms?  

Spark platforms address these gaps by providing additional infrastructure and features. For example:  

#### Databricks Platform  
- **Storage System**: Databricks has its own proprietary storage system (DBFS).  
- **Metadata Catalog**: Provides a robust and integrated metadata catalog.  
- **Cluster Management**: Databricks starts and manages the cluster in the background.  
- **Automation**: Offers tools to automate ETL pipelines and workflows.  

This makes Spark platforms essential for enterprise-level usage. Among these platforms, Databricks stands out. But why choose Databricks over others?  

### Comparing Spark Platforms  

- **Cloudera Hadoop Platform**: Designed for on-premises clusters (not cloud-based).  
- **Amazon EMR, Azure HDInsight, Google Dataproc**: These platforms use Hadoop in the background with YARN as the resource manager and HDFS for storage.  
- **Databricks Platform**:  
  - Uses its proprietary storage system (DBFS).  
  - Employs Spark's standalone cluster manager rather than YARN.  
  - Runs exclusively in the cloud (no on-premises option).  

