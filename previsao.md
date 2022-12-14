# Considerações Gerais - Previsão

Modelos estatísticos conseguem prever acontecimentos futuros, porém são sempre sujeitos a variações.

**Razões**: Porque as variáveis que fazem parte do modelo podem variar, ou pode haver variáveis desconhecidas. Exemplo: Prever um campeão numa copa do mundo. Existem muitas variáveis como Lesões dos jogadores, Condicionamento, Habilidades, Motivação, Local, Esquema Tático, Horário, Clima, Torcida, Árbitros, Gramado, etc.

Em teoria, toda previsão está errada, logo o objetivo é minimizar o erro.

Quanto maiores dados/informações completas sobre um assunto, melhor podemos minimizar o erro de uma previsão.

## Como prever ST?

- Usando próprios dados - ST puras
- Usando outras variáveis - Modelo Explanatório
- Usando as duas técnicas - Modelo misto

## Regressão VS Séries Temporais

Na regressão eu posso usar o modelo para extrapolar os dados conhecidos, mas também dentro dos intervalos de dados. Na Série Temporal só faz sentido extrapolar os dados para além dos dados conhecidos.

**Previsão somente funcionam à partir de um padrão**. Para dados aleatórios teremos somente adivinhação.

## Dois pontos importantes

1 - A previsão sofre maior variabilidade (menor previsibilidade) quando vai mais para frente na série extrapolada, pois as variáveis podem sofrer alterações com o passar do tempo.

2 -  Dados históricos mais antigos tem menor peso na influência do modelo de previsão.

3 - Existe o ponto de previsão e os intervalos (variações para cima e para baixo do ponto) de previsão. Tudo isso se chama de **distribuição da previsão**

## Se existe incerteza, por que prever?

É ainda a melhor forma por ser científica. Existem casos que conseguimos resultados satisfatórios.

## Um bom modelo

- Para conseguirmos bom modelo, precisamos: 1 - Avaliar residuais. 2 - Avaliar Performance (MAE, RMSE). 3 - Avaliar Métricas (AIC, BIC)

Dicas:

- Residuais ok não são suficientes;
- Sempre há espaço para mehorias;
- Somente informações relevantes para aplicar o modelo.