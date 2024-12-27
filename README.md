# Insurance-Analysys-ML
 Projeto com o objetivo de prever valores referente ao valor de seguros médicos de pessoas.
# Insurance Analysis

Este repositório contém um notebook que realiza uma análise detalhada de um dataset do setor de seguros, utilizando ferramentas de análise exploratória de dados, visualização e modelagem preditiva. O objetivo é explorar padrões nos dados e desenvolver modelos preditivos para variáveis de interesse, como custos de seguro.

## Estrutura do Notebook

### 1. **Importação de Bibliotecas**
As bibliotecas utilizadas incluem:
- **Manipulação e processamento de dados:** `pandas`, `numpy`
- **Visualização:** `seaborn`, `matplotlib`
- **Modelagem e validação:** `sklearn`
- **Ferramentas adicionais:** `yellowbrick` (para análise de resíduos e previsões)

### 2. **Funções Auxiliares**
- **Função `get_metrics`:** Um dicionário para calcular métricas de avaliação de modelos, como R², MAE, MAPE e RMSE.

### 3. **Exploração do Dataset**
O dataset utilizado contém informações sobre:
- **age:** Idade do indivíduo.
- **sex:** Gênero (male ou female).
- **bmi:** Índice de Massa Corporal.
- **children:** Número de dependentes.
- **smoker:** Se o indivíduo é fumante (yes ou no).
- **region:** Região onde o indivíduo reside (southwest, southeast, northwest, northeast).
- **charges:** Custos médicos cobrados.

Análises incluem:
- Distribuições e correlações entre variáveis.
- Identificação de padrões relacionados aos custos médicos.
- Impacto do hábito de fumar nos custos.

### 4. **Pré-processamento**
- **Imputação de valores ausentes:** Substituição de dados faltantes usando `SimpleImputer`.
- **Normalização de dados:** Uso de `MinMaxScaler`.
- **Codificação de variáveis categóricas:** `OneHotEncoder`.

### 5. **Divisão de Dados**
- **Treinamento e teste:** Separar os dados para treinamento e validação dos modelos.

### 6. **Modelagem Preditiva**
Modelos utilizados:
- **DummyRegressor:** Baseline para comparação.
- **Regressão Linear:** Modelo linear simples.
- **Modelos Avançados:**
  - LassoCV
  - RidgeCV
  - Random Forest Regressor
  - Gradient Boosting Regressor

### 7. **Validação e Ajuste de Modelos**
- Uso de **GridSearchCV** para encontrar os melhores hiperparâmetros.
- Avaliação das previsões com métricas customizadas e visualização de resíduos.

### 8. **Visualização dos Resultados**
- Análise gráfica de previsões e resíduos usando o Yellowbrick.
- Comparativo entre diferentes modelos e suas métricas.

## Requisitos
Para executar o notebook, certifique-se de que as seguintes dependências estejam instaladas:
```bash
pip install numpy pandas seaborn matplotlib scikit-learn yellowbrick
```

## Como Utilizar
1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/insurance-analysis.git
```

2. Acesse o diretório do projeto:
```bash
cd insurance-analysis
```

3. Execute o notebook:
Utilize seu ambiente Jupyter favorito para abrir e executar o arquivo `insurance.ipynb`.

4. Substitua o arquivo CSV pelo seu conjunto de dados, se necessário.

## Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests com melhorias ou novos recursos.

## Licença
Este projeto está licenciado sob a [MIT License](LICENSE).



