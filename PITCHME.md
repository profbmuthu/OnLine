---
<!-- .slide: data-autoslide="10000" -->
### Hadoop Administration
<br>
<span style="color:#e49436">Play Hadoop</span>
<br>
<span style="color:gray">-</span>
<br>
<span style="color:#e49436">Dr.B.Muthukumaran</span>
---

<!-- .slide: data-autoslide="2000" -->

## Agenda <span style="color: #e49436">Sessions</span>
### <span class="fragment" data-fragment-index="1" data-autoslide="2000"> Hadoop Management <span style="color: #666666">.</span>
<br>
### <span class="fragment" data-fragment-index="2" data-autoslide="3500">Administration<span style="color: #e49436">Management</span>. and <span style="color: #e49436">Guidelines</span>.</li>

---
<!-- .slide: data-autoslide="2000" -->

### Agenda
- Introduction to Big data 
- limitations of existing solutions 
- Hadoop architecture 
- Hadoop components and ecosystem, data loading & reading from HDFS 
- Replication rules 
- Hadoop cluster administrator: Roles and responsibilities

---

<!-- .slide: data-autoslide="2000" -->
### Agenda
- Hadoop server roles and their usage
- Hadoop installation and initial configuration
- Pseudo-distributed mode, multi-node Hadoop cluster
- Understanding working of HDFS  

---

<!-- .slide: data-autoslide="11000" -->

### <span style="color: #e49436">What is data?</span>
- Data is information 
- It is  translated into a form that is more convenient to move or process. 
- From a business context, data is information converted into binary digital form.  
- Data comes in different shapes, sizes, and granularity. 
- It also comes with a lot of uncertainty attached.

---
<!-- .slide: data-autoslide="11000" -->
### <span style="color: #e49436">What is dataset?</span>
- Data is usually collected as data points. 
- Means totals, averages, and medians are only a small part of what a data point is about.  
- Connection between data and what it represents is key to visualization. 
- Data is the key to data analysis and deeper understanding.

---
<!-- .slide: data-autoslide="11000" -->

### <span style="color: #e49436">What is dataset?</span>
- Data set is a snapshot of data in time 
- It captures something that moves and changes. 
- It refers to data selected and arranged in rows and columns. 
- Column represents a particular variable.  
- Row corresponds to a given member of the data set in question. Each value is known as a datum. 

---
<!-- .slide: data-autoslide="11000" -->

### <span style="color: #e49436">What is dataset?</span>
- Data set may comprise data for one or more members, corresponding to the number of rows 
- Data set collection of data points forming aggregates and statistical summaries. 
- Data set generates your  means, medians, and standard deviations.

---
<!-- .slide: data-autoslide="11000" -->

### <span style="color: #e49436">Data Generation?</span>
- Data is being generated faster and faster as more and more people take to the Web. 
- Customers generate data of all kinds, 
- Generated data is difficult to control.  
- Information is now widely available on external events such as market trends, industry news, and competitors’ movements. 
- Led to increasing interest in methods for extracting useful information and knowledge from data—the realm of data science.

---

### <span style="color: #e49436">Types of Data</span>? 
- Data regardless of type, location, and source increasingly has become a core business asset for an enterprise 
- It is now categorized as belonging to two camps:
+ Internal data (enterprise application data) and
+ External data (e.g., web data)

---
<!-- .slide: data-autoslide="2000" -->

### <span style="color: #e49436">Types of Data</span>? 

- There are two types of data in the real world:
    + Static data. (Collected Data). 
    + The volume of static data, for example national census data and human genomic data, will not change over time.

---
<!-- .slide: data-autoslide="2000" -->

### <span style="color: #e49436">Types of Data</span>? 

    + Dynamic data (Data being served continuously) 
    + Dynamic data, such as streaming log data and social network streaming data, the volume increases over time.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> BigData.</span>

- Hadoop software are revolutionizing the Internet services community 
- Achieved by building scalable systems infrastructure for data intensive applications. 
- Business best practices” - increasingly towards basing decisions off data  rather than instinct and theory

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> BigData.</span>
- Corporate thirst for systems that can manage, process, and granularly analyze data is becoming insatiable. 
- Venture capitalists are very much aware of this trend, 
- Funded no fewer than a dozen new companies in recent years 
- e.g., Netezza, Vertica, DATAllegro, Greenplum, Aster Data, Infobright, Kickfire, Dataupia, ParAccel, and Exasol), 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> BigData.</span>
- Big Data is data in large sizes 
- It goes beyond the ability of commonly used software tools to collect, manage, and process within a tolerable elapsed time. 
- Big data refers to datasets whose size is beyond the ability of typical database software tools
- Used  to capture, store, manage, and analyze data. 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> BigData.</span>
- Big data essentially means datasets that are too large for traditional data processing systems.
- It is data that exceeds the processing capacity of conventional database defined systems. 
- It is too big, moves too fast, or doesn’t fit the strictures of conventional database architectures. 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> BigData.</span>

- Valuable patterns and information, previously hidden because of the amount of work required to extract them. 
- It applies to information that can’t be processed or analyzed using traditional processes or tools. 
- The value of big data to an organization falls into two categories: analytical use and enabling new products

---
<!-- .slide: data-autoslide="2000" -->

