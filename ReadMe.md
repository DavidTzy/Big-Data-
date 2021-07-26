Some big data practices like language model, graph analysis,relational data base analysis and machine learning(classfication). Everything is in PySpark.

General Topic including(with some brief intro):

(1)PMI analysis(pointwise mutual information) on Shakespeare's masterpieces: If two events x and y are independent, their PMI will be zero. A positive PMI indicates that x and y are more likely to co-occur than they would be if they were independent.   
Similarly, a negative PMI indicates that x and y are less likely to co-occur.   The PMI of events x and y is given by

PMI(x,y) = log（p(x,y)/p(x)p(y)）

where p(x) and p(y) are the probabilities of occurrence of events x and y, and p(x,y) is the probability of co-occurrence of x and y.


(2)Personalized Pagerank on  Gnutella server network: PageRank is one of the most important methods Google uses to determine a page’s relevance or importance,details and algorithms can be found in section 5.3 in Lin's book(Data-Intensive Text Processing
with MapReduce)

Personalized page rank is like ordinary page rank except:
- One node in the graph is designated as the source node.   Personalized page rank is performed with respect to that source node.
- Personalized page rank is initialized by assigning all probability mass to the source node, and none to the other nodes.   In contrast, ordinary page rank is initialized by giving all nodes the same probability mass.
- Whenever personalized page rank makes a random jump, it jumps back to the source node.   In contrast, ordinary page rank may jump to any node.
- In personalized page rank, all probability mass lost dangling nodes is put back into the source nodes.  In ordinary page rank, lost mass is distributed evenly over all nodes.

(3)Relational data base analysis: 
 The work is done with tabular data based on the schema for the TPC-H benchmark, which is a standard test used to measure the performance of relational database systems. 
 In short, this project is SQL in pyspark :)))).
 
(4)Spamness Classification:
The goal of the project is to detect spam document with the use of a very powerful and simple classifier. The details of the classifier can be referred to the paper in the file, but 
it is really simple and powerful. Here i didn't use any common classifiers(if you are going to use things like SVM, logistic regression, Random forest in Spark, I suggest u try MLlib, they have everything you need!). The details of parallization computation is inside the document.





