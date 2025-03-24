## 📊 О проекте
Комплексный анализ и сравнение эффективности различных моделей машинного обучения для прогнозирования продаж в сети магазинов BigMart. Проект включает полный цикл работы с данными: от предобработки до оценки моделей.

## 🔍 Основные компоненты анализа

### Предобработка данных
- Унификация категорий в `Item_Fat_Content`
- Создание новых информативных признаков:
  - `num_years` (срок работы магазина)
  - `Item_MRP_Scaled` (логарифмированная цена)
  - `Item_Visibility_Scaled` (логарифмированная видимость товара)
- Обработка пропущенных значений с учетом бизнес-логики

### Инженерия признаков
- Масштабирование числовых признаков
- Кодирование категориальных переменных
- Создание производных метрик

### Сравниваемые модели
1. Linear Regression
2. Ridge Regression (α=1.0)
3. Lasso Regression (α=1.0)
4. Random Forest (n_estimators=200, max_depth=4)
5. XGBoost (n_estimators=200, max_depth=4, learning_rate=0.1)
6. Gradient Boosting (n_estimators=200, max_depth=4, learning_rate=0.1)
7. SVR (kernel='rbf', C=1.0, ε=0.1)

## 📈 Метрики оценки
- RMSE (Root Mean Square Error)
- MAE (Mean Absolute Error)
- R² (Coefficient of Determination)

## 🚀 Как использовать

### Требования
```requirements.txt
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
```
