Este é o modelo definitivo de README.md para o seu repositório no GitHub ou para a célula de abertura do seu notebook. Ele foi estruturado para demonstrar não apenas o código, mas o seu raciocínio analítico e a capacidade de gerar valor de negócio.

📡 Telecom X: Previsão de Evasão de Clientes (Churn Prediction)
📋 Visão Geral do Projeto
Este projeto aborda um dos problemas mais críticos para empresas de serviços: a evasão de clientes (Churn). Utilizando dados da Telecom X, desenvolvemos um pipeline completo de Ciência de Dados para identificar padrões de comportamento e construir modelos preditivos capazes de antecipar quais clientes têm maior probabilidade de cancelar seus serviços.

🛠️ Pipeline de Desenvolvimento
1. Engenharia e Limpeza de Dados
Ingestão: Consumo de dados via API JSON e normalização de estruturas aninhadas.

Saneamento: Tratamento de valores nulos em faturas totais e correção de tipos de dados.

Feature Selection: Remoção de identificadores únicos (customerID) para evitar ruído nos modelos.

2. Preparação para Machine Learning
Encoding: Transformação de variáveis categóricas (Contratos, Serviços, Pagamentos) em dados numéricos via One-Hot Encoding.

Escalonamento: Aplicação de StandardScaler para normalizar as grandezas financeiras.

Balanceamento (SMOTE): Tratamento do desequilíbrio de classes (73% ativos vs 26% evasão) através da geração de dados sintéticos da classe minoritária.

3. Modelagem e Avaliação
Comparamos dois modelos com abordagens distintas:

Regressão Logística: Focada em interpretabilidade e probabilidade linear.

Random Forest: Focada em capturar relações não-lineares complexas.

Métricas utilizadas: Acurácia, Precisão, F1-Score e, principalmente, Recall (essencial para capturar o maior número possível de evasões reais).

📈 Principais Descobertas (Insights de Negócio)
O Gatilho do Churn: Clientes com contratos Mês a Mês são os mais propensos a sair.

Risco Tecnológico: Usuários de Fibra Óptica possuem taxa de evasão superior à de DSL, indicando problemas de custo ou qualidade técnica.

Âncora de Retenção: O Suporte Técnico e o Tempo de Casa (Tenure) são os fatores que mais protegem a base de clientes.
