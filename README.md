# 🧠 Comitê de Classificadores - Previsão de Terapia

## 📌 Sobre o Projeto

Este projeto foi desenvolvido no contexto da disciplina **Inteligência Artificial** e tem como objetivo explorar diferentes modelos de aprendizado de máquina aplicados à área da saúde mental.

A proposta foi utilizar a base de dados **Mental Health Diagnosis and Treatment Monitoring** (Kaggle) para prever **qual tipo de terapia seria mais adequada** para cada paciente, considerando seu diagnóstico, idade, histórico de medicação e evolução clínica.

O trabalho envolveu desde a análise e transformação dos dados até a criação de variáveis derivadas, permitindo observar o impacto do pré-processamento na qualidade dos resultados. Foram aplicados diferentes classificadores da biblioteca **Scikit-learn**, com análises comparativas de desempenho.

---

## 🔬 Etapas do Projeto
1. **Limpeza de dados** → remoção de colunas irrelevantes
2. **Análise exploratória** → estatísticas e correlações
3. **Transformação de variáveis** → conversão de texto para IDs categóricos
4. **Testes iniciais** → baixa acurácia nos modelos crus
5. **Feature Engineering** → criação de variáveis derivadas:
   - Agrupamento por idade (`AgeGroupId`)
   - Taxa de melhora por terapia (`ImprovedRate`)
   - Score ponderado por número de pacientes (`ByTherapyScore`)
6. **Treino final** → uso apenas das variáveis derivadas
7. **Resultados** → melhoria significativa na acurácia;
   - Melhor modelo: **Árvore de Decisão** (bom equilíbrio entre desempenho, eficiência e interpretação).

---

## 📊 Resultados

Os testes iniciais com os dados brutos mostraram **acurácia insatisfatória** nos classificadores, independentemente do algoritmo utilizado. Após a criação de variáveis derivadas, os resultados melhoraram substancialmente, evidenciando o impacto do pré-processamento.

Entre os modelos aplicados (**Naive Bayes, Decision Tree, SVM, KNN e Rede Neural**), o que apresentou o melhor desempenho foi a **Árvore de Decisão**, com resultados consistentes, rapidez no treinamento e facilidade de interpretação visual.
