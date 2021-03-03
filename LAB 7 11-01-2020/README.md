# LAB 7

## Wednesday, 11<sup>th</sup> November, 2 - 5 PM

# Assignment 7

The third assignment is **Hand gesture Classification using SVM**.

### Dataset

[Linked](https://drive.google.com/file/d/1g83_ZbWuEiNBja9welgFCsVlRVChTBn0/view?usp=sharing) is the set of papers accepted in AAAI conference, 2019. For each paper, we have the title, abstract, a set of topics, a set of keywords and a single high-level topic.

### Description:

1. Prepare a vocabulary using all these fields (except the high-level keywords), after removing stopwords. **[1 mark]**

2. Implement agglomerative clustering of the papers based on their "keywords", using single-linkage criteria. Use Jaccard coefficient as the similarity measure. Try to choose thresholds such that the number of clusters comes to around 10. **[3 marks]**

3. Implement agglomerative clustering of the papers based on their "topics", using complete-linkage criteria. Use Jaccard coefficient as the similarity measure. Try to choose thresholds such that the number of clusters comes to around 10. **[3 marks]**

4. Represent the abstract of each paper as a vector of word counts. Carry out K-means clustering (using library functions) on these vectors. Use same number of clusters as found in (2) or (3). **[2 marks]**

5. Calculate the rand-index between pairs of clusterings obtained in (2), (3), (4). **[1 mark]**