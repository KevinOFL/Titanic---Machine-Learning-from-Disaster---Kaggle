# 📘 Titanic Machine Learning from Disaster Kaggle
### **Pontuação:** 0.77751

Este repositório corresponde à minha resolução para o desafio do [Titanic - Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic/overview) no Kaggle, contém o desenvolvimento de modelo simples de Random Forest Classifier com SKlearn e enegenharia de feature para extrair a melhor pontuação.
---

## 📌 Sobre o Projeto

A solução é composta por um pipeline preditivo em desenvolvimento, destacando as seguintes entregas e tecnologias:

- **Limpeza e Engenharia de Features (Feature Engineering)**: Tratamento rigoroso de valores nulos e criação de novas variáveis lógicas a partir dos dados brutos. Destaca-se o agrupamento inteligente de idades em faixas demográficas (utilizando pd.cut do Pandas) para capturar as regras sociais de salvamento da época.

- **Treinamento e Otimização de Modelos**: Foram treinados modelos de classificação robustos, com foco na arquitetura Random Forest, utilizando o RandomizedSearchCV para a busca refinada de hiperparâmetros e tratamento de classes desbalanceadas.

- **Avaliação de Performance Realista**: Análise aprofundada do modelo indo além da acurácia. Foram utilizadas métricas de classificação corporativas como Precisão, Recall e F1-Score para mapear com exatidão o comportamento do algoritmo e mitigar o viés pessimista gerado pela desproporção histórica entre o número de vítimas e sobreviventes.

- **Pipeline de Inferência**: Estruturação de um fluxo limpo e reprodutível para o processamento dos dados de teste cegos. O sistema garante que os novos dados passem pelas mesmas transformações do ambiente de treinamento, exportando as predições finais no formato CSV exato exigido para a submissão na plataforma do Kaggle.

## ⚙️ Tecnologias Utilizadas

| Tecnologia | Função |
| :--- | :--- |
| **Scikit-Learn** | Ferramentas de pré-processamento, métricas e treinamento de modelos baseline (*Random Forest*). |
| **Pandas / NumPy** | Manipulação, limpeza e análise matemática estruturada dos dados tabulares da ONG. |

## 🚀 Como Executar Localmente

### 📦 Pré-requisitos

Certifique-se de ter as seguintes ferramentas instaladas no seu sistema:

* [Python 3.13+](https://www.python.org/downloads/)

### 🔧 Passo a Passo (Setup)

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/KevinOFL/DATATHON_Magic_Steps_FIAP.git](https://github.com/KevinOFL/Titanic---Machine-Learning-from-Disaster---Kaggle.git)
   cd SEU_REPOSITORIO
   ```
2. **Instale as depedências:**
   ```bash
   pip install -r requirements.txt
   ```
3. **Execute o notebook Jupyter**

## 📌 Boas Práticas Aplicadas e Arquitetura MLOps

- **Engenharia de Features Robusta**: Criação de variáveis analíticas de discrepância de notas e indicadores (INDE, IEG) e tratamento dinâmico de nulos (imputação por mediana) para maximizar o poder preditivo.
- **Modularização do Pipeline**: Funções de pré-processamento estritamente reutilizáveis, garantindo que os dados de inferência passem pelas exatas mesmas transformações dos dados de treino..
---

## 👥 Contribuição

Pull requests são bem-vindos! Abra uma issue ou contribua diretamente via fork + PR.

---

## 📃 Licença

Este projeto está licenciado sob os termos da licença [MIT](LICENSE).