### Characteristics of <span style="color: #e49436">  bigdata</span>
- Big data has become viable 
- Cost effective approaches have emerged to tame the volume, velocity, variety and variability of massive data. 
- Three Vs of volume, velocity, and variety are commonly used 
- Helpful lens through which to view and understand the nature of the data 
- Helpful to understand software platforms available to exploit them. 

---
<!-- .slide: data-autoslide="2000" -->
### Data <span style="color: #e49436"> Volume</span>
- Amount of data being generated is increasing day by day. 
- Rate of increase of data is accelerating continuously. 
- Volume of data being made publicly available increases every year. 

---
<!-- .slide: data-autoslide="2000" -->
### Data <span style="color: #e49436"> Volume</span>
- Organizations no longer have to merely manage their own data. 
- As data volume increases, the value of different data records will decrease in proportion to age, type, richness, and quantity among other factors. 

---
<!-- .slide: data-autoslide="2000" -->
### Data <span style="color: #e49436">  Volume</span>
- Data generated from emails to Facebook posts, from purchase histories to web links, is contributing to the growth of data. 
- Current challenge is in extracting value from this data.  
- Sometimes this means particular data elements, and at other times, the focus is instead on identifying trends and relationships between pieces of data. 
- Includes the current data volume

---
<!-- .slide: data-autoslide="2000" -->
### Data <span style="color: #e49436">  Velocity.</span>
- Velocity of data is the measure of how fast the data is coming in.  
- Data volume measures the amount of data available to an organization.
- Data velocity measures the speed of data creation, streaming, and aggregation.
- eCommerce has rapidly increased the speed and richness of data used for different business transactions (for example, web-site clicks). 
- Data velocity management is much more than a bandwidth issue; it is also an ingest issue.

---
<!-- .slide: data-autoslide="2000" -->
### Data <span style="color: #e49436"> Velocity.</span>
- Earlier companies analyzed data using a batch process. 
- A chunk of data, is submitted as a job to the server. The job gets executed and results are delivered. 
- That scheme works when the incoming data rate is slower than the batch processing rate and when the result is useful despite the delay. 

---
<!-- .slide: data-autoslide="2000" -->
### Data <span style="color: #e49436"> Velocity.</span>

- New sources of data such as social and mobile applications, the batch process breaks down. 
- Data is streaming into server in real time, in a continuous fashion 
- Result is only useful if the delay is very short

---
<!-- .slide: data-autoslide="2000" -->
### Data <span style="color: #e49436"> Variety.</span>
- Data can help inform intelligent policy making 
- It provides innovative kindling for investigative journalism, 
- Even when data is freely available, it can be shared using data formats that are touch for consuption.

---
<!-- .slide: data-autoslide="2000" -->
### Data <span style="color: #e49436"> Variety.</span>

- Data variety is a measure of the richness of the data representation – text, images video, audio, etc. 

- From an analytic perspective, it is probably the biggest obstacle to effectively using large volumes of data. 

-Incompatible data formats, non-aligned data structures, and inconsistent data semantics represents significant challenges that can lead to analytic sprawl.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> Data Versatility.</span>
- Versatility refers to the adaptability of a system to analytical queries of varying complexity. 
- Versatility also refers to system flexibility in terms of query languages supported, and control in terms of data preparation, placement and management. 
- Within this data lie valuable patterns and information, previously hidden because of the amount of work required to extract them

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> Bigdata Challenges</span>
- Increasingly, organizations today are facing more and more Big Data challenges. 
- The emergence of big data into the enterprise brings with it a necessary counterpart: agility.
- As data sizes grow, the concept of providing a single repository for all this data is not always the most practical solution.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> Benefits of Bigdata</span>
- Big data analytics reveals insights hidden previously by data too costly to process, 

- It can be peer influence among customers, revealed by analyzing shoppers’ transactions and social and geographical data in real time. 

- Meaning of “real time” varies depending on the context in which it is used. 

- Real-time denotes the ability to process data as it arrives, 

- It does not permit storing the data and retrieving it at some point in the future 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> Benefits of Bigdata</span>
-  For  an online merchant, “the present” means the attention span of a potential customer. 

-  Processing time of a transaction exceeds the customer’s attention span, the merchant doesn’t consider it real time.

-  For an options trader,  real time means milliseconds. For a guided missile, real time means microseconds. 

-  Real-time big data analytics is an iterative process involving multiple tools and systems.

---
<!-- .slide: data-autoslide="2000" -->

##  <span style="color: #e49436">Session</span>
### <span class="fragment" data-fragment-index="1" data-autoslide="2000"> Hadoop <span style="color: #666666">.</span>
<br>

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> Hadoop</span>
- Hadoop is based on the Google paper on MapReduce 

- Paper published in 2004, with development from  2005. 

- Hadoop was developed to support the open-source web search engine project called Nutch.

