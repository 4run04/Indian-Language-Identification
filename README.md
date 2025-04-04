# Indian Language Similarity Analysis

Indian Language Similarity Analysis is a Python-based NLP tool for computing semantic similarity between various Indian languages using transformer-based language models. It helps researchers, linguists, and developers understand how closely related these languages are in terms of meaning and expression.

---

## Project Objective

This project aims to analyze and quantify the semantic similarities among Indian languages by comparing vector representations of predefined sentences. It provides a practical approach to studying cross-lingual semantics using modern language models.

---

## Methodology

1. **Predefined Sentences**: A representative sentence is chosen for each Indian language.
2. **Embedding Generation**: Sentences are encoded into vectors using the `paraphrase-MiniLM-L6-v2` model from the SentenceTransformers library.
3. **Cosine Similarity**: Pairwise cosine similarity is computed between sentence vectors.
4. **Similarity Matrix**: The results are displayed as a matrix, where each cell shows the similarity between a pair of languages.

---

## Sample Output

```
           Hindi   Tamil   Telugu  Bengali  Kannada
Hindi       1.00    0.84     0.82     0.87     0.81
Tamil       0.84    1.00     0.89     0.85     0.93
Telugu      0.82    0.89     1.00     0.83     0.90
Bengali     0.87    0.85     0.83     1.00     0.82
Kannada     0.81    0.93     0.90     0.82     1.00
```

---

## Getting Started

### Requirements

- Python 3.7 or higher
- `pandas`
- `sentence-transformers`

Install dependencies using pip:

```bash
pip install pandas sentence-transformers
```

### Running the Script

Run the script with:

```bash
python Indian_language_analysis.py
```

The output will be printed as a similarity matrix in your terminal.

---

## Use Cases

- Analyzing relationships between Indian languages
- Supporting multilingual NLP model development
- Preprocessing or understanding cross-lingual datasets
- Building linguistically aware recommendation systems or bots

---

## Potential Enhancements

- Visualization of the similarity matrix as a heatmap
- Support for dynamic sentence input
- Integration with additional transformer models
- Expansion to more regional languages and dialects
