# Arima

Uma das técnicas específicas para previsão de Séries Temporais.

## Arima não Sazonal
------
- Pode ser usado em qualquer ST, pois é bem robusto.
- Dados precisam ter poucos outliers
- **Requer dados estacionários**: podem ser dados transformados por diferenciação: remove tendencias.

Tem três partes:
- AR: Autoregressivo - avalia e extrai influência da relação entre períodos   
- I: Integrado - Aplica diferenciação, se necessária
- MA: Moving Average - avalia erros e extrai.

Formado por:

- p = ordem da parte autoregressiva
- d = grau de diferenciação
- q = ordem da média móvel
![arima](arima.png "Title")

## Arima Sazonal
-------
- Inclui elementos P,D e Q, tornando elemento mais complexo.
- Opção em tirar sazonalidade da ST e aplicar o Arima padrão.

### Como definir valores de p, d e q?

- p: PACF
- d: Teste de Estacionariedade
- q: ordem de média móvel: ACF

### Como saber qual o melhor modelo?

Através de métricas: AIC e BIC. Precisa testá-las e minimizar o valor resultado.

Não confundir métrica do modelo com métrica da previsão dos dados.

## Processo

1 - Exploração - decomposição, teste de estacionariedade, diagramas de acf e pacf (autocorrelação).
2 - Modelo - desenvolver modelo
3 - Residuais - Avaliar os residuais
4 - Previsão - aplicar modelo e gerar resultados





