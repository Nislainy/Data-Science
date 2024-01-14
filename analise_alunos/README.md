# **Análise Dados - Alunos**

# **Sobre o Projeto**

Projeto desenvolvido juntamente com o curso que conclui, porém, as análises foram realizadas através da minha visão analítica. 

Nesse projeto, foram analisados:

1. Importação de bibliotecas: pandas, numpy, matplotlib e seaborn.
2. Leitura de arquivo csv.
3. DataFrame.
4. Visualização de linhas iniciais e finais.
5. Verificação da quantidade de linhas e colunas de um DataFrame;
6. Conferência dos tipos de dados de cada DF.
7. Selecionar uma ou múltiplas colunas.
8. Ordenar valores de um DataFrame com o sort_values.

Aqui foram geradas algumas informações para termos conhecimento de como está a nossa base de dados e, para aprofundarmos nessas informações, realizei os seguintes processos: 

1. Identifiquei os valores NaN.
2. Utilizei o método describe para trazer um resumo dos dados.
3. Realizei algumas mudanças no DF, como as mudanças no nome de colunas e dados relacionados a linhas.

Optei por calcular a **média**, **moda**, **mediana** e **desvio padrão** para analisar os valores e identificar a melhor solução para tratar os valores NaN.

> Moda: 7.0.

> Média das notas é: 6.8.

> Mediana das notas: 7.0.

> STD: 2.204953.

Para a correção dos valores NaN, utilizei da seguinte análise:

- **Moda**: é o valor que mais se repete, se trata de valores categóricos, porém, os valores se diferem mais uns dos outros.
- **Média**: os dados são distribuídos aproximadamente simétricos, segundo os dados existem muitas variações, alguns valores sendo muito altos e outros baixos, o que nessa base de dados não fez diferença, mas em outra base de dados, a média poderia interferir na análise.
- **Mediana**: utilizaria a mediana se tivéssemos outliers - valores muito distantes dos outros, ou que mediante pesquisas identificássemos que é um valor impossível de ocorrer. Porém, o valor é exatamente igual à moda, significando que os dados estão distribuídos aproximadamente simétrica, fornecendo uma estimativa central semelhante aos dados.
- **Desvio Padrão**: o resultado foi um valor baixo, o que indica que os valores podem estar mais próximos da média com menor variabilidade.

Não considerei tratar os valores NaN como 0 / ou realizando a retirada desses alunos, pois não achei viável e por isso considerei os valores NaN, com o resultado da mediana. 

Nesta base de dados utilizada, todos os resultados estão próximos e não iriam ter um impacto muito diferente se utilizássemos as substituições por outros cálculos. 

Como analista, identifiquei que, mesmo realizando a substituição das notas pela mediana, alguns alunos não atingiram a nota mínima: 7.0 e mesmo assim estavam com a condição de aprovados. Os alunos com notas acima de 7.0 constavam como reprovados. 
Todos os valores identificados como: NaN estão como reprovados, porém, com as novas atualizações, foram realizadas as devidas correções. 

Após isso, aprofundei em minhas análises, e aprendi:

1. Identificar o que fazer durante um processo de análise exploratória.
2. Fazer seleções utilizando o método query.
3. Visualizar valores únicos com o unique.
4. Remover de alunos.
5. Remoção de colunas.

E, como realizamos as substituições das notas para os dados que continuam informações como: NaN, resolvi calcular a média, moda, mediana e o std novamente para verificar as diferenças entre um e outro. A média, moda e a média obtiveram como resultados o valor: 7.0 e o STD permanece baixo, indicando uma menor dispersão.

Para melhores análises, identifiquei:

1. A idade médias dos alunos aprovados e reprovados.
2. Calcular percentuais dos alunos aprovados e reprovados.
3. Plotar gráfico de pizza, com as devidas informações.
4. Salvar dados no formato csv.

Para encerrar as minhas análises, realizei algumas correções solicitadas, como:

1. Alteração das notas com valores 7.0 para 8.0.
2. Ajustes de notas extras para mais 40% baseado na nota atual.
3. Método describe, moda.

Utilizei o describe como base de comparação nas informações com todas as alterações realizadas, porém mesmo com todas essas mudanças os cálculos permanecem viáveis. Concluindo, utilizar a mediana como substituição dos dados NaN foi uma excelente opção. 
