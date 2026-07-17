# Как запустить проект

## Требования

- Python 3.9+
- Jupyter Notebook или JupyterLab

## Установка

1. Склонируйте репозиторий:

   ```bash
   git clone <ссылка-на-репозиторий>
   cd <папка-репозитория>
   ```

2. Создайте и активируйте виртуальное окружение:

   ```bash
   python -m venv venv
   source venv/bin/activate      # Linux/macOS
   venv\Scripts\activate         # Windows
   ```

3. Установите зависимости:

   ```bash
   pip install -r requirements.txt
   ```

## Данные

Файл `Metrika_dannye_VRP_bez_summarnykh_pokazateley_new.csv` должен лежать в корне репозитория (или в той папке, откуда его читает ноутбук).

## Запуск

1. Запустите Jupyter:

   ```bash
   jupyter notebook
   ```

2. Откройте ноутбук проекта (`<имя_ноутбука>.ipynb`) и выполните ячейки по порядку (Kernel → Restart & Run All).

## Примечания

- Оценка 2SLS через `linearmodels.iv.IV2SLS` и тесты (Стока-Його, Ву-Хаусман, Вулдридж, Бройша-Пагана, Уайта) считаются быстро — тяжёлых вычислений в ноутбуке нет.
- Графики (`boxplots_clean.png`, `histograms_log.png`, `correlation_heatmap.png`), на которые ссылается README, сохранены в `assets/`; при повторном запуске ноутбука они не перезаписываются автоматически.
