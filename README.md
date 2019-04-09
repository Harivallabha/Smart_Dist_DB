# Smart_Dist_DB
Design and Implementation of a Smart Distributed Database for a Small Multi-Outlet Business.
(Project for the Database Management Systems course @ BITS Pilani - Hyderabad)

### Brief Outline
**Proposal**: We propose to design and implement a distributed database for a small multi-outlet business: a DVD and Movie rental-and-sales service. We plan to recreate Joseph Grech’s thesis with the following inclusions:  A front-end user interface, decentralized cloud deployment and a personalized recommender system. 

(As an ambitious goal, or extension of the project beyond the submission date (28.04.19) we intend to implement a parallel DBMS architecture for the same and carry out a performance comparison between the decentralized (distributed), parallel and the centralized cloud (distributed processing) solution.)

Point to note: Distributed (decentralized) database management is distinct from distributed processing. A distributed processing solution usually makes use of a centralized repository/parent database.

**Motivation**: DVD and Movie rental outlets often store transaction information (handwritten) physically in books. A database distributed across the outlets in various locations would expedite the daily business process, and make data available for business analytics. Moreover, a distributed database offers performance improvements for query processing and doesn’t have a single point of failure.

**Functionality**: As a case study, we take the example of a movie rental service with outlets in three locations. We implement a database solution for this business with a range of functionalities including features to store customer and movie records, track transactions, check availability, generate reports of sales and rentals, for stock taking and profit calculation, user-authentication and privileges.

In particular, we note that the distributed solution must maintain referential integrity, data consistency and fault tolerance across the outlets through fragmentation, allocation and replication while allowing for concurrency in transactions. 

A limitation of the project is that the data is populated artificially and serves as a proof of concept without actual real-world deployment.
We utilize this data in conjunction with the MovieLens Dataset for the purpose of generating predictive ratings for personalized recommendations, using machine learning with python.

**Technology**: We intend to use Oracle Streams, Standard One Edition for the distributed database solution, the python Flask microframework for the front-end, and Oracle Bare Metal Cloud Service for cloud deployment and performance comparison. Querying would be done with the help of SQL procedures.

**References** 
Joseph Grech. (2009). *Designing and Implementing a Distributed Database for a Small Multi-Outlet Business*. Master's thesis, Regis University.


### Contributors
* Harivallabha Rangarajan
* Mukundhan Jayaraman
* Nikhil Lokesh
