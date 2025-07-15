# auto-correct
# 🔧 Spell Checker & Sentence Corrector in Python

A lightweight, pure‑Python implementation of a **spell checker** based on
Peter Norvig’s edit‑distance algorithm.  
Given a sentence, it generates candidate corrections that are **one edit
distance** away (insertion, deletion, substitution, transposition) and
returns the most probable word from a large corpus.

---

## 📌 How It Works
1. **Corpus**  
   Loads `big.txt` (1 MB of public‑domain text) and builds a word–frequency
   dictionary with `Counter`.
2. **Edit‑Distance Generation**  
   - **Insertion** of a letter  
   - **Deletion** of a letter  
   - **Substitution** of a letter  
   - **Transposition** of adjacent letters
3. **Probability Ranking**  
   Chooses the candidate with the highest frequency in the corpus.
4. **Sentence Correction**  
   Applies word‑level correction across all tokens in a sentence.

---
