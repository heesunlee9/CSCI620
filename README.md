# CSCI620

#[What Does 'Big Data' Mean?](https://cacm.acm.org/blogs/blog-cacm/155468-what-does-big-data-mean/fulltext)

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



#[What Does 'Big Data' Mean? (Part 2)](https://cacm.acm.org/blogs/blog-cacm/156102-what-does-big-data-mean-part-2/fulltext)

Big volume – big analytics

metrics
Covariance Calculation
correlation coefficient
the difference in variance of the two time series

Most complex analytics (linear regression, data clustering, feature detection, machine learning, etc.) have the same characteristic; they are matrix calculations and are expressed as collections of linear algebra operations.

1. 기술
2. 경제
3. 트렌드
4. 예술
5. 생존력

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
