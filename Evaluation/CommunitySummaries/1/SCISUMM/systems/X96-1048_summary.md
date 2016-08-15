The introduction of two new tasks into the MUC evaluations and the restructuring of information extraction into two separate tasks have infused new life into the evaluations . 
Nearly half the sites chose to participate in all four tasks , and all but one site participated in at least one SGML task and one extraction task . 
Many of the sites have emphasized their pattern-matching techniques in discussing the strengths of their MUC6 systems . 
Nonetheless , as one rough measure of progress in the area of information extraction as a whole , we can consider the F-measures of the top-scoring systems from the MUC5 and MUC6 evaluations . 
Commercial systems are available already that include identification of those defined for this MUC6 task , and since a number of systems performed very well for MUC6 , it is evident that high performance is probably within reach of any development site that devotes enough effort to the task . 
NE Results Overall Fifteen sites participated in the NE evaluation , including two that submitted two system configurations for testing and one that submitted four , for a total of 20 systems . 
OVERVIEW OF RESULTS OF THE MUC-6 EVALUATION
The evolution and design of the MUC6 evaluation are discussed in the paper by Grishman and Sundheim in this volume . 
An algorithm developed by the MITRE Corporation for MUC6 was implemented by SAIC and used for scoring the task . 
The other two tasks , Template Element and Scenario Template , were information extraction tasks that followed on from the MUC evaluations conducted in previous years . 
Overall recall and precision on the CO task 2 2 Key to recall and precision scores : UDurham 36R/44P , UManitoba 63R/63P , UMass 44R/51P , NYU 53R/62P , UPenn 55R/63P , USheffield 51R/71P , SRI 59R/72P.. 
As indicated in table 2 , all systems performed better on identifying person names than on identifying organization or location names , and all but a few systems performed better on location names than on organization names . 
Note also that even the best system on the third event was unable to determine that the succession event was occurring at McCannEfickson ; in addition , it only partially captured the full title of the post . 
The two SGML-based tasks required innovations to tie system-internal data structures to the original text so that the annotations could be inserted by the system without altering the original text in any other way . 
This capability has other useful applications as well , e.g. , it enables text highlighting in a browser . 
In the middle of the effort of preparing the test data for the formal evaluation , an annotator variability test was conducted . 
As defined for MUC6 , the ST task presents a significant challenge in terms of system portability , in that the test procedure required that all domain-specific development be done in a period of one month . 
As shown in table 1 , performance on the NE task overall was over 90 % on the F-measure for half of the systems tested , which includes systems from seven different sites . 
oSix systems : New York Times ( publication name in phrase , `` a framed page from the New York Times '' ; without sufficient context , the name can be ambiguous in its reference to a physical object versus an organization ) eThree systems : Coca-Cola Classic ( product name deriving from `` Coca-Cola , '' which appears separately in several places in the article and is occasionally ambiguous even in context between product name and organization name ) eOne system : Not Butter ( part of product name , `` I Ca n't Believe It 's Not Butter '' ) eOne system : Taster ( part of product name , `` Taster 's Choice '' )  One system : Choice ( part of product name , `` Taster 's Choice '' ) eFive systems : a hot agency ( nonspecific use of indefinite in phrase `` ... is interested in acquiring a hot agency '' ) Given the variety of contextual clues that must be taken into account in order to analyze the above entities correctly , it is understandable that just about any given system would commit at least one of them . 
The latest in a series of natural language processing system EVALUATION was concluded in October 1995 and was the topic of the Sixth Message Understanding Conference ( MUC6 ) in November . 