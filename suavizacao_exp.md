# Suavização Exponencial

Uma das técnicas mais importantes para aplicação em ST. Existem várias técnicas de Suavização.

## Princípios Básicos
-----------------------------------
- Intervalos passados possuem pesos. Quanto mais recentes, maior peso;
- Utiliza médias para observações mais distantes;
- Parametro que determina indice de redução entre 0 e 1:
    - Próximo de 0: antigas maior peso.
    - Próximo de 1: recentes maior peso.

## Suavização Simples
-----------------------------------
- Não considera tendencia ou sazonalidade

## Tendencia Linear de Hold (1957)
-----------------------------------
- Para dados com tendencia;
- Gera tendencia linear para futuro;
- Bem antiga.

## Tendencia Amortecida (1985)
-----------------------------------
- Diferente da anterior que vai "reto" até o infinito, essa amortece a tendencia conforme a previsão avança;
- Padrão de amortecimento entre 0 e 1;
- tendencia que o crescimento sofra uma amortização.

## Holt-Winters Sazonal (1960)
-----------------------------------
- Mais sofisticada, pois captura sazonaldade além da tendencia;
- Pode ser Aditiva (sazonal constante) ou Multiplicativa (sazonal variável).

## ETS (Error, Trend, Seasonal)
-----------------------------------
- Método poderoso de previsão baseado na suavização exponencial.
- Suporta sazonalidade e tendencia
- Existem técnicas que podem achar o melhor modelo automaticamente.


## Texto resumo
____________

As técnicas de suavização exponencial são um **tipo de modelo de previsão de séries temporais que buscam suavizar a tendência e a sazonalidade de uma série temporal**. Elas são baseadas no uso de uma média móvel exponencial, que **dá mais peso às observações mais recentes e menos peso às observações mais antigas**.

Existem basicamente dois **tipos de técnicas**de suavização exponencial: (1) o modelo de suavização exponencial simples (SES, na sigla em inglês) e (2) o modelo de suavização exponencial com tendência e sazonalidade (ETS, na sigla em inglês).

**O modelo SES é adequado para séries temporais estacionárias**, ou seja, aquelas que não apresentam tendência ou sazonalidade. Ele é usado para suavizar a variabilidade da série temporal e prever seus valores futuros.

Já **o modelo ETS é adequado para séries temporais não estacionárias**, ou seja, aquelas que apresentam tendência ou sazonalidade. Ele é usado para suavizar a tendência e a sazonalidade da série temporal e prever seus valores futuros.

**Ambos os modelos são geralmente utilizados em conjunto com outros modelos de previsão, como o modelo ARIMA**, para ajustar ainda mais a previsão dos valores futuros da série temporal.


