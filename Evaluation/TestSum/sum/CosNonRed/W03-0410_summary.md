Because we make the simplifying assumption of a single correct classification for each verb , we also removed any verb : that was deemed excessively polygamous that belonged to another class under consideration in our study ; or for which the class did not correspond to the main sense . 
A number of supervised learning approaches have extracted such information about verbs from corpora , including their argument roles ( Gildea and Jurafsky , 2002 ) , selectional preferences ( Resnik , 1996 ) , and lexical semantic classification ( i.e. , grouping verbs according to their argument structure properties ) ( Dorr and Jones , 1996 ; Lapata and Brew , 1999 ; Merlo and Stevenson , 2001 ; Joanis and Stevenson , 2003 ) . 
We have previously shown that a broad set of 220 noisy features performs well in supervised verb classification ( Joanis and Stevenson , 2003 ) . 
4.1 Clustering Parameters . 
All experiments reported here were run on this same final set of 20 verbs per class ( including a replication of our earlier supervised experiments ) . 
We started with a list of all the verbs in the given classes from Levin , removing any verb that did not occur at least 100 times in our corpus ( the BNC , described below ) . 
This confirms that appropriate feature selection , and not just a small number of features , is important for the task of verb class discovery . 
Here we briefly describe the features that comprise our feature space , and refer the interested reader to Joanis and Stevenson ( 2003 ) for details . 
The third column of Table 2 gives the baseline we calculated from random clusterings . 
Currently , our only such feature is an extension of the animate feature of Merlo and Stevenson ( 2001 ) . 
We then describe our clustering methodology , the measures we use to evaluate a clustering , and our experimental results . 
In contrast to Merlo and Stevenson ( 2001 ) , we confirmed that a set of general features can be successfully used , without the need for manually determining the relevant features for distinguishing particular classes ( cf . 
For example , the accuracy measure ( Stevenson and Joanis 2003 ; Korhonen , Krymolowski , and Marx 2003 ) evaluates whether a verb is assigned to a correct cluster with respect to the gold standard class of the majority of cluster members . 
In recent work , Stevenson and Joanis ( 2003 ) compared their supervised method for verb classification with supervised and unsupervised techniques . 
In these experiments , they enlarged the number of gold standard English verb classes to 14 classes related to Levin classes , with a total of 841 verbs . 
A plausible scenario is that researchers would have examples of verbs which they believe fall into different classes of interest , and they want to separate other verbs along the same lines . 
They found that a supervised approach where the classifier was trained with five seed verbs from each verb class outperformed both a manual selection of features and the unsupervised 186 approach of Dash , Liu , and Yao ( 1997 ) , which used an entropy measure to organize data into a multidimensional space . 
Dorri and Jones , 1996 ; Schulte im Walde and Brew , 2002 ) . 
We use , the mean of the silhouette measure from Matlab , which measures how distant a data point is from other clusters . 
7 5 0 Table 1 : Verb classes ( see Section 3.1 ) , their Levin class numbers , and the number of experimental verbs in each ( see Section 3.2 ) . 
We focus here on extending the applicability of unsupervised methods , as in ( Schulte im Walde and Brew , 2002 ; Stevenson and Merlo , 1999 ) , to the lexical semantic classification of verbs . 
Like others , we have assumed lexical semantic classes of verbs as defined in Levin ( 1993 ) ( hereafter Levin ) , which have served as a gold standard in computational linguistics research ( Dorr and Jones , 1996 ; Kipper et al. , 2000 ; Merlo and Stevenson , 2001 ; Schulte im Walde and Brew , 2002 ) . 
Our second measure , the adjusted Rand measure used by Schulte im Walde ( 2003 ) , instead gives a measure of how consistent the given clustering is overall with respect to the gold standard classification . 
However , a general feature space means that most features will be irrelevant to any given verb discrimination task . 
Unsupervised or semi-supervised approaches have been successful as well , but have tended to be more restrictive , in relying on human filtering of the results ( Riloff and Schmelzenbach , 1998 ) , on the hand- selection of features ( Stevenson and Merlo , 1999 ) , or on the use of an extensive grammar ( Schulte im Walde and Brew , 2002 ) . 
We then replaced 10 of the 260 verbs ( 4 % ) to enable us to have representative seed verbs for certain classes in our semi-supervised experiments ( e.g. , so that we could include wipe as a seed verb for the Wipe verbs , and fill for the Fill verbs ) . 
In an unsupervised ( clustering ) scenario of verb class discovery , can we maintain the benefit of only needing noisy features , without the generality of the feature space leading to âthe curse of dimensionality 
However , it gives important information about the quality of a clustering : The other measures being equal , a clustering with a higher value indicates tighter and more separated clusters , suggesting stronger inherent patterns in the data . 
4.2.2 Adjusted Rand Measure Accuracy can be relatively high for a clustering when a few clusters are very good , and others are not good . 
However , creating a Verb classification is highly resource intensive , in terms of both required time and linguistic expertise . 