<h1 align="center">Diabetes Prediction Dataset</h1>

## Sumário

* [Objetivo](#objetivo)
* [Dataset](#dataset)
* [Resultados](#resultados)
* [Gráficos](#gráficos)
* [Conclusão](#conclusão)
* [Perguntas](#perguntas)

## Objetivo
Implementar e comparar algoritmos de classificação supervisionada em um conjunto de dados real, por meio da aplicação de técnicas de pré-processamento, modelagem e avaliação de desempenho.

## Dataset
**Fonte:** [Diabetes prediction dataset](https://www.kaggle.com/datasets/iammustafatz/diabetes-prediction-dataset)

**Features:** Gender, Age, Hypertension, Heart Disease, Smoking History, BMI, HbA1c Level, Blood Glucose Level e Diabetes.

**Variável Alvo:** `Diabetes`

**Justificativa:** Escolhi o dataset de diabetes por ser bem estruturado e apresentar ótimos dados para fazer predições e classificações. O conjunto de dados pode ser utilizado para fazer classificações simples quanto classificações mais profundas. Eu pretendo utilizar o dataset futuramente para análises mais aprofundadas.

## Resultados

***DECISION TREE***

```
Acurácia: 0.9529
Matriz de Confusão:
 [[17815   477]
 [  464  1244]]
Relatório de Classificação:
               precision    recall  f1-score   support

           0       0.97      0.97      0.97     18292
           1       0.72      0.73      0.73      1708

    accuracy                           0.95     20000
   macro avg       0.85      0.85      0.85     20000
weighted avg       0.95      0.95      0.95     20000

F1-Score (weighted): 0.9530
```

***KNN***
```
Acurácia: 0.9544
Matriz de Confusão:
 [[18182   110]
 [  802   906]]
Relatório de Classificação:
               precision    recall  f1-score   support

           0       0.96      0.99      0.98     18292
           1       0.89      0.53      0.67      1708

    accuracy                           0.95     20000
   macro avg       0.92      0.76      0.82     20000
weighted avg       0.95      0.95      0.95     20000

F1-Score (weighted): 0.9490
```

***LOGISTIC REGRESSION***
```
Acurácia: 0.9590
Matriz de Confusão:
 [[18127   165]
 [  654  1054]]
Relatório de Classificação:
               precision    recall  f1-score   support

           0       0.97      0.99      0.98     18292
           1       0.86      0.62      0.72      1708

    accuracy                           0.96     20000
   macro avg       0.91      0.80      0.85     20000
weighted avg       0.96      0.96      0.96     20000

F1-Score (weighted): 0.9559
```
## Gráficos

## Conclusão
**`Qual modelo apresentou melhor desempenho no dataset escolhido?`**

Todos os modelos apresentaram resultados muito próximos. No entanto, por pouco, o modelo de Regressão Logística apresentou o melhor desempenho (acurácia = 0.9590; F1-Score = 0.9559).

**`O resultado faz sentido? (justificar com base nos dados)`**

Sim, todos os modelos apresentaram bons resultados e o fato do modelo de regressão logística ter o melhor desempenho faz sentido, pois ele apresentou um bom equilíbrio na precisão e no recall para as duas classes, o que é necessário para datasets desbalanceados.

**`O que poderia ser feito para melhorar os modelos (ex: normalização, mais features, tuning de hiperparâmetros)?`**

Acredito que uma melhoria para os modelos seria o tratamento de dados desbalanceados, pois eles dificultam a classificação. Além disso, acredito que seria interessante fazer o treinamento com outros modelos também.

## Perguntas
As respostas das perguntas feitas no documento estão no notebook `perguntas` e no final do notebook `diabetes_prediction`
