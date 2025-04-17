# Direct QR Factorizations for Tall-and-Skinny Matrices in MapReduce

This repository contains the presentation and Python code for our research on stable and scalable QR factorizations for tall-and-skinny matrices using MapReduce. The study is based on the paper:

> **“Direct QR Factorizations for Tall-and-Skinny Matrices in MapReduce Architectures”**  
> *by Austin R. Benson, David F. Gleich, and James Demmel*

---

## 🎯 Project Objective

To implement and evaluate various QR factorization methods for tall-and-skinny matrices in distributed systems, focusing on **Direct TSQR** — a numerically stable, efficient algorithm well-suited for big data environments.

---

## 🧪 Implemented Methods

- `cholesky_qr(A)`
- `householder_qr(A)`
- `indirect_tsqr(A)`
- `direct_tsqr(A)`

Each method is tested for:
- Reconstruction Error: `‖A - QR‖`
- Orthogonality: `‖QᵀQ - I‖`

---

## 📂 Files in this Repo

| File | Description |
|------|-------------|
| `presentation.pdf` | Slide deck summarizing the background, algorithm, implementation, and results |
| `qr_methods.ipynb` | Jupyter Notebook implementing and evaluating the factorization techniques |
| `README.md` | You're here! |

---

## 🖥️ Environment & Tools

- Python with **Dask** for parallel/distributed computation
- NumPy & SciPy for numerical operations
- Jupyter for demonstration and analysis

---

## 📊 Results Summary

- **Cholesky QR**: Fast but unstable on ill-conditioned matrices
- **Householder QR**: Accurate but not scalable
- **Indirect TSQR**: Accurate R, unstable Q
- **Direct TSQR**: Best trade-off between performance and accuracy

---

## 📈 Use Cases

- Distributed Linear Algebra
- Machine Learning (e.g., PCA, least squares)
- Scientific Computing with large datasets
- Big Data Systems using Hadoop/Spark

---

## 📎 Reference

The original paper and implementation:  
🔗 [https://github.com/arbenson/mrtsqr](https://github.com/arbenson/mrtsqr)

---

## 👩‍💻 Authors

- **Manami Das** - MDS202423  
- **Maria Paul Thurkadayil** - MDS202424  
- **Mohit Singh Sinsniwal** - MDS202425

Guided by **Prof. Kavita Sutar**

---

## 📜 License

This project is for academic and educational purposes only.
