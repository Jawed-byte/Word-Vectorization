# Word Vectorization

This project compares two popular word vectorization techniques: Singular Value Decomposition (SVD) and Word2Vec (Skip-gram), analyzing their performance across different metrics and window sizes for text classification tasks.

## Overview

The study evaluates the effectiveness of SVD and Word2Vec (Skip-gram) through:
- Different window size configurations
- Multiple performance metrics
- Detailed analysis of results
- Investigation of strengths and limitations

## Techniques Implemented

### 1. Singular Value Decomposition (SVD)
- Window sizes: 1, 2, and 3
- Linear algebra-based approach
- Co-occurrence matrix decomposition

### 2. Word2Vec (Skip-gram)
- Window sizes: 1, 2, and 5
- Neural network-based approach
- Contextual word embeddings

## Results

### SVD Performance

| Window Size | Accuracy | Precision | Recall | F1 Score |
|-------------|----------|-----------|---------|-----------|
| 1 | 0.7454 | 0.7504 | 0.7454 | 0.7441 |
| 2 | 0.7736 | 0.7848 | 0.7736 | 0.7748 |
| 3 | 0.7812 | 0.7847 | 0.7812 | 0.7817 |

### Skip-gram Performance

| Window Size | Accuracy | Precision | Recall | F1 Score |
|-------------|----------|-----------|---------|-----------|
| 1 | 0.8639 | 0.8641 | 0.8639 | 0.8639 |
| 2 | 0.8589 | 0.8584 | 0.8589 | 0.8584 |
| 5 | 0.8637 | 0.8643 | 0.8637 | 0.8637 |

## Key Findings

### Word2Vec Advantages
1. **Superior Performance**
   - Consistently higher accuracy across all window sizes
   - Better precision and recall scores
   - More stable F1 scores

2. **Semantic Richness**
   - Better capture of contextual relationships
   - Enhanced semantic understanding
   - More nuanced word representations

3. **Non-linear Capabilities**
   - Ability to model complex relationships
   - Better handling of linguistic patterns
   - More expressive embeddings

### Technique Limitations

#### SVD Shortcomings
- Limited semantic understanding
- Difficulty with contextual relationships
- Linear transformation constraints

#### Word2Vec Shortcomings
- Dependency on pre-trained models
- Challenges with out-of-vocabulary words
- Computational resource requirements

## Best Configurations

### SVD
- Best window size: 3
- Test Accuracy: 0.7812
- Optimal for capturing broader context

### Skip-gram
- Best window sizes: 1 and 5 (similar performance)
- Test Accuracy: ~0.8639
- More robust across different window sizes




