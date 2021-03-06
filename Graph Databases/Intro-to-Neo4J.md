https://www.youtube.com/watch?v=U8ZGVx1NmQg

Often, graph data models is a much more natural way of representing data

Relational Database provided ACID transition capabilities
ACID: Atomicity, Consistency, Isolation, Durability
These are properties intended to guarantee validity even in the event of errors, power failures etc.
Atomicity: Guarantee that each transaction is treated as a single unit which either succeeds or completely fails. The database remains unchanged if the transaction failed
Consistency: All data written must be valid by all rules, constraints
Isolation: Concurrent Transactions leave DB in same state that would have been if they were executed in some "order"
Durability: Data once committed, will stay even in case of system failure

ACID guarantee lowers the performance, so we add index
But these do not help in capturing relationship between data

Neo4J helps often in being the single source of truth. Neo4J supports ACID transaction.
Neo4J usecases
-> Real Time Recommendations: Creating multiple links off the same product, creating links off people with similar buying patterns
-> Master Data Management: Storing our people, storing heirarchy. Now we connect people with same job profile etc.
-> Fraud Detection
-> Graph Based Search
-> Network & IT-Operations
-> Identity & Access Management 

To normalize the database, we create primary and secondary keys.But this leads to lot of join operations which are expensive

This leads to a situation where we have to trade-off between computation time vs storage 

Neo4J offers three properties
(i) Intuitiveness: Much more intuitive as one can connect with real world scenarios much easily
(ii) Speed: Much faster to understand and run queries on the data
(iii) Agility: Much more agile. It's quite easy to add/remove the data

-> Property: properties corresponding to a particular node/relationship
-> Relationship: relationship between two nodes

How do you use Neo4J?
-> Create Model
-> Load Data
-> Query Data

Bolt protocol is much faster than HTTP protocol

We found Neo4J to be literary thousands of times faster than our prior MySQL solution, with queries that require 10 to 100 times less code
- Senior Developer at E-Bay
