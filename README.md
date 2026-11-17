# Classificação de Categoria de Acesso — Árvore de Decisão

## Sobre o projeto

Este projeto utiliza técnicas de **Machine Learning** para desenvolver um modelo de classificação capaz de prever a categoria de acesso dos comensais dos Restaurantes Universitários (RUs) da Universidade Federal do Ceará (UFC).

O modelo utiliza o algoritmo **Árvore de Decisão (Decision Tree)**, considerando informações sobre o vínculo do comensal, o tipo de refeição e a quantidade de refeições registradas.

O desenvolvimento foi realizado no **Google Colab**, utilizando Python e bibliotecas de análise de dados e aprendizado de máquina.

## Tecnologias e bibliotecas

- Python
- Google Colab
- Pandas
- Scikit-learn
- Matplotlib

## Dataset

Os dados utilizados são provenientes do arquivo:

[17_prae_comensais_2024.csv](https://github.com/bhpp12/datasets/blob/main/17_prae_comensais_2024.csv)

O dataset contém registros relacionados às refeições dos comensais dos Restaurantes Universitários.

### Variáveis utilizadas

| Variável | Descrição |
|---|---|
| `vinculo_comensal` | Vínculo do usuário com a universidade. |
| `tipo_refeicao` | Tipo de refeição realizada. |
| `quantidade_refeicao` | Quantidade de refeições registradas. |
| `categoria_acesso` | Variável-alvo que o modelo busca prever. |

## Desenvolvimento

O notebook contempla as seguintes etapas:

1. **Carregamento dos dados:** importação do dataset diretamente do GitHub utilizando Pandas.
2. **Limpeza dos dados:** remoção de registros com mais de 1.000 refeições para reduzir a influência de valores extremos.
3. **Definição das variáveis:** seleção das features e da variável-alvo.
4. **Pré-processamento:** aplicação de One-Hot Encoding nas variáveis categóricas.
5. **Divisão dos dados:** separação em conjuntos de treinamento (80%) e teste (20%).
6. **Treinamento:** construção de um modelo de Árvore de Decisão com profundidade máxima igual a 5.
7. **Previsão:** classificação dos registros do conjunto de teste.
8. **Avaliação:** análise da acurácia, precisão, recall e F1-score.
9. **Visualização:** representação gráfica da árvore de decisão utilizando Matplotlib e Scikit-learn.

## Avaliação do modelo

O desempenho do modelo é analisado por meio de:

- **Accuracy:** percentual de previsões corretas.
- **Precision:** proporção de previsões corretas entre as classificações realizadas para cada classe.
- **Recall:** capacidade de identificar corretamente os registros de cada classe.
- **F1-Score:** equilíbrio entre precisão e recall.

Os resultados são exibidos diretamente no notebook do Google Colab.

## Execução

O projeto pode ser executado diretamente no Google Colab, sem necessidade de configuração de ambiente local.

As bibliotecas utilizadas podem ser importadas no próprio notebook, e o dataset é carregado automaticamente por meio de sua URL no GitHub.

## Autor

**Bruno Henrique Pacheco Prudêncio**

Estudante de Ciência de Dados — Universidade Federal do Ceará (UFC).

[GitHub](https://github.com/bhpp12)
