# Prompts

A versão gratuita do ChatGPT na data dessa entrega(25/01/2025) só permite o upload de um arquivo por dia.
Dessa forma, utilizei a Perplexity Ai, que utiliza o ChatGPT, mas oferece um limite maior de uploads de arquivo

## Descrevendo os dados

Primeiramente  foi solicitado que a IA descrevesse a base e identicasse eventuais sazonalidades, utilizando o prompt abaixo:
```
Faça uma análise descritiva dos dados agrupando por país e prevendo possíveis sazonalidades.
```
Além de gerar uma tabela de resumo , foram gerados alguns insights.

### Resumo
|País|Total de Vendas (Quantidade)|Total em Moeda Original|
|-----|-----|----|
|Australia|	30|	2,300|
|UK|25|	1,800|
|Canada|20|1,500|
|Germany|22|1,600|
|France|18|1,400|
|Japan|10|800|
|USA|15|1,200|

### Sazonalidade
Para prever sazonalidades, analisamos os dados ao longo do tempo. Observamos que:
Picos de Vendas: Os meses de agosto e setembro mostraram um aumento significativo nas vendas, possivelmente devido a promoções ou lançamentos de novos produtos.
Queda nas Vendas: Os meses de janeiro e fevereiro apresentaram uma queda nas vendas, o que pode estar relacionado a um período pós-festas ou férias.
Gráfico de Vendas Mensais
Um gráfico (não apresentado aqui) pode ser gerado para visualizar as vendas mensais ao longo do ano. Espera-se que os picos sejam visíveis nos meses mencionados anteriormente.
### Previsão
Com base nos padrões observados:
Expectativa de Crescimento: Se a tendência continuar, espera-se que as vendas aumentem nos próximos meses antes das festividades de fim de ano.
Promoções: A implementação de campanhas promocionais durante os meses com menor volume pode ajudar a equilibrar as vendas ao longo do ano.

## Agrupando os dados

Por ultimo foi solicitado uma tabela resumo com o valor da venda em reais e a porcentagem de desconto.

Prompt 

```
gere uma tabela de vendas por pais . Contudo converta o valor total de vendas  para reais utilizando a cotação de fechamento de 24/01/2025.
use as  cotações abaixo :
1GPB = 7.38 BRL
1USD = 5.92BRL
1EUR = 6.20BRL
Agrupe os dados por país . Inclua o desconto das vendas também em reais e calcula o percentual de desconto aplicado em reais
```

| País      | Total Vendas (Moeda Original) | Total Desconto (Moeda Original) | Total Vendas (BRL) | Total Desconto (BRL) | Percentual de Desconto (%) |
|-----------|-------------------------------|----------------------------------|---------------------|-----------------------|-----------------------------|
| Australia | 2,080 GBP                     | 52.47 GBP                        | 15,358.40           | 386.95                | 2.51                        |
| Australia | 1,100 USD                     | 6.71 USD                        | 6,512.00            | 39.67                 | 0.61                        |
| UK        | 1,340 GBP                     | 78.12 GBP                       | 9,867.20            | 576.03                | 5.83                        |
| Germany   | 1,060 USD                     | 46.51 USD                       | 6,267.20            | 275.33                | 4.39                        |
| Germany   | 280 EUR                       | 9.66 EUR                        | 1,736.00            | 59.91                 | 3.44                        |
| Canada    | 1,380 GBP                     | 42.13 GBP                       | 10,193.40           | 310.87                | 3.05                        |
| USA       | 1,020 EUR                     | 36.51 EUR                       | 6,324.00            | 226.93                | 3.58                        |
| Japan     | 500 EUR                       | -                                | 3,100.00            | -                     | -                           |
| France    | 1,360 USD                     | -                                | 8,059.20            | -                     | -                           |

nota: o código markedwn também foi gerado por ia com o prompt abaixo

```
gere o código Markdon da tabela acima
```