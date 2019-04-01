
# Word Similarity Datasets for Thai Language

## Summary

This repo contains translated and re-rated datasets for **word similarity for Thai language**.
The four datasets are listed in the table below. The *Dataset* files are csv files, and just contain
the word pairs, and the similarity score between the two words.
Furthermore, we provide the individual annotator ratings as well as statistcs (inter-annotator agreement,
correlation between TH and EN versions, etc.) in the *Dataset Details* files.   


|Name            | Dataset       | Dataset Details |
|----------------| ------------- | ------------- |
|TH-WordSim-353  | [th-wordsim-353.csv](th-wordsim-353.csv)  | [th-wordsim-353.details.xlsx](th-wordsim-353.details.xlsx)|
|TH-SimLex-999   | [th-simlex-999.csv](th-simlex-999.csv)    | [th-simlex-999-details.xlsx](th-simlex-999-details.xlsx)  |
|TH-SemEval-500  | [th-semeval-500.csv](th-semeval-500.csv)  | [th-semeval-500-details.xlsx](th-semeval-500-details.xlsx)|  
|TWS-65          | [tws65.csv](tws65.csv)                    | [tws65_full.csv](tws65_full.csv)                          |  



## The Datasets
* *TH-WordSim-353*: in based on [WordSim-353](http://www.cs.technion.ac.il/~gabr/resources/data/wordsim353/).
    The English WordSim-353 is the most popular word similarity dataset. It contains 353 word pairs, and measures the semantic relatedness and a scale from 0 to 10. 
    We translated the dataset to Thai, and rated the word pairs with 10 annotators. 

* *TH-SimLex-999*: in based on [SimLex-999](https://fh295.github.io/simlex.html).
    SimLex-999 is specifically designed to capture similarity between terms, as opposed to relatedness (like in WordSim-353).
    The dataset contains 666 noun, 222 verb and 111 adjective pairs. Characteristics of this dataset are that it only includes words from the vocabulary of WordNet, 
    and that it contains a large number of antonymy pairs. The similarity ratings were created with crowdsourcing via Amazon Mechanical Turk, 
    originally on a scale from 0 to 6, later linearly re-scaled to [0,10]. 

* *TH-SemEval-500*: in based on the dataset from [SemEval2017 (Task 2)](http://alt.qcri.org/semeval2017/task2/).
    SemEval-500 is a multilingual dataset for English, Farsi, German, Italian and Spanish for SemEval-2017, task 2.
    The dataset contains 500 word pairs. The goal is to provide a challenging dataset, which includes word pairs from 34 domains such as 
    chemistry and mineralogy, computing, culture and society.
    Furthermore, the dataset contains named entities (e.g., Microsoft), or multiword expressions (e.g., black hole) in any of the 34 domains.
    For rating they use a 5-point Likert scale with a step size of 0.25, and the instructions for the annotators contain both the notions of relatedness and similarity, 
    in which similarity is rated higher.


* *tws-65*: This dataset is found in [Osathanunkul et al.](https://link.springer.com/chapter/10.1007/978-3-642-22000-5_56). 
    This is work by Osathanunkul et al., we only loaded it into a .csv file and provide it here. 
    We provide 2 versions, one with only 3 columns (the Thai word pair and the rating), 
    and a version which includes the English terms and the stddev.

## Cite
TODO .. add arxiv
A submission (of the preprint) to *IEEE Access* is under review. 


##  References
    *WordSim-353:* L. Finkelstein, E. Gabrilovich, Y. Matias, E. Rivlin, Z. Solan, G. Wolfman, and E. Ruppin, “Placing search in context: The concept revisited,” ACM Transactions on information systems, vol. 20, no. 1, pp. 116–131, 2002.
    *SimLex-999:* F. Hill, R. Reichart, and A. Korhonen, “Simlex-999: Evaluating semantic models with (genuine) similarity estimation,” Computational Linguistics, vol. 41, no. 4, pp. 665–695, 2015.
    [pdf on arxiv](https://arxiv.org/abs/1408.3456v1)
    *SemEval-500:* J. Camacho-Collados, M. T. Pilehvar, N. Collier, and R. Navigli, “Semeval-2017 task 2: Multilingual and cross-lingual semantic word similarity,” in Proc. 11th Int. Workshop on Semantic Evaluation (SemEval2017). Association for Computational Linguistics, 2017, pp. 15–26.




