# Data-Mining-and-Information-Retrieval-system-Medication-Documents-l-

This project presents an Information Retrieval system developed to identify and retrieve the most relevant document based on a user's query. The system processes user-provided input, such as symptoms, medication details, or any related information, and efficiently retrieves the most appropriate document to meet the user's needs. This system is designed by AI students in their second year, ensuring practical learning and problem-solving.

### Considerations:
1. **Document Collection**: All text documents are gathered into a single variable by using a `for` loop. You can upload text files in the specified cell (IMPORTING & LOAD).
2. **Error Handling**: Various errors, particularly with data frames and lists, are handled and fixed to ensure that the code functions correctly across different situations.
3. **Simplified Output**: Ranking, different representations, and plotting are omitted for simplicity, focusing purely on the retrieval process.
4. **Commentary**: The code includes clear and concise comments for commonly misunderstood parts, ensuring that users can easily follow along.
5. **Result Dependence**: The results are based on similarity metrics to determine the most relevant documents.
  
### Key Features:
- **Text Preprocessing**:
  - **Tokenization**: Breaking the text into individual words or tokens.
  - **Lowercasing**: Converting all text to lowercase for uniformity.
  - **Stopwords Removal**: Eliminating common, less meaningful words (e.g., “and”, “the”).
  - **Stemming**: Reducing words to their root form (e.g., “running” to “run”).
  - **Lemmatization**: Converting words to their base form (e.g., “better” to “good”).
  
- **Text Representation**:
  - **TF-IDF Calculation**: Term Frequency-Inverse Document Frequency is used to evaluate the relevance of terms within documents.

- **Similarity Metrics**:
  1. **Jaccard Similarity**: Measures the similarity between documents based on shared tokens (randomly selected documents).
  2. **Cosine Similarity**: Computes the cosine of the angle between document vectors, with results presented in a DataFrame (without using external libraries).
  3. **Dice Similarity**: Measures the similarity between two sets, presented in a DataFrame (without using external libraries).

- **Ranking**:
  - Ranking the top 5 documents based on individual similarity scores.
  - Ranking the top 5 documents across all similarity measures.
  - Results are also presented in plots (though plotting is optional).

- **Evaluation**:
  - **Recall** and **Precision** are calculated manually to evaluate the retrieval performance.

This approach ensures a comprehensive understanding of information retrieval, from text preprocessing to evaluation, with hands-on learning by AI students.

- **Datasets**:
The dataset in the **data_DMproject** folder contains 32 text documents, with 5 irrelevant ones. The remaining 27 documents discuss medications broadly, but they do not focus on specific diseases or infections. This project, however, aims to prioritize documents related to **popular diseases and infections**, to make the system more targeted and relevant to users seeking information on these common health issues.

