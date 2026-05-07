# AI-Based Intrusion Detection and Prevention System (IDPS)

## Project Description

An advanced machine learning-based Intrusion Detection and Prevention System (IDPS) that leverages the NSL-KDD dataset to identify and classify network traffic anomalies. This system performs both binary classification (normal vs. attack) and multi-class classification (identifying specific attack types including DoS, Probe, R2L, U2R, etc.).

The project demonstrates a complete machine learning pipeline: data preprocessing, exploratory analysis, feature engineering, model training, hyperparameter tuning, and comprehensive evaluation with detailed performance metrics.

Best Results:
- Binary Classification: ~79% accuracy
- Multi-Class Classification: ~72% accuracy
- Random Forest emerged as the top-performing model

---

## Dataset

Name: NSL-KDD (Network Security Lab - Knowledge Discovery in Databases)

Files:
- KDDTrain+.txt - Training dataset
- KDDTest+.txt - Test dataset

Description:
NSL-KDD is a refined and balanced version of the original KDD'99 dataset, specifically designed for benchmarking intrusion detection systems. It contains 125,973 network connection records with labeled attributes indicating normal traffic or specific attack types.

---

## Technologies and Libraries

Language: Python 3.x
Environment: Jupyter Notebook

Key Libraries:
- pandas, numpy - Data manipulation and numerical computing
- scikit-learn - Machine learning models and preprocessing utilities
- matplotlib, seaborn - Data visualization and exploratory analysis
- tensorflow, keras (optional) - Deep learning implementations

---

## Machine Learning Models Implemented

Random Forest Classifier - Ensemble - Best Overall
Decision Tree Classifier - Tree-based - Good Baseline
Support Vector Machine (SVM) - Kernel-based - Competitive
K-Nearest Neighbors (KNN) - Instance-based - Exploratory
Multi-Layer Perceptron (MLP) - Neural Network - Experimental

---

## Data Preprocessing Pipeline

1. Feature Handling
   - Separation of categorical and numerical features
   - One-Hot Encoding for categorical variables
   - Min-Max Scaling (0-1 normalization) for numerical features

2. Label Encoding
   - Binary classification: Normal vs. Attack
   - Multi-class classification: 5 attack categories + Normal

3. Data Splitting
   - Official NSL-KDD train/test split preservation
   - No data leakage between train and test sets

---

## Classification Tasks

Task 1: Binary Classification
- Class 0: Normal traffic
- Class 1: Any attack type

Task 2: Multi-Class Classification
- Class 0: Normal traffic
- Class 1: DoS (Denial of Service)
- Class 2: Probe (Reconnaissance)
- Class 3: R2L (Remote to Local)
- Class 4: U2R (User to Root)

---

## Evaluation Metrics

- Accuracy - Overall correctness
- Precision (Weighted) - False positive rate per class
- Recall (Weighted) - False negative rate per class
- F1-Score - Harmonic mean of precision and recall
- Confusion Matrix - Detailed classification breakdown
- Feature Importance - Most influential attributes for detection

---

## Key Results

Metric | Binary Classification | Multi-Class Classification
Accuracy | ~79% | ~72%
Precision | 0.78 | 0.71
Recall | 0.79 | 0.72
F1-Score | 0.78 | 0.71

Winner: Random Forest Classifier demonstrated superior performance across all metrics.

---

## Project Structure

idps-project/
├── KDDTrain+.txt - Training data
├── KDDTest+.txt - Test data
├── idps_project.ipynb - Main notebook with full pipeline
├── README.md - Project documentation
└── /models/ - (Optional) Saved trained models

---

## Applications

- Academic Research - Cybersecurity curriculum and ML coursework
- Skill Demonstration - Portfolio project for Data Science/ML/Security roles
- Practical Learning - Hands-on experience with real-world security datasets
- Baseline System - Foundation for production IDS/IPS systems

---

## Future Enhancements

- Class Imbalance Handling - Implement SMOTE, class weights, or cost-sensitive learning
- Advanced Deep Learning - LSTM, CNN, or Transformer-based models
- Real-Time Detection - Integration with live network traffic streams
- Model Deployment - REST API or containerized microservice
- Hyperparameter Optimization - Grid search or Bayesian optimization
- Explainability - SHAP values, LIME, or attention mechanisms

---

## Author

Developed as an academic and portfolio project to demonstrate machine learning and cybersecurity expertise.

---

## License

Open for educational and research purposes.

# Система обнаружения и предотвращения вторжений на основе ИИ (IDPS)

## Описание проекта

