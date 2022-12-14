# Definição

O que são séries temporais? 

R: Dados coletados em intervalos Regulares de Tempo (precisam ser regulares)

Exemplos: _Dados consolidados em dias, horas, segundos, anos, etc._

**Os dados Precisam estar vinculados com o tempo**

Exemplos de dados temporais: Cotação da bolsa por minuto, total de produção de carros por mês, toneladas de soja colhidas por dia, nascimentos por ano no estado de são paulo, etc.

## Componentes de Série temporal
------------------------------
- Medida: "Total de..."
- Fato: "...produção de pneus..."
- Unidade de Tempo: "...por semana."

## Ordem
--------------------------------
Toda série temporal precisa ter ordem dos registros.

Exemplo: dados de total de drogas apreendidas por mês em Kt

------------>>>>>>>>>>>>>>>>>>>>>
01-2022 | 02-2022 | 03-2022 | 04-2022
---------|----------|------------|---------
215 | 512 | 470 | 190

**Não pode mudar a granularidade dos dados** (Ex: de mês para dia)

## Razão das Séries Temporais
--------------------------------
- Compreender e prever aproximadamente os eventos

## Termos
____________________________
- Crescimento Linear
- Sazonalidades
- Histograma
- Irregular
- Tendencia
- Períodos com falta de dados

Para que consigamos aplicar as técnicas estatísticas e prever, precisamos de dados que nos tragam padrões de comportamento. Com dados aleatórios não podemos fazer melhor do que a média por exemplo.

Dados mais recentes tem peso maior na aplicação de previsões.

## Componentes de uma Série Temporal
_________________________________
- Tendência: aumento de dados ou redução dos mesmos ao longo prazo. Não se aplica em dados aleatórios.
- Sazonalidade: padrões que ocorrem em intervalos fixos (Exemplo, compras aumentam no final do ano)
- Ciclo: aumento ou redução de frequência em intervalos dinâmicos. Exemplo: Crise Economica.
- Erro: Não da para explicar matematicamente. Pode ser chamado de diferença ou resto.

## Autocorrelação
____________________________________
- É o mesmo que correlação, porém aplicada na mesma variável que são dois intervalos de uma mesma série temporal.
- Resultado deve entre -1 e 1, sendo zero a ausência de autocorrelação.
- Medida em intervalos (lag)

### Autocorrelação - ACF

### Autocorrelação - PACF

### Com sazonalidade e tendencia
- Tendencia: tende a ser grande e positiva.
- Com Sazonalidade: Temde a ser maior nos intervalos com maiores valores.

### Ruído Branco
- Não apresenta autocorrelação. Isso tem que ocorrer quando menos de 5% dos intervalos fora da linha de significancia.

## Residuais, Valores Ajustados e Erros
________________________________________
- Residuais: diferença entre o valor real e o valor ajustado no modelo.
- Erro: diferença entre valor previsto e fato observado. Pode ser medido das seguintes formas: 1 - Aguardar o acontecimento. 2 - Separar dados de treino e teste. 3 - Criar modelo e comparar com os próprios dados 
- Métricas para avaliar erro:
- São importantes para avaliação do modelo.
- Pressupostos para avaliar: 1 - Residuos não devem estar autocorrelacionados. Caso exista, existe informação que deveria ser utilizada na previsão. 2 - A média deve ser próxima de zero. 3 - Variância deve ser constante. 4 - Dados devem ser distribuidos normalmente.
- Usar o Ljung-Box test para ver o p-value. Este precisa ser maior que 0.05 para ver que os residuos não estão autocorrelacionados.

## Decomposição
_________________________
- Definição: Processo de "separar" os componentes mencionados anteriormente.
- Razões: Compreensão e Previsão.
- Modelos principais: Aditivo e Multiplicativo








