# GARCH-модель для прогнозирования временного ряда

## Описание проекта  
В этом проекте мы анализируем временной ряд количества международных авиапассажиров и применяем модель **GARCH** для прогнозирования изменчивости ряда.

## Данные  
Используемый набор данных: **international-airline-passengers.csv**  
- **Период**: 1949-1960 гг.  
- **Переменная**: Количество пассажиров в месяц  

## Этапы работы  
1. **Загрузка данных** и предобработка  
2. **Преобразование Бокса-Кокса** для стабилизации дисперсии  
3. **Первое дифференцирование** для устранения тренда  
4. **Сезонное дифференцирование** для устранения сезонности  
5. **Обучение модели GARCH** и кросс-валидация  
6. **Оценка точности модели и визуализация результатов**  

## Итоги  
- **Оптимальные параметры модели GARCH**: (p=1, q=2)  
- **Метрики качества** (по Rolling Forecast CV):  
  - **MAE**: 0.1104  
  - **MSE**: 0.0197  
  - **RMSE**: 0.1402  

## Как запустить код  
1. **Клонировать репозиторий**:  
```bash  
git clone https://github.com/ТВОЙ_РЕПО.git  
cd ТВОЙ_РЕПО  
```
2. **Запустить Jupyter Notebook** или Colab  
3. **Запустить ячейки последовательно**  

## Структура проекта  
```
📂 project_root/
├── 📂 notebooks/      # Основной код в Jupyter Notebook
├── 📂 data/           # Файл с данными
├── 📂 models/         # Сохранённые параметры модели
└── README.md          # Описание проекта
```

## Выводы  
- Применение Бокса-Кокса, дифференцирования и сезонного дифференцирования позволило добиться **стационарности** ряда  
- Модель **GARCH(1,2)** показала **низкую ошибку** и хорошо предсказала изменчивость ряда  
- Возможны улучшения за счёт подбора **других параметров p, q** или использования **гибридных моделей**  



