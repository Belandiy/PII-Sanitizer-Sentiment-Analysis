# Text Data Sanitization (PII Removal) & Sentiment Analysis

A demonstration of data preparation for LLM training. In commercial environments, it's critical to mask Personal Identifiable Information (PII) before feeding data to models to prevent data leakage. This project showcases regex-based PII masking and subsequent sentiment classification.

## 📋 Описание проекта

Цель этого проекта — продемонстрировать процесс подготовки текстовых данных для безопасного использования в моделях машинного обучения. Мы реализуем очистку текстов от персонально идентифицируемой информации (PII) с помощью регулярных выражений и проведем анализ тональности отзывов на очищенных данных.

Основные этапы:
1.  **Генерация "грязных" данных**: Программная вставка фейковых email-адресов и номеров телефонов в отзывы.
2.  **Очистка (Sanitization)**: Использование регулярных выражений для замены PII на специальные токены.
3.  **Sentiment Analysis**: Обучение модели классификации для определения тональности отзывов (позитивный/негативный).

## 🛠 Технологии и инструменты

*   **Python 3.x**
*   **pandas** — обработка и анализ данных.
*   **re (Regex)** — очистка персональных данных.
*   **scikit-learn** — векторизация текста (Tfidf) и обучение модели классификации.
*   **nltk** — базовая предобработка текста.

## 🚀 Как запустить

1.  Убедитесь, что у вас установлен Python.
2.  Установите необходимые библиотеки:
    ```bash
    pip install pandas numpy scikit-learn nltk jupyter
    ```
3.  Запустите Jupyter Notebook:
    ```bash
    jupyter notebook pii_sanitizer_sentiment.ipynb
    ```

## 📊 Результаты

В ноутбуке представлены примеры текстов до и после очистки, а также метрики качества модели (Accuracy, F1-score), обученной на обезличенных данных.
