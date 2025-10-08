# CS230 – Lecture 2: Supervised, Self-Supervised, & Weakly Supervised Learning

**Date:** 2025-10-08  
**Instructor:** Kian Katanforoosh  

---

## Core Concept

A **Model** is composed of two essential parts:

- **Architecture** → The blueprint or design of the neural network.  
- **Parameters** → The numerical values (weights and biases) that the model learns during training.

---

## Feature Engineering vs. Feature Learning

| Concept | Description |
|----------|--------------|
| **Feature Engineering** | Manual process where humans specify which features to use. |
| **Feature Learning** | Automatic process — the network learns the important features on its own. |

---

## Encodings & Embeddings

- **Encoding:** Any representation of data in vector form.  
- **Embedding:** A type of encoding where **closeness in space = semantic similarity**.  
- **One-Hot Vector:** Exactly one thing is true.  
- **Multi-Hot Vector:** Multiple things can be true at once.

---

## Practical Tips

- Use a **known proxy project** to estimate how much data you need.  
- **Be scrappy:** if you can’t run large-scale experiments, test with human approximations.  
  - Example: to find good image resolution, ask friends to classify images manually.  
- **Data collection** strategy is *critical* to project success — don’t hesitate to “get out of the building.”  
- Run **human experiments** to refine labeling strategies.  
- **Consult experts** early to avoid wasting time and to steer in a good direction.

---

## Example: Face Verification System

In **face verification**, an **encoder network** learns to represent faces in a lower-dimensional **encoding** space by focusing on non-noisy, identity-preserving features.

---

## Triplet Loss Function

Used in face verification and embedding learning.

Let:
- **Anchor (A)** → Reference image  
- **Positive (P)** → Same identity as anchor  
- **Negative (N)** → Different identity  

**Goal:**  
- Minimize distance: `distance(A, P)`  
- Maximize distance: `distance(A, N)`

**Triplet Loss Formula:**
\[
L(A, P, N) = \max(0, ||f(A) - f(P)||^2 - ||f(A) - f(N)||^2 + \alpha)
\]

Where **α (alpha)** is a margin that ensures separation.

---

## Face-Related Tasks

| Task | Goal |
|------|------|
| **Face Verification** | Check if two faces are of the same person. |
| **Face Identification** | Match a face to a known identity from a set. |
| **Face Clustering** | Group similar faces without predefined labels. |

---

## Key Takeaways

- Neural networks automatically learn hierarchical features.  
- Data quality and labeling strategy often matter more than architecture choice.  
- Embeddings enable similarity-based reasoning and clustering.  
- Triplet loss helps models learn discriminative representations.

---

**End of Lecture 2 Notes**
