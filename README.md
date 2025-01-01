# **Face Recognition Using Information Retrieval Techniques**

This project explores face recognition by combining these methods:
- **VGG16** for deep feature extraction,
- **XGBoost** for classification, and
- **FAISS** for fast similarity-based retrieval.

By leveraging the **Labeled Faces in the Wild (LFW)** dataset, the project demonstrates how information retrieval techniques can be applied to enhance face recognition systems.

---

## **Features**
- **Deep Feature Extraction**: Utilizes **VGG16** to generate embeddings (feature vectors) from face images.
- **Supervised Learning**: Implements **XGBoost** for accurate face classification.
- **Similarity Search**: Employs **FAISS** to enable efficient retrieval of similar faces.

---

## **Project Workflow**
1. **Data Preparation**:
   - Load and preprocess the LFW dataset.
   - Resize images to 224x224 pixels (compatible with VGG16).
   - Normalize pixel values and ensure all images are in RGB format.

2. **Feature Extraction**:
   - Use a pretrained **VGG16** model to extract embeddings for each face image.

3. **Classification**:
   - Train an **XGBoost** classifier using the extracted embeddings.
   - Evaluate the classifier on the test dataset.

4. **Similarity-Based Retrieval**:
   - Build a **FAISS index** using embeddings from the training set.
   - Query the FAISS index with embeddings from the test set to retrieve the most similar faces.

---
