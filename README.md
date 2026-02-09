## Experimental Scenarios

## Dataset
Two labeled datasets are used in the paper **Mohammad Omar (2020)**:
- **Collected Dataset**: 141 open-ended English questions from multiple academic sources  
- **Yahya et al. (2012) Dataset**: 600 open-ended English questions balanced across Bloom levels

## Tools
Python

## Library 
spaCy, scikit-learn, Gensim, NumPy, Pandas

Five classification scenarios are evaluated using different feature representations and SVM kernels:

1. **Scenario 1: TFPOS-IDF**  
   Feature: TFPOS-IDF  
   Kernel: Linear, RBF

2. **Scenario 2: ETFPOS-IDF**  
   Feature: ETFPOS-IDF  
   Kernel: Linear, RBF

3. **Scenario 3: Word2Vec**  
   Feature: Pretrained Word2Vec embeddings  
   Kernel: Linear, RBF

4. **Scenario 4: TFPOS-IDF + Word2Vec**  
   Feature: Combination of syntactic weighting and semantic embeddings  
   Kernel: Linear, RBF

5. **Scenario 5: ETFPOS-IDF + Word2Vec**  
   Feature: Bloom-aware syntactic weighting integrated with Word2Vec  
   Kernel: Linear, RBF
