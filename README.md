# distributed-database-management-system
A distributed database is basically a database that is not limited to one system, it is spread over different sites.
 i.e, on multiple computers or over a network of computers. A distributed database system is located on various sites that don’t share physical components. This may be required when a particular database needs to be accessed by various users globally. It needs to be managed such that for the users it looks like one single database. 

 ## type of distributed database
 * ### Homogeneous Database
 in homogeneous like the name imply all different site store database identically The operating system, database management system, and the data structures used are all the same at all site and they are easy to maintain 

 * ### Heterogeneous Database: 
In a heterogeneous distributed database, different sites can use different schema and software that can lead to problems in query processing and transactions. Also, a particular site might be completely unaware of the other sites. Different computers may use a different operating system, different database application. They may even use different data models for the database. Hence, translations are required for different sites to communicate. 

## Distributed Data Storage :
There are 2 ways in which data can be stored on different sites. These are: 

1. ### Replication –
In this approach, the entire relationship is stored redundantly at 2 or more sites. If the entire database is available at all sites, it is a fully redundant database. Hence, in replication, systems maintain copies of data. 

This is advantageous as it increases the availability of data at different sites. Also, now query requests can be processed in parallel. 
However, it has certain disadvantages as well. Data needs to be constantly updated. Any change made at one site needs to be recorded at every site that relation is stored or else it may lead to inconsistency. This is a lot of overhead. Also, concurrency control becomes way more complex as concurrent access now needs to be checked over a number of sites. 

2. ### Fragmentation –
In this approach, the relations are fragmented (i.e., they’re divided into smaller parts) and each of the fragments is stored in different sites where they’re required. It must be made sure that the fragments are such that they can be used to reconstruct the original relation (i.e, there isn’t any loss of data). 
Fragmentation is advantageous as it doesn’t create copies of data, consistency is not a problem. 
 

Fragmentation of relations can be done in two ways: 
 

* Horizontal fragmentation – Splitting by rows – 
The relation is fragmented into groups of tuples so that each tuple is assigned to at least one fragment.
* Vertical fragmentation – Splitting by columns – 
The schema of the relation is divided into smaller schemas. Each fragment must contain a common candidate key so as to ensure a lossless join.
In certain cases, an approach that is hybrid of fragmentation and replication is used.


### Distributed database system can be applied in:
* hotel chain
* search engine
* multi media application



 A distributed database system is a type of database management system that stores data across multiple computers or sites that are connected by a network. In a distributed database system, each site has its own database, and the databases are connected to each other to form a single, integrated system.

  The main advantage of a distributed database system is that it can provide higher availability and reliability than a centralized database system. Because the data is stored across multiple sites, the system can continue to function even if one or more sites fail. In addition, a distributed database system can provide better performance by distributing the data and processing load across multiple sites.

There are several different architectures for distributed database systems, including:
* Client-server architecture: In this architecture, clients connect to a central server, which manages the distributed database system. The server is responsible for coordinating transactions, managing data storage, and providing access control.

* Peer-to-peer architecture: In this architecture, each site in the distributed database system is connected to all other sites. Each site is responsible for managing its own data and coordinating transactions with other sites.

* Federated architecture: In this architecture, each site in the distributed database system maintains its own independent database, but the databases are integrated through a middleware layer that provides a common interface for accessing and querying the data.

  Distributed database systems can be used in a variety of applications, including e-commerce, financial services, and telecommunications. However, designing and managing a distributed database system can be complex and requires careful consideration of factors such as data distribution, replication, and consistency.