- Hadoop separated from Nutch and became its own project under the Apache Foundation. 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> Hadoop</span>
- Hadoop is the best–known MapReduce framework in the market. 
- Companies have grown around Hadoop to provide support, consulting, and training services for the Hadoop software. 
- At its core, Hadoop is a Java–based MapReduce framework.  
- Hadoop remained a system in which users submitted jobs that ran on the entire cluster.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> Hadoop</span>
-  Jobs would be executed in a First In, First Out (FIFO) mode. 
- However, this lead to situations in which a long-running, less important job would hog resources and not allow a smaller yet more important job to execute. 
- To solve this problem, more complex job schedulers in Hadoop, such as the Fair Scheduler and Capacity Scheduler were created. 
- But Hadoop still had scalability limitations that were a result of some deeply entrenched design decisions resulting in Hadoop 2.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> Hadoop Hive </span>(1/2)
- Hadoop Users realized that developing MapReduce programs is a very programming-intensive task, which makes it errorprone and hard to test. 
- There was a need for more expressive languages such as SQL 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> Hadoop Hive </span>(2/3)

- Required to enable users to focus on the problem instead of low-level implementations of typical SQL artifacts 
- Apache Hive evolved to provide a data warehouse (DW) capability to large datasets. 
- Users can express their queries in Hive Query Language, which is very similar to SQL. 

---

<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> Hadoop Hive </span>(3/3)
- The Hive engine converts these queries to low-level MapReduce jobs transparently. 
- More advanced users can develop user-defined functions (UDFs) in Java. 
- Hive also supports standard drivers such as ODBC and JDBC. 
- Hive is also an appropriate platform to use when developing Business Intelligence (BI) types of applications for data stored in Hadoop.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> Hadoop Pig </span> 
- Motivation for Pig was similar to Hive 
- Hive is a SQL-like language, which is declarative. 
- Pig is a procedural language that works well in data pipeline scenarios. 
- Pig appeals to programmers who develop data-processing pipelines  
- It is also an appropriate platform to use for extract, load, and transform (ELT) types of applications.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Hadoop Hbase</span>
- All the preceding projects, including MapReduce, are batch processes. 
- There is a strong need for real–time data lookup in Hadoop. 
- Hadoop did not have a native key/value store. 
- Consider a Social Media site such as Facebook. 
- If you want to look up a friend’s profile, you expect to get an answer immediately (not after a long batch job runs).

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> Hadoop</span>
- Hadoop is a distributed data store. 

- Reliability of data store, coupled with its flexibility in running multiple processing frameworks makes it an ideal choice. 

- Characteristic of Hadoop - Store any type of data as is, without placing any constraints on how that data is processed.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> Hadoop</span>

- Schema-on-Read. 
  + Refers to the fact that raw, unprocessed data can be loaded into Hadoop, 
  + Structure imposed at processing time 
  + based on the requirements of the processing application.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436"> Hadoop</span>

- Schema-on-Write. 
  + Used with traditional data management systems. 
  + Such systems require the schema of the data store to be defined before the data can be loaded. 
  + Leads to lengthy cycles of analysis, data modeling, data transformation, loading, testing, 
  
---
<!-- .slide: data-autoslide="2000" -->

##  <span style="color: #e49436">Session</span>
### <span class="fragment" data-fragment-index="1" data-autoslide="2000"> HDFS <span style="color: #666666">.</span>
<br>

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">HDFS</span>
- HDFS is Hadoop distributed file system. 
- Designed to run on commodity hardware. 
- Built to support high throughput, streaming reads and writes of huge files. 
- Highly fault-tolerant 
- Designed to be deployed on low-cost hardware. 


---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">HDFS</span>


