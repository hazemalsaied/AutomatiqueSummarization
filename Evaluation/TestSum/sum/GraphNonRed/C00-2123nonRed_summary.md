The details are given in ( Och and Ney , 2000 ) . 
We use a solution to this problem similar to the one presented in ( Och et al. , 1999 ) , where target words are joined during training . 
The model is often further restricted so that each source word is assigned to exactly one target word ( Brown et al. , 1993 ; Ney et al. , 2000 ) . 
The goal of machine translation is the translation of a text given in some source language into a target language . 
The translation scores for the hypotheses generated with different threshold values t0 are compared to the translation scores obtained with a conservatively large threshold t0 = 10:0 . For each test series , we count the number of sentences whose score is worse than the corresponding score of the test series with the conservatively large threshold t0 = 10:0 , and this number is reported as the number of search errors . 
We are given a source string fJ 1 = f1 : : : fj : : : fJ of length J , which is to be translated into a target string eI 1 = e1 : : : ei : : : eI of length I . Among all possible target strings , we will choose the string with the highest probability : ^eI 1 = arg max eI 1 fPr ( eI 1jfJ 1 ) g = arg max eI 1 fPr ( eI 1 ) Pr ( fJ 1 jeI 1 ) g : ( 1 ) The argyle operation denotes the search problem , i.e . the generation of the output sentence in the target language . 
In Section 3 , we introduce our novel concept to word reordering and a DP-based search , which is especially suitable for the translation direction from German to English . 
The alignment model uses two kinds of parameters : alignment probabilities p ( aj jajô1 I ; J ) , where the probability of alignment aj for position j depends on the previous alignment position ajô1 Ney et al. , 2000 ) and lexicon probabilities p ( fj jean . 
What is important and is not expressed by the notation is the so-called coverage constraint : each source position j should be hit exactly once by the path of the inverted alignment bI 1 = b1 : : : bi : : : bI . Using the inverted alignments in the maximum approximation , we obtain as search criterion : max I ( p ( JjI ) max eI 1 ( I Yi=1 p ( eijeiô1 ) max bI 1 I Yi=1 [ p ( bijbiô1 I ; J ) p ( fbi jei ) ] ) ) = = max I ( p ( JjI ) max eI 1 ; bI 1 ( I Yi=1 p ( eijeiô1 ) p ( bijbiô1 I ; J ) p ( fbi jei ) ] ) ) ; where the two products over i have been merged into a single product over i. p ( eijeiô1 ) is the trigram language model probability . 
Table 4 shows translation results for the three approaches . 
Word Re-ordering and DP-based Search in Statistical Machine Translation
The algorithm works due to the fact that not all permutations of cities have to be considered explicitly . 
The alignment mapping is j ! i = aj from source position j to target position i = aj . The use of this alignment model raises major problems if a source word has to be aligned to several target words , e.g . when translating German compound nouns . 
This measure has the advantage of being completely automatic . 
A procedural definition to restrict1In the approach described in ( Berger et al. , 1996 ) , a mor pathological analysis is carried out and word morphemes rather than full-form words are used during the search . 
The quasi-monotone search performs best in terms of both error rates mWER and SSER . 
Pr ( eI 1 ) is the language model of the target language , whereas Pr ( fJ 1 jeI1 ) is the translation model . 
To explicitly handle the word reordering between words in source and target language , we use the concept of the so-called inverted alignments as given in ( Ney et al. , 2000 ) . 
An extended lexicon model is defined , and its likelihood is compared to a baseline lexicon model , which takes only single-word dependencies into account . 
The resulting algorithm is depicted in Table 1 . 
E.g . when 'Zahnarzttermin ' is aligned to dentist 's , the extended lexicon model might learn that 'Zahnarzttermin ' actually has to be aligned to both dentist 's and ap ointment . 
Here , we process only full-form words within the translation procedure . 
We apply a beam search concept as in speech recognition . 
man 5 . 
These alignment model are similar to the concept of hidden Markov model ( HMM ) in speech recognition . 