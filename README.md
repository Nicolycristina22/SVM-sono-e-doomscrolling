# Doomscrolling e Qualidade do Sono: Classificação com SVM

Projeto acadêmico desenvolvido para analisar a relação entre hábitos de uso de telas, doomscrolling e qualidade do sono utilizando aprendizado de máquina supervisionado.

## Objetivo

Utilizar o algoritmo **Support Vector Machine (SVM)** para classificar a qualidade do sono com base em variáveis relacionadas aos hábitos de uso de telas e doomscrolling.

O projeto trabalha com duas tarefas de classificação:

- **Classificação binária (principal):** sono ruim (*Poor*) versus sono não ruim (*Good* e *Fair*).
- **Classificação em três classes (complementar):** *Good*, *Fair* e *Poor*.

## Base de dados

Foi utilizada a base **Sleep and Doomscrolling Habits**, disponibilizada no Kaggle, contendo 1.000 registros e 30 variáveis.

A base reúne informações relacionadas aos hábitos digitais e à qualidade do sono.

> Antes de disponibilizar o arquivo original da base neste repositório, verifique a licença e as condições de redistribuição definidas pelo responsável pela publicação no Kaggle.

## Metodologia

O desenvolvimento foi organizado nas seguintes etapas:

1. **Coleta dos dados:** obtenção e carregamento da base do Kaggle.
2. **Pré-processamento:** tratamento dos dados e preparação das variáveis para o modelo.
3. **Divisão dos dados:** separação entre conjuntos de treinamento e teste.
4. **Treinamento:** aplicação do algoritmo SVM para classificação.
5. **Avaliação:** análise do desempenho por meio de métricas, matriz de confusão e gráficos.

## Resultados

### Classificação binária — tarefa principal

Resultados obtidos no conjunto de teste:

| Métrica | Resultado |
|---|---:|
| Acurácia | 81,0% |
| AUC | 0,87 |
| Acurácia balanceada | 76,6% |
| Precisão para a classe *Poor* | 75,0% |
| Sensibilidade (*Recall*) para a classe *Poor* | 63,6% |
| F1-score para a classe *Poor* | 0,689 |

A validação cruzada apresentou acurácia média de **81,9%**.

### Classificação em três classes — análise complementar

Na classificação das categorias *Good*, *Fair* e *Poor*, a acurácia obtida foi de **59,0%**.

As duas tarefas são apresentadas separadamente porque representam problemas de classificação diferentes.

## Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- SciPy
- Statsmodels
- Jupyter Notebook
- Kaggle

## Estrutura do repositório

```text
.
├── notebook/        # Notebook de análise e modelagem
├── poster/           # Pôster do projeto
├── requirements.txt  # Dependências necessárias
└── README.md         # Documentação do projeto
```

Ajuste a estrutura conforme os nomes das pastas e arquivos enviados ao repositório.



## Considerações finais

O projeto demonstra a aplicação de aprendizado de máquina na classificação da qualidade do sono a partir de hábitos digitais.

Os resultados representam o desempenho do modelo na base de dados analisada e não comprovam, por si só, uma relação de causa e efeito entre o uso de telas, o doomscrolling e a qualidade do sono.

---

**Projeto acadêmico — Engenharia de Software | UMC**
