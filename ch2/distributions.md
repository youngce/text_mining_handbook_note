# Distributions
| notations | defines |
| -- | -- |
| *D* | a collection of documents |
| *K* | a set of concepts |
| *D/K* | the subset of documents in *D* labeled with all of the concepts in *K* |
| *k* | a single concept |
| *D/k* | it is clear from the context, given a single concept k |
| $$f(D,K1|K2)$$ | the proportion of all those documents in *D* labeled with *K2* that are also labeled with *K1* , that is, $$f ( D, K1 | K2 ) =
f (D/K2, K1)$$|
|  $$P_K(x)$$| distributions – it will assign to any concept *x* in *K* a value between 0 and 1 – where the values are not required to add up to 1. |
| $$F_K(D, x)$$ | the proportion of documents in *D* labeled with *x* for any *x* in *K*. When *D* is clear from context, we will write this as $$F_K( x)$$. |
| 0:9 | 1:9 |
| 0:10 | 1:10 |


Whether as an initial step, to create a baseline, or to create more meaningful subdivisions of a single document collection for comparison purposes, text mining systems generally need to refer to some subcollection of a complete document collection. This activity is commonly referred to as *concept selection*. 




### Concept Selection


If *D* is a collection of documents and *K* is a set of concepts, *D/K* is the subset of documents in *D* labeled with all of the concepts in *K* . When it is clear from the context, given a single concept *k*, rather than writing *D/{k}* we use the notation *D/k*.

For example, the collection W contains a subset of the World Affairs collection – namely those documents that are labeled with the concepts iran, nicaragua, and reagan; W/bush contains the subset of documents that are labeled (at least) with reagan; and W/G8 contains those documents that are labeled with any terminal node under G8 (i.e., labeled with any G8 country). G8 is treated as a concept here when is being performed concept selection (rather than being viewed as the set of concepts under it, in which case it would have required all of its descendants to be present).

當執行Concept Selection時，G8被視為一個概念（而不是被視為concept selection下的一個概念集）

###Concept Proportion

If D is a collection of documents and K is a set
ofconcepts, $$f(D,K)$$ is the fraction of documents in D labeled with all of the concepts
in K, that is,  $$f(D,K)=\frac{|D/k|}{|D|}$$. Given one concept k, rather than writing $$f (D, {k})$$, we $$|D|$$
 use the notation $$f ( D, k)$$. When $$D$$ is clear from context, we drop it and write $$f ( k)$$.
 
Thus, for example, $$f (W, \big\{ iran, nicaragua, reagan \big\})$$ is the fraction of documents in the World Affairs collection labeled with iran, nicaragua, and reagan; $$f (reagan)$$ is the proportion of the collection labeled with the concept reagan; and $$f (G8)$$ is the proportion labeled with any (G8) country.


### Conditional Concept Proportion－$$f(D,K1 | K2)$$
If *D* is a collection of documents and *K1* and *K2* are sets of concepts, $$f(D,K1 | K2)$$ is the proportion of all those documents in *D* labeled with *K2* that are also labeled with *K1* , that is, $$f ( D, K1 | K2 ) =
f (D/K2, K1)$$. When *D* is clear from context, we will write this as $$f (K1 | K2)$$.
Applying this definition, we find that $$f (reagan | iran)$$ would represent the proportion of all documents labeled by the concept iran that are also labeled by the concept *reagan*.


### Concept Proportion Distribution－$$F_K(D, x)$$
Note the distinction between PK(x) and FK(x). PK(x) refers generically to any func- tion that is a concept distribution. FK(x) is a specific concept distribution defined by a particular concept-labeled set of documents.

