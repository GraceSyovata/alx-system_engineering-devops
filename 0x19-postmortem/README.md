Issue Summary 
-	Duration: Thursday 29 th June, 2024 from 14. 00 Hours – 16. 30 Hours (GMT). 
-	Impact: Service disruptions and slow connection speeds were reported to have acts of inconvenience by the users. It was established that about forty percent of the users were impacted. 
-	Root Cause: A situation in which the selected database gets overloaded by the queries that were used in the process. 
Timeline 
-	2:00 PM: Issue reported by a monitoring alert that showed high database response time. 
-	2:10 PM: The first intervention was initiated; thought it was a network problem. 
-	2:7:30 PM: Knew that the problem was with the database; referred the case to the DBA. 
-	2:45 PM: DBA team – Several queries were pointed out as being uncompensated that led to the overload. 
-	3:00 PM: Temporary remedy of the problem done in this manner by restarting the database service. 
-	3:15 PM: drill down examination was made and queries actual contributors to the problem were identified. 
-	4:12:00 PM : Queries have been tuned for the best performance and new indexes created. 
-	4:30 PM: Total recovery of the service. 

Root Cause and Resolution 
-	Root Cause: The query involved in the database incurred several problems due to several unoptimized problems. These queries were consuming much CPU time and this harmed the overall response time and the services being delivered. Solving the main problem started with identifying the fact that there was a group of queries that were not properly indexed; as a result, the requests caused full table scans every time. 

-	Resolution: The problematic queries were discovered on the basis of logs and performance analyses of the prior period. Following modifications where made to the queries; indexes were added at the correct places to help the database, parts of the SQL where rewrote more efficiently, and lastly, the frequent results where cached to cut the load of the database. Also, a short-term solution of restarting the database service was incorporated to help on a short-term basis while the database had the desired improvements made. 

Corrective and Preventative Measures 
-	Improvements: That is why, to avoid similar problems, it is important to set up definite time intervals for the performance of databases’ reviewing. This encompasses daily examination of query performance, finding poor-performing queries, and guaranteeing that all new queries are written appropriately on the database.
-	Tasks: 
-	Implement Query Optimization Best Practices: It is necessary to review all the database queries to identify if there is a need to optimize it to become more efficient. 
-	Add Monitoring on Query Performance: Create robust monitoring systems that will helps in early identification of query performance problems. 
-	Schedule Regular Database Performance Reviews: Do a workshop once in a while to determine any foreseeable performance thorn in the flesh of the company. These reviews should, therefore, be incorporated into the development phase to try and identify such complications as early as possible. 
-	Train Development Team on Best Practices: Make certain that all developers are familiar with the recommendations for generating the most effective SQL code.
-	Implement Caching Strategies: Applying caching policies on heavy accessed data will result in minimizing the call on the database. 
-	Conduct Load Testing: Conduct a load test frequently to discover the present robustness of the current database setting to find out the areas of vulnerability. 
