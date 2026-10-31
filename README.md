# Iris Flower Classification in C++(CodeAlpha_task-1)

A lightweight, high-performance C++ implementation of the **K-Nearest Neighbors (KNN)** machine learning algorithm for classifying Iris flower species from standard CSV datasets.

---

## 📌 Project Overview

This project implements machine learning fundamentals directly in modern C++ without relying on external ML libraries. It parses raw dataset records from a CSV file, performs a deterministic train-test split, computes Euclidean distance matrices, and performs multi-class classification using majority voting.

### Key Features
* **Custom Dataset Parser:** Handles standard Iris CSV formats, variable column structures, carriage returns (`\r`), and missing/malformed rows.
* **Exact KNN Classifier:** Implements Euclidean distance metric calculation and majority voting for $K=3$ nearest neighbors.
* **Automated Data Splitting:** Performs an 80/20 train-test split without external dependencies.
* **Performance Evaluation:** Computes and displays overall test accuracy percentage upon execution.

---

## 🛠️ Tech Stack & Concepts

* **Language:** C++11 (or higher)
* **Standard Library Components:** `std::vector`, `std::stringstream`, `std::fstream`, `std::algorithm`
* **Algorithm:** K-Nearest Neighbors (KNN)
* **Distance Metric:** Euclidean Distance ($d = \sqrt{\sum_{i=1}^n (x_i - y_i)^2}$)

---

## 📂 Dataset Format

The program expects an `iris.csv` file located in the project root directory. It gracefully parses both standard 5-column CSV files and 6-column exports (e.g., datasets including an `Id` column).

Expected label mapping:
| Class Label | Target Name |
| :--- | :--- |
| **0** | `Iris-setosa` / `setosa` |
| **1** | `Iris-versicolor` / `versicolor` |
| **2** | `Iris-virginica` / `virginica` |

---

## 🚀 Getting Started

### Prerequisites
Make sure you have a standard C++ compiler installed:
* `g++` (GCC) or `clang++`
* `make` (optional)

### Installation & Execution

1. **Clone the Repository**
   ```bash
   git clone [https://github.com/your-username/iris-classification-cpp.git](https://github.com/your-username/iris-classification-cpp.git)
   cd iris-classification-cpp# codealpha_tasks-1
