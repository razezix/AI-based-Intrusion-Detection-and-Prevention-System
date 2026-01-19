# AI-Based Intrusion Detection and Prevention System (IDPS)

## 📌 Project Overview
This project implements an **AI-based Intrusion Detection and Prevention System (IDPS)** using machine learning techniques and the **NSL-KDD dataset**.  
The system is designed to detect malicious network traffic and classify it as either **normal** or **attack**, as well as identify **specific attack types** (multi-class classification).

The project demonstrates the full machine learning pipeline: data preprocessing, feature engineering, model training, evaluation, and analysis of results.

---

## 📂 Dataset
- **Name:** NSL-KDD
- **Files used:**
  - `KDDTrain+.txt`
  - `KDDTest+.txt`
- **Description:**  
  NSL-KDD is a refined version of the KDD’99 dataset, widely used for benchmarking intrusion detection systems.  
  It contains network traffic records labeled as normal activity or different types of attacks.

---

## ⚙️ Technologies Used
- **Programming Language:** Python  
- **Environment:** Jupyter Notebook  

### Libraries:
- `pandas`, `numpy` — data processing and analysis  
- `scikit-learn` — machine learning models and preprocessing  
- `matplotlib`, `seaborn` — data visualization  
- *(optional)* `tensorflow / keras` — deep learning models  

---

## 🧠 Implemented Models
- Random Forest Classifier  
- Decision Tree Classifier  
- *(optional / experimental)*  
  - Support Vector Machine (SVM)  
  - K-Nearest Neighbors (KNN)  
  - Multi-layer Perceptron (MLP)  

---

## 🔄 Data Preprocessing
- Handling categorical and numerical features
- One-Hot Encoding for categorical variables
- Min-Max scaling for numerical features
- Binary and multi-class label encoding
- Train/Test separation using official NSL-KDD splits

---

## 📊 Classification Tasks
### 1. Binary Classification
- **Normal traffic**
- **Attack traffic**

### 2. Multi-Class Classification
- Normal traffic
- Multiple attack categories (DoS, Probe, R2L, U2R, etc.)

---

## 📈 Evaluation Metrics
- Accuracy
- Precision (weighted)
- Recall (weighted)
- F1-score
- Confusion Matrix
- Feature Importance (Random Forest)

---

## ✅ Results Summary
- **Binary Classification Accuracy:** up to ~79%
- **Multi-Class Classification Accuracy:** up to ~72%
- Random Forest showed the best overall performance
- Key influential features were identified using feature importance analysis

---

## 📁 Project Structure
├── KDDTrain+.txt
├── KDDTest+.txt
├── idps_project.ipynb
├── README.md

yaml
Копировать код

---

## 🎯 Purpose of the Project
- Academic research and coursework
- Demonstration of machine learning skills
- Cybersecurity & intrusion detection practice
- Portfolio project for Data Science / ML / Security roles

---

## 🚀 Future Improvements
- Class imbalance handling (SMOTE, class weights)
- Advanced deep learning models
- Real-time traffic simulation
- Integration with real IDS/IPS systems

---

## 👤 Author
Developed as part of an academic and portfolio project.

🇷🇺 README (Russian Version)
md
Копировать код
# Система обнаружения и предотвращения вторжений на основе ИИ (IDPS)

## 📌 Описание проекта
Данный проект представляет собой **систему обнаружения и предотвращения вторжений (IDPS)** на основе методов машинного обучения с использованием датасета **NSL-KDD**.  
Система предназначена для обнаружения вредоносного сетевого трафика и его классификации как **нормального** или **атаки**, а также для определения **конкретных типов атак** (многоклассовая классификация).

Проект демонстрирует полный цикл машинного обучения: предобработку данных, обучение моделей, оценку качества и анализ результатов.

---

## 📂 Датасет
- **Название:** NSL-KDD
- **Используемые файлы:**
  - `KDDTrain+.txt`
  - `KDDTest+.txt`
- **Описание:**  
  NSL-KDD — улучшенная версия датасета KDD’99, широко используемая для тестирования систем обнаружения вторжений.  
  Содержит сетевые соединения с метками нормального трафика и различных типов атак.

---

## ⚙️ Используемые технологии
- **Язык программирования:** Python  
- **Среда разработки:** Jupyter Notebook  

### Библиотеки:
- `pandas`, `numpy` — обработка и анализ данных  
- `scikit-learn` — машинное обучение и предобработка  
- `matplotlib`, `seaborn` — визуализация данных  
- *(опционально)* `tensorflow / keras` — глубокое обучение  

---

## 🧠 Реализованные модели
- Random Forest  
- Decision Tree  
- *(опционально / экспериментально)*  
  - SVM  
  - KNN  
  - MLP  

---

## 🔄 Предобработка данных
- Разделение числовых и категориальных признаков
- One-Hot Encoding для категориальных данных
- Нормализация числовых признаков (Min-Max Scaling)
- Бинарное и многоклассовое кодирование меток
- Использование официальных train/test выборок NSL-KDD

---

## 📊 Задачи классификации
### 1. Бинарная классификация
- Нормальный трафик
- Атака

### 2. Многоклассовая классификация
- Нормальный трафик
- Различные типы атак (DoS, Probe, R2L, U2R и др.)

---

## 📈 Метрики оценки
- Accuracy
- Precision (взвешенная)
- Recall (взвешенная)
- F1-score
- Матрица ошибок
- Анализ важности признаков

---

## ✅ Результаты
- **Точность бинарной классификации:** до ~79%
- **Точность многоклассовой классификации:** до ~72%
- Наилучшие результаты показал Random Forest
- Определены ключевые признаки, влияющие на обнаружение атак

---

## 📁 Структура проекта
├── KDDTrain+.txt
├── KDDTest+.txt
├── idps_project.ipynb
├── README.md

yaml
Копировать код

---

## 🎯 Цель проекта
- Учебный и исследовательский проект
- Демонстрация навыков машинного обучения
- Практика в области кибербезопасности
- Портфолио для Data Science / ML / Security позиций

---

## 🚀 Возможные улучшения
- Устранение дисбаланса классов
- Использование более сложных DL-моделей
- Моделирование реального сетевого трафика
- Интеграция с реальными IDS/IPS системами

---

## 👤 Автор
Проект выполнен в учебных и портфолио целях.
