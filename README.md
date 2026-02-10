# Previsão de Inadimplência Bancária (Projeto em progresso)

![Status](https://img.shields.io/badge/Status-Em_Desenvolvimento-yellow)
![Python](https://img.shields.io/badge/Python-3.x-blue)
![Machine Learning](https://img.shields.io/badge/Focus-Credit_Risk-green)

## Sobre o Projeto

A inadimplência (default) é um dos maiores riscos para instituições financeiras. Este projeto visa desenvolver um modelo de **Machine Learning** capaz de prever a probabilidade de um cliente não honrar seus pagamentos, permitindo ações preventivas e melhor gestão de risco de crédito.

Atualmente, o projeto consiste em um **MVP (Minimum Viable Product)** focado na análise exploratória e modelagem inicial. O objetivo final é evoluir este notebook para uma solução **End-to-End** robusta, simulando um ambiente produtivo real.

## Metodologia

O projeto segue o fluxo do **CRISP-DM**, com ênfase rigorosa na análise estatística dos dados antes da modelagem:

1.  **Entendimento do Negócio:** Foco na redução de perdas financeiras.
2.  **Análise Exploratória (EDA):** Uso de testes de hipótese (Teste T de Student) e Intervalos de Confiança para validar a relevância das features.
3.  **Pré-processamento:** Limpeza de dados, tratamento de outliers e *One-Hot Encoding*.
4.  **Balanceamento:** Aplicação de técnicas de Oversampling (ROS) apenas nos dados de treino para evitar *data leakage*.
5.  **Modelagem:** Treinamento de algoritmos de classificação (Random Forest).

## Resultados Preliminares

No estágio atual (MVP), o modelo apresentou os seguintes resultados no conjunto de teste:

* **Acurácia:** ~93%
* **Recall (Classe 1 - Inadimplentes):** ~78%
    * *Nota: O foco principal é maximizar o Recall da classe positiva para minimizar o prejuízo financeiro com "falsos bons pagadores".*

## Roadmap de Evolução (Em Construção)

Este repositório é um projeto vivo. As próximas atualizações focarão na refatoração do código para padrões de Engenharia de Software e na construção do pipeline de dados.

- [x] **MVP:** Análise Exploratória, Testes Estatísticos e Modelo Base (Notebook).
- [ ] **Refatoração:** Otimização da ingestão de dados (Pandas nativo) e modularização do código (criação de scripts `.py`).
- [ ] **Ingestão de Dados:** Implementação de script para coleta automatizada.
- [ ] **Processamento:** Pipeline de transformação de dados (ETL).
- [ ] **Orquestração:** Automação do fluxo (ex: Airflow ou Prefect).
- [ ] **Deploy:** Disponibilização do modelo via API ou Container Docker.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python
* **Análise e Manipulação:** Pandas, NumPy
* **Estatística:** SciPy (Testes T, Intervalos de Confiança)
* **Visualização:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-learn (Random Forest, Metrics, Preprocessing)

## 🤝 Contribuições e Feedback

Sugestões e feedbacks são muito bem-vindos, especialmente relacionados a melhores práticas de MLOps e Engenharia de Dados. Sinta-se à vontade para abrir uma *issue* ou entrar em contato.

---
*Desenvolvido por Antonio Edson*