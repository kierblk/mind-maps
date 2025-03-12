---
title: markmap
markmap:
  color: ["#FF80BF", "#FF9580", "#FFCA80", "#FFFF80", "#14710A", "#6ECC66", "#047FB4", "#644AC9"]
  colorFreezeLevel: 2
  maxWidth: 300
---

# Vectors

- **Definition**
  - Mathematical objects representing quantities with magnitude (length) & direction (orientation)
  - Represented in CS as ordered collections (arrays, lists, tuples) encoding data points, directions, or attributes

- **Notation & Vocabulary**
  - **Vector Notation**
    - Bold lowercase (**v**)
    - Arrow notation ($\vec{v}$)
  - **Magnitude**
    - Length: $\|\vec{v}\|$
  - **Dimension**
    - Number of components (elements in vector)

- **Representation in Code**
  - Arrays, Lists: `[x, y, z]`
  - Tuples: `(x, y, z)`
  - Custom structures/classes for vectors

- **Types of Vectors in CS & ML**
  - **Position vectors** (points/locations)
  - **Direction vectors**
    - Directions, offsets
  - **Feature vectors**
    - Represent attributes/features for ML models
  - **Zero vector** ($\vec{0}$)
    - Origin or no-change representation

- **Vector Operations**

  - **Addition**
    - Element-wise sum: $$\vec{u} + \vec{v} = (u_x+v_x,\, u_y+v_y,\, u_z+v_z)$$
    - Used for combining directions or movements

  - **Subtraction**
    - Element-wise difference: $$\vec{u} - \vec{v} = (u_x-v_x,\, u_y-v_y,\, u_z-v_z)$$
    - Relative direction, displacement calculations

  - **Scalar Multiplication (Scaling)**
    - Changes magnitude, preserves/reverses direction:
      $$
      c\vec{v} = (c v_x,\, c v_y,\, c v_z)
      $$
    - Applications: graphics scaling, ML weighting

  - **Dot Product (Scalar Product)**
    - Produces scalar indicating vector similarity:
      $$
      \vec{u}\cdot\vec{v} = u_x v_x + u_y v_y + u_z v_z
      $$
    - Measures alignment (cosine similarity):
      $$
      \vec{u}\cdot\vec{v} = \|\vec{u}\|\|\vec{v}\|\cos(\theta)
      $$
    - Applications: ML similarity scoring, graphics lighting/shading

  - **Cross Product (Vector Product)**
    - Vector perpendicular to two vectors:
      $$
      \vec{u}\times\vec{v}=
      \begin{vmatrix}
      \hat{i} & \hat{j} & \hat{k}\\
      u_x & u_y & u_z\\
      v_x & v_y & v_z
      \end{vmatrix}
      $$
    - Applications: 3D graphics normals, rotation calculations, physics

- **Magnitude & Normalization**
  - **Magnitude (Length):**
    - $$\|\vec{v}\| = \sqrt{x^2 + y^2 + z^2}$$
  - **Normalization (Unit Vector):**
    - $$\hat{v} = \frac{\vec{v}}{\|\vec{v}\|}$$
  - Applications: ML direction features, graphics directions

- **Machine Learning & AI Applications**

  - **Vectorization Techniques**
    - Converting data into numeric vectors
      - Text (TF-IDF, Word2Vec, FastText)
      - Numerical (One-hot encoding, normalization/scaling)

  - **Embeddings & Feature Representation**
    - Dense embeddings (BERT, GPT, Sentence Transformers)
    - Word embeddings: semantic meaning capture
    - Feature vectors: numeric attribute representations

  - **LLMs & Vector-based Retrieval**
    - Semantic similarity search (cosine similarity)
    - Vector databases (Pinecone, FAISS, Chroma, Weaviate)
    - Retrieval-Augmented Generation (RAG)
    - Applications: chatbots, semantic search, question-answering

  - **Dimensionality Reduction & Visualization**
    - PCA, t-SNE, UMAP for simplification & visualization
    - Reduce dimensionality to improve efficiency, interpretability, and accuracy of vector searches