![HDFS Architecture](https://hadoop.apache.org/docs/r2.7.2/hadoop-project-dist/hadoop-hdfs/images/hdfsarchitecture.png)

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">HDFS</span>
- Offers centralized, low-latency access to large file systems. 
- It has many similarities with existing distributed file systems. 
- Relaxes a few POSIX requirements 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">HDFS</span>

- Enables streaming access to file system data. 
- Was originally built as infrastructure for the Apache Nutch web search engine project. 
- It is now an Apache Hadoop subproject. 

---
<!-- .slide: data-autoslide="2000" -->
###  <span style="color: #e49436">Goals </span>
- Large Data Sets 
+	Applications that run on HDFS have large data sets. 
+	A typical file in HDFS is gigabytes to terabytes in size. Thus, HDFS is tuned to support large files. 
+	It should provide high aggregate data bandwidth and scale to hundreds of nodes in a single cluster. 
+	It should support tens of millions of files in a single instance. 

---
<!-- .slide: data-autoslide="2000" -->
###  <span style="color: #e49436">Goals</span>
- Hardware Failure 

  + Hardware failure is the norm rather than the exception. 
  + HDFS instance may consist of hundreds or thousands of server machines.
  + Huge number of components interact 

---
<!-- .slide: data-autoslide="2000" -->
###  <span style="color: #e49436">Goals</span>
- Hardware Failure 

  + Each component has a non-trivial probability of failure 
  + Some component of HDFS is always non-functional. 
  + Detection of faults and quick, automatic recovery from them is a core architectural goal of HDFS. 

---
<!-- .slide: data-autoslide="2000" -->
###  <span style="color: #e49436">Goals</span>
- Streaming Data Access 
    + Applications on HDFS need streaming access to data sets. 
    + HDFS is designed more for batch processing rather than interactive use by users. 
    + Emphasis is on high throughput of data access rather than low latency of data access. 
    + POSIX imposes hard requirements that are targeted for HDFS. 
    + POSIX semantics in a few key areas has been traded to increase data throughput rates. 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">HDFS Similarities</span>
- HDFS has many similarities to a traditional file system. The following are some of them:
   + Files are stored in blocks. 
   + Metadata is available, which keeps track of filenames to block mapping.
   + It also supports the directory tree structure, as a traditional file system.
   + It works on the permission model. 
   + You can give different access rights on the file to different users.

---
<!-- .slide: data-autoslide="2000" -->
###  <span style="color: #e49436">HDFS Differences</span>
-  Very low storage cost per byte: 
   + HDFS uses commodity storage 
   + Shares the cost of the network it runs on with other systems of the Hadoop stack. 
   + Reduces the total cost of ownership. 
   + Allows an organization to store the same amount of data at a very low cost compared to traditional NAS or SAN systems.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">HDFS Differences</span>
- Block size for the data: 
   + Traditional file systems generally use around 8 KB block size for the data, 
   + HDFS uses larger block size of data. 
   + Block size in HDFS is 128 MB, 
   + Admin can raise it to 1 GB or higher. 

---
<!-- .slide: data-autoslide="2000" -->
###  <span style="color: #e49436">HDFS Differences</span>
- Larger block size ensures that the data can be read and written in large sequential operations. 
- It can improve performance 
- it minimizes drive seek operations, especially when performing large I/O streaming operations.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">HDFS Differences</span>
-  Data protection mechanisms: 
   + Traditional file systems use specialized data storage for data protection. 
   + HDFS replicates each block to multiple machines in the cluster. 
   + By default, it replicates the data block to three nodes. 
   + Ensures data reliability and high availability


---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">UseFul Features HDFS</span>

- File permissions and authentication.
- Rack awareness: to take a node’s physical location into account while scheduling tasks and allocating storage.
- Safemode: an administrative mode for maintenance.
- fsck: a utility to diagnose health of the file system, to find missing files or blocks.


---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">UseFul Features HDFS</span>

- fetchdt: a utility to fetch DelegationToken and store it in a file on the local system.
- Balancer: tool to balance the cluster when the data is unevenly distributed among DataNodes.
- Upgrade and rollback: it is possible to rollback to HDFS’ state before the upgrade in case of unexpected problems.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">UseFul Features HDFS</span>

- Secondary NameNode: 
  + performs periodic checkpoints of the namespace  
  + helps keep the size of file containing log of HDFS modifications within certain limits at the NameNode.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Name Node</span>
- Is a centralized service in the cluster operating on a single node. 
- Manages the file system namespace 
- This is file system tree and the metadata for all the files and directories are maintained. 
- It is the arbitrator and repository for all HDFS metadata. 
- Is designed in such a way that user data never flows through the Name Node. 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Name Node</span>
- Maintains and stores the namespace tree and the mapping of file blocks to Data Nodes 
- Two files are used
  + the namespace image
  + the edit log

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Name Node</span>
- File system metadata is stored on a metadata server. 
- Metadata operations may be handled by a single metadata server
- Cluster will configure multiple metadata servers as primary-backup failover pairs. 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Name Node</span>

- Includes the namespace, data location and access permissions. 
- Clients contact the Name Node for file operations 
- Common file system operations, such as open, close, rename, and delete. 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Heart Beat</span>
- Name Node does not store HDFS data 
- Maintains a mapping between HDFS file name, a list of blocks in the file, and the Data Node(s) on which those blocks are stored. 
- Periodically receives a Heartbeat and a Block report from each of the Data Nodes in the cluster. 
- Receipt of a Heartbeat implies that the Data Node is functioning properly. 
- Block report contains a list of all blocks on a Data Node.

---
<!-- .slide: data-autoslide="2000" -->
### Data <span style="color: #e49436">Node</span>
- Daemon responsible for storing and retrieving block data is called the datanode (DN). 
- Responsible for serving read and write requests from clients 
- Perform block operations upon instructions from name node. 

---
<!-- .slide: data-autoslide="2000" -->
### Data <span style="color: #e49436">Node</span>
- Stores HDFS blocks on behalf of local or remote clients. 
- Block is saved as a separate file in the node’s local file system. 
- Data Node abstracts away details of the local storage arrangement, 

---
<!-- .slide: data-autoslide="2000" -->
### Data <span style="color: #e49436">Node</span>
- Nodes do not have to use the same local file system. 
- Blocks are created or destroyed on Data Nodes at the request of the Name Node, which validates and processes requests from clients. 
- Clients communicate directly with Data Nodes in order to read or write data at the HDFS block level. 
---
<!-- .slide: data-autoslide="2000" -->
### Data <span style="color: #e49436">Node</span>
- Data node normally has no knowledge about HDFS files. 
- Scans through the local file system 
- Creates a list of HDFS data blocks corresponding to each of these local files 
- Sends this report to the Name node. 

---
<!-- .slide: data-autoslide="2000" -->
### Data <span style="color: #e49436">Node</span>
- Individual files are broken into blocks of a fixed size 
- Distributed across multiple DataNodes in the cluster. 
- The Name Node maintains metadata about the size and location of blocks and their replicas

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Client </span>
- Client is an api of applications. 
- Communicates with the Namenode for metadata 
- Once received it directly runs operations on the Datanodes. 
- If the operation is a MapReduce operation, the client creates a job and sends it to the queue. 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Client </span>
- JobTracker handles this queue. 
- Client perform file metadata operations such as create file and open file, at the NameNode over an RPC protocol and read/write the data of a file directly to DataNodes using a streaming socket protocol called the data-transfer protocol.

---
<!-- .slide: data-autoslide="2000" -->
###  <span style="color: #e49436">Blocks</span>
- Disk has a block size, 
- is the minimum amount of data that it can read or write. 
- File systems for a single disk build by dealing with data in blocks, 
- An integral multiple of the disk block size. 

---
<!-- .slide: data-autoslide="2000" -->
###  <span style="color: #e49436">Blocks</span>
- File system blocks are typically a few kilobytes in size 
- Disk blocks are normally 512 bytes. 
- Transparent to the file system user who is simply reading or writing a file of whatever length. 
- There are tools to perform file system maintenance, such as df and fsck, that operate on the file system block level.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Large blocks</span>
- HDFS, has the concept of a block
- Much larger unit 128 MB. 
- Files in HDFS are broken into block-sized chunks, 
- Stored as independent units.

---
<!-- .slide: data-autoslide="2000" -->
###  <span style="color: #e49436">Large blocks</span>
- Are large compared to disk blocks, the reason is to minimize the cost of seeks. 
- By making a block large enough, the time to transfer the data from the disk can be significantly longer than the time to seek to the start of the block. 
- The time to transfer a large file made of multiple blocks operates at the disk transfer rate. 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Large blocks</span>
- Having a block abstraction for a distributed filesystem brings several benefits. 
- File can be larger than any single disk in the network. 
- Take advantage of any of the disks in the cluster. 
- In fact, it would be possible, if unusual, to store a single file on an HDFS cluster whose blocks filled all the disks in the cluster

---
<!-- .slide: data-autoslide="15000" -->
### Large <span style="color: #e49436">Blocks </span>
- Making the unit of abstraction a block rather than a file simplifies the storage subsystem. 
- Storage subsystem deals with blocks, simplifying storage management and eliminating metadata concerns 
- Blocks are just chunks of data to be stored, 
- file metadata such as permissions information does not need to be stored with the blocks, so another system can handle metadata separately

---
<!-- .slide: data-autoslide="15000" -->
### Large <span style="color: #e49436">Blocks </span>
-  Blocks fit well with replication for providing fault tolerance and availability. 
- Insure against corrupted blocks and disk and machine failure, 

---
<!-- .slide: data-autoslide="15000" -->
### Large <span style="color: #e49436">Blocks </span>
- Block is replicated to a small number of physically separate machines.
- Block becomes unavailable, a copy can be read from another location in a way that is transparent to the client.
- Block that is no longer available due to corruption or machine failure can be replicated from its alternative locations 

---
<!-- .slide: data-autoslide="15000" -->
###  <span style="color: #e49436"> File system Namespace</span>

- Traditional local file systems support a persistent name space. 
- Local file system views devices as being locally attached, 
- The devices are not shared, and hence there is no need in the file system design to enforce device sharing semantics.

---
<!-- .slide: data-autoslide="15000" -->
###  <span style="color: #e49436"> File system Namespace</span>

- HDFS supports a traditional hierarchical file organization. 
- User or an application can create directories and store files inside these directories. 
- File system namespace hierarchy is similar to most other existing file systems 

---
<!-- .slide: data-autoslide="15000" -->
###  <span style="color: #e49436"> File system Namespace</span>

- Create and remove files, move a file from one directory to another, or rename a file. 
- HDFS does not yet implement user quotas or access permissions. 
- HDFS does not support hard links or soft links. 
- HDFS architecture does not preclude implementing these features

---
<!-- .slide: data-autoslide="15000" -->
###  <span style="color: #e49436"> Federation </span>

- HDFS Federation, introduced in the 2.x release series, 
- Allows a cluster to scale by adding name nodes, 
- Manages a portion of the file system namespace.

---
<!-- .slide: data-autoslide="15000" -->
###  <span style="color: #e49436"> Federation </span>

- Each name node manages a namespace volume
- Made up of the metadata for the namespace 
- Made up of a block pool containing all the blocks for the files in the namespace. 

---
<!-- .slide: data-autoslide="15000" -->
###  <span style="color: #e49436"> Federation </span>

- Namespace volumes are independent of each other 
- Name nodes do not communicate with one another 
- Failure of one name node does not affect the availability of the namespaces managed by other name nodes. 

---
<!-- .slide: data-autoslide="15000" -->
###  <span style="color: #e49436"> Federation </span>

- Block pool storage is not partitioned 
- Data nodes register with each name node in the cluster and store blocks from multiple block pools. 
- To access a federated HDFS cluster, clients use client-side mount tables to map file paths to name nodes. 
- This is managed in configuration using ViewFileSystem and the viewfs:// URIs.

---
<!-- .slide: data-autoslide="15000" -->
### Function of <span style="color: #e49436"> Configuration Files </span>

- Every machine in the Hadoop Cluster has its own set of configuration files. 
- Earlier  Hadoop had a single configuration file: hadoop-site.xml. 
- Subsequent versions of Hadoop split this file into multiple files based on functionality. 
- Additionally, there are two types of configuration files: 
   +  *-default.xml  
   +  *-site.xml. 

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Conf Files</span>
-  *-site.xml file configurations override the ones in the *-default.xml file. The *-default.xml files are read-only and are read directly from the JAR files in the classpath.
   +  core-default.xml Default core Hadoop properties. 
   + The file is located in the following JAR file: hadoop-common-2.2.0.jar (assuming version 2.2.0).

---
<!-- .slide: data-autoslide="15000" -->
###  <span style="color: #e49436">Conf Files</span>
   +  hdfs-default.xml Default HDFS properties. 
   + The file is located in the following JAR file: hadoop-hdfs-2.2.0.jar (assuming version 2.2.0).

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Conf Files</span>

   + mapred-default.xml Default MapReduce properties. 
   + The file is located in the following JAR file: hadoop-mapreduce-client-core-2.2.0.jar (assuming version 2.2.0).

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Conf Files</span>
   +  yarn-default.xml Default YARN properties. 
   + The file is located in the following JAR file: hadoop-yarn-common-2.2.0.jar (assuming version 2.2.0).

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> Installation Procedure</span>

- Required software for Linux include:
+  Java™ must be installed.
+  ssh must be installed and sshd must be running to use the Hadoop scripts that manage remote Hadoop daemons.

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> Core-site.xml  </span>
 
 <configuration>
 
     property>
     
     <name>fs.defaultFS</name>
     
     <value>hdfs://MastercomputerIP or localhost:9000</value>
     
     /property>
 
 </configuration>


---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> HDFS-site.xml  </span>
 
 <configuration>
 
    property>
    
        name>dfs.replication</name>
        
        value>1</value>
        
    /property>
 
 </configuration>


---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> MaRed-site.xml  </span>
 
 <configuration>
 
   property>

     name>mapreduce.framework.name</name>

     value>yarn</value>

    /property>
 
 </configuration>

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> Yarn-site.xml  </span>
 
 <configuration>
 
 name>yarn.resourcemanager.address</name>

    value>MastercomputerIP or localhost:8022</value>

     /property>

    property>

  name>yarn.resourcemanager-scheduler.address</name>

  value>MasterComputerIP or localhost:8021</value>

/property>
 
 </configuration>

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> Hadoop Env</span>

- set the java path in JAVA_HOME
- slaves:
- localhost

- Commands
 - >hadoop namenode -format
 - >start-all.sh
  
---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Failover</span>

- Transition from the active namenode to the standby is managed by failover controller. 
- There are various failover controllers, 
- The default implementation uses ZooKeeper to ensure that only one namenode is active.

---

<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Graceful </span> Failover

- Each namenode runs a lightweight failover controller process 
- Job is to monitor its namenode for failures and trigger a failover should a namenode fail. 
- Failover may also be initiated manually by an administrator, 
- Example, in the case of routine maintenance. 
- This is known as a graceful failover.

---
<!-- .slide: data-autoslide="15000" -->

### Ungraceful <span style="color: #e49436">Failover</span>

- Case of an ungraceful failover,  
- it is impossible to be sure that the failed namenode has stopped running. 
- Example, a slow network or a network partition can trigger a failover transition, even though the previously active namenode is still running and thinks it is still the active name node. 

 
---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436"> Fencing </span>

- The HA implementation goes to great lengths to ensure that the previously active namenode is prevented from doing any damage and causing corruption of data
- This is  known as fencing


---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436"> Stonith</span>

- “shoot the other node in the head,”
- Range of fencing mechanisms includes 
- revoking the namenode’s access to the shared storage directory 
- disabling its network port via a remote management command 
- Last resort, the previously active namenode can be fenced with a technique rather graphically known as STONITH, 
- Uses a specialized power distribution unit to forcibly power down the host machine.


---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">UseFul Features HDFS</span>

- Checkpoint node: 
 + performs periodic checkpoints of the namespace 
 + helps minimize the size of the log stored at the NameNode containing changes to the HDFS. 
 + Replaces the role previously filled by the Secondary NameNode 
 + NameNode allows multiple Checkpoint nodes simultaneously, as long as there are no Backup nodes registered with the system.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Checkpoint Node </span>

- When a NameNode starts up, it merges the fsimage and edits journal to provide an up-to-date view of the file system metadata. 
- The NameNode then overwrites fsimage with the new HDFS state and begins a new edits journal.
- Checkpoint node periodically creates checkpoints of the namespace. 
- Downloads fsimage and edits from the active NameNode, 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Checkpoint Node </span>

- Merges them locally, and uploads the new image back to the active NameNode. 
- Checkpoint node runs on a different machine than the NameNode 
- Its memory requirements are on the same order as the NameNode. 
- Checkpoint node is started by bin/hdfs namenode -checkpoint on the node specified in the configuration file.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Checkpoint Node </span>
- Location of the Checkpoint (or Backup) node and its accompanying web interface are configured 
- Checkpoint node stores the latest checkpoint in a directory that is structured the same as the NameNode’s directory. 
- This allows the checkpointed image to be always available for reading by the NameNode if necessary.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Checkpoint Node </span>

- Start of the checkpoint process on the Checkpoint node 
- Controlled by two configuration parameters.
   +  dfs.namenode.checkpoint.period, 
      + set to 1 hour by default 
      + specifies the maximum delay between two consecutive checkpoints

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Checkpoint Node </span>
- Controlled by two configuration parameters.
   +  dfs.namenode.checkpoint.txns, 
      + set to 1 million by default, 
      + defines the number of uncheckpointed transactions on the NameNode 
      + Will force an urgent checkpoint, even if the checkpoint period has not been reached.



---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Backup Node </span>

- Backup node provides the same checkpointing functionality 
- Maintains an in-memory, up-to-date copy of the file system namespace 
- It is always synchronized with the active NameNode state. 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Backup Node </span>

- Accepts a journal stream of file system edits from the NameNode 
- Applies the edits into its own copy of the namespace in memory, 
- Creates a backup of the namespace.
- As the Backup node maintains a copy of the namespace in memory, its RAM requirements are the same as the NameNode.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Backup Node</span>

- NameNode supports one Backup node at a time. 
- No Checkpoint nodes may be registered if a Backup node is in use. 
- Using multiple Backup nodes concurrently will be supported in the future.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Backup Node</span>

- Backup node is configured in the same manner as the Checkpoint node. 
- It is started with bin/hdfs namenode -backup.
- Location of the Backup (or Checkpoint) node and its accompanying web interface are configurable 
- Done with 
  + dfs.namenode.backup.address 
  + dfs.namenode.backup.http-address configuration variables.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Balancer</span>

- HDFS data might not always be be placed uniformly across the DataNode. 
- One common reason is addition of new DataNodes to an existing cluster. 
- While placing new blocks, NameNode considers various parameters before choosing the DataNodes to receive these blocks. 

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Balancer</span>
- Some of the considerations are:
  +  Policy to keep one of the replicas of a block on the same node as the node that is writing the block.
  +  Need to spread different replicas of a block across the racks 
  +  Cluster can survive loss of whole rack.

---
<!-- .slide: data-autoslide="2000" -->
### <span style="color: #e49436">Balancer</span>

  +  Cross-rack network I/O is reduced.
  +  Spread HDFS data uniformly across the DataNodes in the cluster.
  +  HDFS provides a tool for administrators that analyzes block placement and rebalanaces data across the DataNode.

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436"> Standard File formats </span>

- Text data
- Common use of Hadoop is the storage and analysis of logs such as web logs and server logs. 
- Such text data, of course, comes in many other forms: CSV files, or unstructured data such as emails

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436"> Standard File formats </span>

- Structured text data
- Specialized form of text files is structured formats such as XML and JSON. 
- Present special challenges with Hadoop since splitting XML and JSON files for processing is tricky, 
- Hadoop does not provide a built-in InputFormat for either. 
- JSON presents even greater challenges than XML, since there are no tokens to mark the beginning or end of a record.


---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436"> Standard File formats </span>
- Binary data
- Text is typically the most common source data format stored in Hadoop, 
- Also use Hadoop to process binary files such as images. 
- Storing and processing binary files in Hadoop, using a container format such as SequenceFile is preferred.



---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436"> Hadoop File formats </span>
- Splittable compression
- Support common compression formats and are also splittable.  
- The ability to split files can be a key consideration for storing data in Hadoop 
- Allows large files to be split for input to MapReduce and other types of jobs. 

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436"> Hadoop File formats </span>
- Agnostic compression
- File can be compressed with any compression codec, 
- Readers need not know the codec. 
- Codec is stored in the header metadata of the file format

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> File Based Storage</span>

- SequenceFile format is one of the most commonly used file-based formats in Hadoop,
- Every SequenceFile uses a common header format 
- Contains basic metadata about the file, 
  + compression codec used, key and value class names, user-defined metadata, and a randomly generated sync marker.

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> File Based Storage</span>

- Other file-based formats are available,  MapFiles, SetFiles, ArrayFiles, and BloomMapFiles.
- Three formats available for records stored within SequenceFiles

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> File Based Storage</span>

- Uncompressed
- uncompressed SequenceFiles don’t provide any advantages over their compressed alternatives
- They’re less efficient for input/output (I/O) and take up more space on disk than the same data in compressed form.

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> File Based Storage</span>

- Record-compressed
- This format compresses each record as it’s added to the file. 

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> File Based Storage</span>

- Block-compressed
- Format waits until data reaches block size to compress, rather than as each record is added. 
- Block compression provides better compression ratios compared to record-compressed SequenceFiles, 
- The preferred compression option for SequenceFiles. 
-  A block in block compression refers to a group of records that are compressed together within a single HDFS block.

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> Serialization</span>

- Serialization refers to the process of turning data structures into byte streams 
- Done for storage or transmission over a network. 
- Deserialization is the process of converting a byte stream back into data structures. 

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> Serialization</span>

- Serialization is core to a distributed processing system such as Hadoop, 
- It allows data to be converted into a format that can be efficiently stored as well as transferred across a network connection. 

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> Serialization</span>

- Serialization is commonly associated with two aspects of data processing in distributed systems:
- interprocess communication (remote procedure calls, or RPC) and data storage. 
- The main serialization format utilized by Hadoop is Writables. 
- Writables are compact and fast, but not easy to extend or use from languages other than Java. 


---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> Thirft</span>

- Thrift was developed at Facebook as a framework 
- Developed for implementing cross-language interfaces to services. 
- Uses an Interface Definition Language (IDL) to define interfaces, 
- Uses an IDL file to generate stub code to be used in implementing RPC clients 
- Allows us to implement a single interface that can be used with different languages to access different underlying systems. 

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436"> Thirft</span>

- Thrift has several drawbacks: 
- it does not support internal compression of records, 
- it’s not splittable, and it lacks native MapReduce support. 
- There are externally available libraries such as the Elephant Bird project to address these drawbacks,
- Hadoop does not provide native support for Thrift as a data storage format. 



---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">YARN</span>

- YARN for splitting up the functionalities of resource management and job scheduling/monitoring into separate daemons. 
- A global ResourceManager (RM) 
- per-application ApplicationMaster (AM). An application is either a single job or a DAG of jobs.
- The ResourceManager and the NodeManager form the data-computation framework. 

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Resource Manager</span>

- ResourceManager authority that arbitrates resources among all the applications in the system. 
- NodeManager is the per-machine framework agent 
- Responsible for containers, monitoring their resource usage (cpu, memory, disk, network) 
- reporting the same to the ResourceManager/Scheduler.

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Resource Manager</span>

- ResourceManager has two main components: 
  + Scheduler and 
  + ApplicationsManager.

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Resource Manager</span>

- Scheduler is pure scheduler 
- Scheduler is responsible for allocating resources
- Resources allocated to various running applications subject to constraints of capacities, queues etc. 

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Resource Manager</span>

- Performs no monitoring or tracking of status for the application. 
- Offers no guarantees about restarting failed tasks either due to application failure or hardware failures. 
- Performs its scheduling function based the resource requirements of the applications 

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Resource Manager</span>

- it does so based on the abstract notion of a resource Container 
- Resource container incorporates elements such as memory, cpu, disk, network etc.

---
<!-- .slide: data-autoslide="15000" -->

### <span style="color: #e49436">Resource Manager</span>

- Scheduler has a pluggable policy 
- Policy responsible for partitioning the cluster resources among the various queues, applications etc. 
- The current schedulers such as the CapacityScheduler and the FairScheduler would be some examples of plug-ins.

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Application Master</span>
- per-application ApplicationMaster is, a framework specific library  
- is tasked with negotiating resources from the ResourceManager 
- is working with the NodeManager(s) to execute and monitor the tasks.

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Application Master</span>

- is responsible for accepting job-submissions, 
- negotiates the first container for executing the application specific ApplicationMaster 
- Provides the service for restarting the ApplicationMaster container on failure. 

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Application Master</span>

- Has the responsibility of negotiating appropriate resource containers from the Scheduler, 
- Is responsible for tracking their status and monitoring for progress.


---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Capacity Scheduler</span>

- is designed to run Hadoop applications as a shared, multi-tenant cluster 
- is meant for maximizing the throughput and the utilization of the cluster.
- Each organization has it own private set of compute resources 

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Capacity Scheduler</span>

- Capacity designed to meet the organization’s SLA under peak or near peak conditions. 
- Sharing Hadoop clusters between organizations is cost-effective 
- Allows firms to reap benefits of economies of scale

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Capacity Scheduler</span>

- is designed to allow sharing a large cluster 
- Gives each organization capacity guarantees. 
- the available resources in the Hadoop cluster are shared among multiple organizations 

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Capacity Scheduler</span>

- Provides elasticity for the organizations in a cost-effective manner.
- Sharing clusters support for multi-tenancy 
- Primary abstraction provided by the CapacityScheduler is the concept of queues. 
- Queues are typically setup by administrators to reflect the economics of the shared cluster.

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Capacity Scheduler</span>

- Hierarchical Queues  
- Hierarchy of queues is supported to ensure resources are shared among the sub-queues of an organization before other queues are allowed to use free resources, there-by providing more control and predictability.

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Capacity Scheduler</span>

- Capacity Guarantees  
- Queues are allocated a fraction of the capacity of the grid
- A certain capacity of resources will be at their disposal. 
- All applications submitted to a queue will have access to the capacity allocated to the queue. 
- Adminstrators can configure soft limits and optional hard limits on the capacity allocated to each queue.

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Capacity Scheduler</span>

- Security - 
- Each queue has strict ACLs which controls which users can submit applications to individual queues. 
- safe-guards to ensure that users cannot view and/or modify applications from other users. 
- Per-queue and system administrator roles are supported.

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Capacity Scheduler</span>

- Elasticity 
- Free resources can be allocated to any queue beyond it’s capacity. 
- When there is demand for these resources, as tasks scheduled on these resources complete, they will be assigned to applications on queues running below the capacity (pre-emption is not supported). 
- This ensures that resources are available in a predictable and elastic manner to queues, thus preventing artifical silos of resources in the cluster which helps utilization.

---
<!-- .slide: data-autoslide="15000" -->
### <span style="color: #e49436">Capacity Scheduler</span>

- Multi-tenancy - 
- Comprehensive set of limits are provided to prevent a single application, user and queue from monopolizing resources of the queue or the cluster as a whole to ensure that the cluster isn’t overwhelmed..

---






![Thanks](images/thanks.png)