Продвинутая система обнаружения и предотвращения сетевых вторжений (IDPS) на основе методов машинного обучения, использующая датасет NSL-KDD для выявления и классификации аномалий сетевого трафика. Система выполняет как бинарную классификацию (нормальный трафик vs. атака), так и многоклассовую классификацию (определение конкретных типов атак: DoS, Probe, R2L, U2R и другие).

Лучшие результаты:
- Бинарная классификация: ~79% точность
- Многоклассовая классификация: ~72% точность
- Random Forest показал лучшую производительность

---

## Датасет

Название: NSL-KDD (Network Security Lab - Knowledge Discovery in Databases)

Файлы:
- KDDTrain+.txt - Набор данных для обучения
- KDDTest+.txt - Набор данных для тестирования

Описание:
NSL-KDD - это усовершенствованная и сбалансированная версия исходного датасета KDD'99, специально разработанная для бенчмаркинга систем обнаружения вторжений. Содержит 125,973 записей сетевых соединений с метками, указывающими на нормальный трафик или конкретные типы атак.

---

## Технологии и библиотеки

Язык программирования: Python 3.x
Среда разработки: Jupyter Notebook

Основные библиотеки:
- pandas, numpy - Обработка данных и численные вычисления
- scikit-learn - Машинное обучение и предобработка данных
- matplotlib, seaborn - Визуализация и исследовательский анализ
- tensorflow, keras (опционально) - Реализация глубокого обучения

---

## Реализованные модели машинного обучения

Random Forest Classifier - Ансамбль - Лучшая
Decision Tree Classifier - Дерево решений - Хорошая базовая модель
Support Vector Machine (SVM) - Метод опорных векторов - Конкурентная
K-Nearest Neighbors (KNN) - На основе экземпляров - Экспериментальная
Multi-Layer Perceptron (MLP) - Нейронная сеть - Экспериментальная

---

## Конвейер предобработки данных

1. Обработка признаков
   - Разделение категориальных и числовых признаков
   - One-Hot Encoding для категориальных переменных
   - Min-Max нормализация для числовых признаков

2. Кодирование меток
   - Бинарная классификация: Норма vs. Атака
   - Многоклассовая классификация: 5 типов атак + Нормальный трафик

3. Разделение данных
   - Сохранение официального разделения train/test NSL-KDD
   - Предотвращение утечки данных между выборками

---

## Задачи классификации

Задача 1: Бинарная классификация
- Класс 0: Нормальный трафик
- Класс 1: Любой тип атаки

Задача 2: Многоклассовая классификация
- Класс 0: Нормальный трафик
- Класс 1: DoS (Отказ в обслуживании)
- Класс 2: Probe (Разведка)
- Класс 3: R2L (Удаленный доступ к локальной системе)
- Класс 4: U2R (Повышение привилегий)

---

## Метрики оценки

- Accuracy - Общая корректность предсказаний
- Precision - Процент верно предсказанных положительных примеров
- Recall - Процент обнаруженных примеров из всех положительных
- F1-Score - Гармоническое среднее точности и полноты
- Confusion Matrix - Детальная матрица ошибок классификации
- Feature Importance - Анализ важности признаков для обнаружения

---

## Ключевые результаты

Метрика | Бинарная классификация | Многоклассовая классификация
Accuracy | ~79% | ~72%
Precision | 0.78 | 0.71
Recall | 0.79 | 0.72
F1-Score | 0.78 | 0.71

Победитель: Random Forest Classifier продемонстрировал превосходную производительность по всем метрикам.

---

## Структура проекта

idps-project/
├── KDDTrain+.txt - Данные для обучения
├── KDDTest+.txt - Данные для тестирования
├── idps_project.ipynb - Основной ноутбук с полным конвейером
├── README.md - Документация проекта
└── /models/ - Сохраненные модели

---

## Применение

- Академические исследования - Учебные курсы по кибербезопасности и МО
- Демонстрация навыков - Портфолио проект для специалистов Data Science/ML/Security
- Практическое обучение - Практический опыт с реальными датасетами безопасности
- Базовая система - Основание для production IDS/IPS систем

---

## Возможные улучшения

- Обработка дисбаланса классов - Применение SMOTE, весов классов или cost-sensitive обучения
- Продвинутое глубокое обучение - LSTM, CNN или Transformer-модели
- Детектирование в реальном времени - Интеграция с потоками живого сетевого трафика
- Развертывание модели - REST API или микросервис в контейнере
- Оптимизация гиперпараметров - Grid Search или Bayesian Optimization
- Интерпретируемость - SHAP values, LIME или механизмы внимания

---

## Автор

Разработано как академический и портфолио проект для демонстрации экспертизы в машинном обучении и кибербезопасности.

---

## Лицензия

Открыто для образовательных и исследовательских целей.
