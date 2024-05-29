### Machine Translation System: English to French

This project implements a basic machine translation system from English to French using word embeddings. Key steps include:

1. **Data Preparation**: Load English and French embeddings and a bilingual dictionary.
2. **Transformation Matrix**: Compute a transformation matrix \( R \) that maps English embeddings to French embeddings by minimizing the Frobenius norm loss.
3. **Gradient Descent**: Optimize \( R \) using gradient descent to minimize translation errors.
4. **k-Nearest Neighbors (k-NN)**: Use k-NN to find the closest French word embedding to the transformed English embedding.
5. **Translation Accuracy**: Evaluate translation accuracy by checking if the nearest French embedding corresponds to the correct French word.

### Key Functions

- `get_matrices()`: Extracts matrices \( X \) (English) and \( Y \) (French) from the dictionary and embeddings.
- `compute_gradient()`: Calculates the gradient of the loss function with respect to \( R \).
- `align_embeddings()`: Optimizes \( R \) using gradient descent.
- `test_vocabulary()`: Tests the accuracy of the translation by comparing the nearest French embeddings to the actual translations.
