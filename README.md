# Análise da Relação entre Renda Per Capita, Altura dos Atletas e Desempenho Olímpico

## Sumário

Este projeto explora a complexa relação entre fatores socioeconômicos (como a renda per capita de um país) e características físicas dos atletas (como a altura) com o desempenho olímpico, medido pelo número de medalhas conquistadas. A análise utiliza dados históricos de atletas e nações olímpicas para identificar tendências e correlações significativas ao longo do tempo.

## Objetivo do Estudo

*   Investigar a influência da renda per capita dos países no número de medalhas olímpicas.
*   Avaliar a correlação entre a altura dos atletas e o seu desempenho em Jogos Olímpicos, especificamente na conquista de medalhas.
*   Identificar padrões e tendências históricas no desempenho olímpico em relação aos fatores analisados.

## Fontes de Dados

Foram utilizadas duas bases de dados principais para esta análise:

1.  **Base de Performance Olímpica:** Contém dados de altura e peso de atletas, bem como informações sobre suas participações e medalhas em diversas edições dos Jogos Olímpicos.
2.  **Base de GPD (Produto Interno Bruto) das Nações:** Inclui dados de renda per capita dos países, provenientes de fontes reconhecidas.

## Qualidade e Pré-processamento dos Dados

Para garantir a precisão e relevância da análise, foram realizados os seguintes passos de pré-processamento e tratamento de dados:

### Base de Performance Olímpica

*   **Preenchimento:** A base apresenta bom preenchimento de dados de altura e peso a partir de 1988.
*   **Anos com Falhas:** A edição de 1996 e dados de Jogos Olímpicos de Inverno foram excluídos devido a falhas significativas de preenchimento e para evitar viés na análise.

### Base de GPD das Nações

*   **Dados Nulos:** Informações nulas (especialmente na referência de 2023) foram identificadas e tratadas devido a problemas de preenchimento.
*   **Exclusão de Dados Errados:** Dados do Afeganistão e Paquistão foram removidos devido ao preenchimento incorreto das colunas.

## Análise e Principais Conclusões

A análise revelou insights importantes sobre os fatores que influenciam o desempenho olímpico:

### 1. Relação entre Tamanho dos Atletas e Desempenho Olímpico

*   **Correlação Positiva:** Há uma correlação positiva entre a altura dos atletas e o desempenho em medalhas, observada desde 1988.
*   **Aumento da Altura Média:** A média de altura tanto para atletas masculinos quanto femininos aumentou significativamente ao longo do tempo, refletindo também um aumento nas conquistas de medalhas.
    *   **Atletas Femininas:** Altura média aumentou de 1,652 m (1988) para 1,665 m (2016), um incremento de 0,8%. A proporção de medalhistas femininas na faixa de 1,71m a 1,80m passou de 27% (1988) para 70% (2016).
    *   **Atletas Masculinos:** Altura média aumentou de 1,756 m (1988) para 1,780 m (2016), um incremento de 1,4%.
*   **Conclusão:** A altura pode ser um fator relevante para o desempenho olímpico, sugerindo que características físicas influenciam os resultados, além de treinamento e dedicação.

### 2. Influência da Renda per Capita no Desempenho Olímpico

*   **Ausência de Correlação Direta:** Não há uma correlação direta entre o aumento da renda per capita e o número de medalhas *conquistadas por país*. No entanto, países com maior renda per capita tendem a ter uma representação crescente nas competições.
*   **Exemplo dos EUA:** Apesar de um aumento de 34% no PIB de 1988 a 2016, os EUA registraram apenas 14% de aumento em medalhas, sugerindo uma possível estagnação na eficiência em transformar riqueza em medalhas.
*   **Disparidade Crescente:** Nações com alta renda, especialmente após 1992, começaram a dominar a distribuição de medalhas, indicando uma crescente disparidade entre os 10% mais ricos e os demais países.

### 3. Diferença no Tamanho dos Atletas entre Países com Diferentes Níveis de Renda

*   Países com maior renda per capita tendem a ter atletas mais altos.
*   **Fatores Socioeconômicos:** Isso sugere que melhores condições de saúde, nutrição e treinamento, influenciadas por fatores socioeconômicos, contribuem para o desenvolvimento físico dos atletas.

### 4. Tendência Histórica do Desempenho Olímpico em Relação à Renda per Capita

*   A distância nas conquistas olímpicas entre países ricos e os demais tem aumentado.
*   O sucesso olímpico continua a ser dominado por nações economicamente favorecidas.

## Pontos Fortes da Análise

*   **Coleta de Dados:** Utilização de fontes confiáveis (base Olympics e dados de PIB reconhecidos).
*   **Tratamento de Dados:** Exclusão eficaz de dados com falhas para garantir precisão.
*   **Identificação de Tendências:** Sucesso na identificação de correlações importantes e disparidades.

## Áreas de Melhoria e Próximos Passos

A análise realizada fornece uma base sólida, mas existem áreas para aprofundamento e refinamento:

1.  **Ajuste do GPD à Inflação:** A falta de ajuste do PIB per capita à inflação pode introduzir viés. Ajustar os dados para a inflação (ex: usando o valor do dólar como referência) proporcionaria uma perspectiva mais acurada das mudanças econômicas ao longo do tempo e sua influência no desempenho olímpico.
2.  **Impacto de Esportes Coletivos:** Esportes coletivos podem inflar desproporcionalmente o número de medalhas de um país. Seria benéfico desenvolver uma metodologia para considerar a proporção de medalhas individuais em relação às coletivas, oferecendo uma avaliação mais justa do desempenho dos países.

## Conclusão Final

Este estudo revela que, enquanto características físicas como a altura ainda desempenham um papel significativo no sucesso esportivo, a renda per capita e os fatores socioeconômicos associados destacam uma profunda desigualdade de oportunidades. Atletas de países mais ricos tendem a ter acesso a melhores recursos e treinamentos, o que limita o desempenho de nações de renda média ou baixa.

Para um esporte mais justo e inclusivo, é fundamental que políticas esportivas e investimentos em treinamento sejam reavaliados para garantir que talentos de todas as origens tenham a chance de competir em igualdade de condições nos Jogos Olímpicos. A continuidade desta pesquisa, incorporando as melhorias propostas, pode fornecer insights ainda mais profundos e fundamentados sobre as dinâmicas complexas que moldam o desempenho olímpico.

https://dbc-510e01d2-ae74.cloud.databricks.com/sql/dashboardsv3/01f0ddc3fa7710c790ccda195579f43a?o=7474659419639021 - Dash com info de medalhas por GPD e Altura
https://dbc-510e01d2-ae74.cloud.databricks.com/sql/dashboardsv3/01f0ddc5b00316cca97d3a10e54197d7/pages/bb689302?o=7474659419639021
