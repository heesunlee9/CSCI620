# CSCI620

# [What Does 'Big Data' Mean?](https://cacm.acm.org/blogs/blog-cacm/155468-what-does-big-data-mean/fulltext)

Big Volume, Small Analytics

First solution
multi-petabyte data warehouses

request
1. resource elasticity 
2. sharing a common resource

second solution
Hive/Hadoop
inefficiency of Hadoop, compared to parallel DBMSs.
schema migration without incurring downtime

SQL vendors will all move to column stores

storage ideas, including compression and encryption. Sampling to cut down query costs is also of interest.



# [What Does 'Big Data' Mean? (Part 2)](https://cacm.acm.org/blogs/blog-cacm/156102-what-does-big-data-mean-part-2/fulltext)

Big volume – big analytics

metrics
Covariance Calculation
correlation coefficient
the difference in variance of the two time series

Most complex analytics (linear regression, data clustering, feature detection, machine learning, etc.) have the same characteristic; they are matrix calculations and are expressed as collections of linear algebra operations.

Analytics on big data : data management operations + linear algebra

possible approaches to big analytics on big data:

Option 1: Use a statistics package such as R, S, SAS, SPSS, etc.
linear algebra
may not scale

Option 2: Use an RDBMS. (SQL)
data management

the simulation is not easy to figure out.
(convergence) 

Shortcoming: performance! (There is something I don't know)

Option 3: Use both option 1 and 2 together.

Option 4: Use extended RDBMS features.

Option 5: Use an array DBMS, such as Rasdaman or SciDB

First, I think complex analytics will increase

Second, enterprises will have to upgrade the skill set of their business analysts. Instead of merely running current business intelligence tools, they will need to become facile in statistical operations. 

Lastly, notice that I have not included Hadoop as an option. Since complex analytics are not "embarrassingly parallel," Hadoop will suffer significant performance problems. Hence, I do not consider this a reasonable Hadoop use case. (?)

# [What Does 'Big Data' Mean? (Part 3)](https://cacm.acm.org/blogs/blog-cacm/157589-what-does-big-data-mean-part-3/fulltext)

"Big velocity" means "drinking from a firehose," i.e. coping with data arriving at very high speed. (댓글 : 이게 왜 빅데이터인지 모르겠다)



we can divide the high velocity space into two components. The first one requires <strong>real-time attention</strong> to the feed, while the second one allows one to collect large groups of messages for batch processing.

I assume we must have sub-second response time to high volumes of real-time messages.

two cases of interest
- to find patterns that should trigger electronic trades: "big pattern – little state"
- at various locations: "little pattern – big state."

Legacy RDBMSs, such as DB2, Oracle, and SQLServer

Forty years of DBMS research has clearly demonstrated the advantages of high-level data languages (better data independence, better code maintainability, easier to understand code, no loss of performance).

I believe that the NoSQL vendors are misguided in their belief that low level notations yield better performance. => not true

The second point of the NoSQL vendors is that giving up ACID transactions yields better performance.
=> not true






