# Примеры пайплайнов в Clearml

Данный репозиторий содержит примеры использования пайплайнов в Clearml.

Все крутится вокруг трех шагов:
- скачивания данных из внешнего источника;
- подготовка набора данных;
- обучение модели на подготовленных данных.

## Запуск экспериментов

Эксперименты запускаются локально, поэтому нужно установить окружение

```bash
conda env create --file environment.yml
```

После этого нужно последовательно запустить три скрипта:
- step1_dataset_artifact.py;
- step2_data_processing.py;
- step3_train_model.py.

Это необходимо для того, чтобы в Clearml возникли задачи, на которые пайплайн будет ссылаться.