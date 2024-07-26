# Relatório de Análise de Dados de Preços de Aluguel de Veículos

## Introdução
Este repositório contém um relatório de análise de um conjunto de dados fornecido por uma empresa de aluguel de veículos. O objetivo do estudo é explorar as variáveis que influenciam os preços de aluguel e examinar as relações entre essas variáveis e o preço do aluguel. A análise foi conduzida utilizando técnicas estatísticas e de regressão linear e quadrática.

## Conjunto de Dados
O conjunto de dados consiste em 20 observações aleatórias de locações de veículos com as seguintes variáveis:
- **Preço**: Valor do aluguel em Reais (R$)
- **Portas**: Número de portas (duas ou quatro)
- **Ar Condicionado**: Presença de ar condicionado (com ou sem ar condicionado)
- **Quadrimestre**: Quadrimestre do ano em que a locação ocorreu (primeiro, segundo ou terceiro quadrimestre)
- **Idade do Locatário**: Idade do locatário em anos
- **Quilometragem**: Quilometragem do veículo no momento da locação

## Análise do Preço
1. **Histograma do Preço**
   - O histograma mostra a distribuição dos preços de aluguel, destacando a concentração em diferentes intervalos de preço.
   
2. **Boxplot do Preço**
   - O boxplot visualiza a dispersão e possíveis outliers nos preços de aluguel, permitindo uma análise rápida da variabilidade dos preços.
   
3. **Estatísticas Descritivas do Preço**
   - Média: R$ 440,7
   - Desvio Padrão: R$ 51,1
   - Mínimo: R$ 339,5
   - Primeiro Quartil: R$ 415,8
   - Mediana: R$ 447,8
   - Terceiro Quartil: R$ 463,5
   - Máximo: R$ 551,3

## Relação entre Preço e Quadrimestre
4. **Boxplot entre Preço e Quadrimestre**
   - O boxplot visualiza a relação entre o preço e o quadrimestre.
   
5. **Análise de Variância (ANOVA)**
   - **Objetivo**: Avaliar se os preços dos carros variam significativamente entre diferentes quadrimestres do ano.
   - **Conclusão**: Existe uma diferença significativa entre o preço médio de pelo menos um quadrimestre em relação aos outros, pois o p-valor é 0,000126, menor que o nível de significância de 0,05. Portanto, rejeitamos a hipótese nula de que os preços médios são iguais entre os quadrimestres.
   - **Resumo**: A análise indica que os preços dos carros variam significativamente entre os quadrimestres do ano. Isso sugere que fatores sazonais podem estar influenciando os preços.

## Relação entre Preço e Portas
6. **Boxplot entre Preço e Portas**
   - O boxplot visualiza a relação entre o preço e o número de portas.
   
7. **Teste t de Student**
   - **Objetivo**: Avaliar se os preços dos carros variam significativamente entre diferentes categorias de quantidade de portas.
   - **Conclusão**: Não há diferença significativa entre os preços de veículos com duas portas e quatro portas (Statistic: -0.142, p-valor: 0.888). Isso sugere que o número de portas não é um fator determinante no preço do aluguel.

## Relação entre Preço e Quilometragem
8. **Gráfico de Dispersão entre Preço e Quilometragem**
   - O gráfico de dispersão mostra a relação entre preço e quilometragem.
   
9. **Coeficiente de Correlação**
   - A correlação entre preço e quilometragem é de -0.823, indicando uma forte correlação negativa. Isso significa que, à medida que a quilometragem do veículo aumenta, o preço do aluguel tende a diminuir significativamente.
   
10. **Regressão Linear entre Preço e Quilometragem**
    - 67.8% da variação no preço pode ser explicada pela quilometragem (R²: 0.678). Isso indica que a quilometragem é uma variável preditora significativa e explica uma grande parte da variação observada no preço do aluguel dos veículos. O restante da variação (32.2%) pode ser atribuída a outros fatores não incluídos neste modelo simples.

## Conclusão
Este estudo revelou que a quilometragem do veículo tem uma influência significativa nos preços de aluguel, enquanto a cotação do dólar e o número de portas não apresentam impacto significativo. A análise de variância indicou que há uma diferença significativa no preço médio entre os diferentes quadrimestres do ano.

**Recomendações**:
- Considerar a quilometragem do veículo como um fator importante na determinação dos preços de aluguel, possivelmente implementando uma política de preços baseada na quilometragem.
- Monitorar e ajustar os preços de aluguel de acordo com os quadrimestres do ano para aproveitar as variações sazonais e maximizar as receitas.
- Continuar a coletar dados para aumentar o tamanho da amostra e melhorar a precisão das análises futuras.



## Autor
[Vinicius Farineli]

## Licença
Este projeto é licenciado sob a Licença MIT - veja o arquivo LICENSE para mais detalhes.
