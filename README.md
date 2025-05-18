# Обнаружение паттернов изменения давления в нефтяных скважинах

## Описание проекта
Этот проект посвящен разработке решения для автоматического обнаружения паттернов изменения давления в нефтяных скважинах в рамках хакатона Siam ML Hack. Основная задача — выделить интервалы восстановления давления (КВД) и падения давления (КПД) во временных рядах. Необходимо разработать модель для бинарной классификации фреймов на предмет наличия полезных данных для ГДИС с точным определением начала и конца полезных участков данных.

## Структура репозитория
```plaintext
siam-ml-hack/
├── data/                    # Папка для хранения данных
│   ├── raw/                 # Исходные данные (основной датасет, частичная разметка, тестовый датасет)
│   ├── processed/           # Предобработанные данные
│   └── submissions/         # Файлы для сабмита на платформу
├── notebooks/               # Jupyter Notebooks для анализа и экспериментов
│   ├── 01_eda.ipynb         # Исследовательский анализ данных
│   ├── 02_preprocessing.ipynb  # Предобработка данных
│   └── 03_baseline_model.ipynb # Бейзлайн модель
├── src/                     # Исходный код
│   ├── preprocessing.py     # Скрипт для предобработки данных
│   ├── feature_engineering.py # Скрипт для извлечения признаков
│   ├── models.py            # Скрипт для обучения моделей
│   └── utils.py             # Вспомогательные функции
├── config/                  # Конфигурационные файлы
│   └── config.yaml          # Параметры модели и пути к данным
├── requirements.txt         # Зависимости проекта
├── README.md                # Описание проекта
└── .gitignore               # Игнорируемые файлы
```

## Установка и запуск
1. Клонируй репозиторий:
   ```bash
   git clone https://github.com/твой-username/siam-ml-hack.git
   cd siam-ml-hack
   ```

2. Установи зависимости:
   ```bash
   pip install -r requirements.txt
   ```

3. Запусти Jupyter Notebook для анализа:
   ```bash
   jupyter notebook
   ```

## Данные
- **Основной датасет:** Временные ряды давления для обучения модели.
- **Частичная разметка:** Примеры разметки для 100 кейсов.
- **Тестовый датасет:** Данные для тестирования модели.
- **Submit файл:** Шаблон для загрузки предсказаний на платформу.

## Технологии и инструменты
- ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
- ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
- ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
- ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
- ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

## Команда проекта:
1. [Никита Зонтов](https://github.com/zoLikeCode) - ml-специалист и backend-разработчик.
2. [Павел Шабуров](https://github.com/Shavelo) - ml-специалист.

## Лицензия
Этот проект распространяется под лицензией MIT. Подробнее см. в файле [LICENSE](LICENSE).
