### Santander Coders 2023 - 2024 | 2º semestre - DS (Turma #1114)

### **Grupo:** Demetrio Martins, Gabriel Lopes, Gabriela Milagres, Miller Machado, Suzielli Mendonça

### **Projeto**  
Machine Learning II   
Projeto Final de Machine Learning

### **Sobre o conjunto de dados:**    
Escolhemos um conjunto de dados sintético sobre estratégias de campanha de Marketing. O conjunto de dados data de 2014 e consta com as seguintes informações :
- **AcceptedCmp1** - 1 se o cliente aceitou a oferta na 1ª campanha, 0 caso contrário
- **AcceptedCmp2** - 1 se o cliente aceitou a oferta na 2ª campanha, 0 caso contrário
- **AcceptedCmp3** - 1 se o cliente aceitou a oferta na 3ª campanha, 0 caso contrário
- **AcceptedCmp4** - 1 se o cliente aceitou a oferta na 4ª campanha, 0 caso contrário
- **AcceptedCmp5** - 1 se o cliente aceitou a oferta na 5ª campanha, 0 caso contrário
- **Response (target original)** - 1 se o cliente aceitou a oferta na última campanha, 0 caso contrário
- **Complain** - 1 se o cliente reclamou nos últimos 2 anos
- **DtCustomer** - data de inscrição do cliente na empresa
- **Education** - nível de educação do cliente
- **Marital** - estado civil do cliente
- **Kidhome** - número de crianças pequenas no domicílio do cliente
- **Teenhome** - número de adolescentes no domicílio do cliente
- **Income** - renda anual do domicílio do cliente
- **MntFishProducts** - valor gasto em produtos de peixe nos últimos 2 anos
- **MntMeatProducts** - valor gasto em produtos de carne nos últimos 2 anos
- **MntFruits** - valor gasto em produtos de frutas nos últimos 2 anos
- **MntSweetProducts** - valor gasto em produtos doces nos últimos 2 anos
- **MntWines** - valor gasto em produtos de vinho nos últimos 2 anos
- **MntGoldProds** - valor gasto em produtos de marca *premium* nos últimos 2 anos
- **NumDealsPurchases** - número de compras feitas com desconto
- **NumCatalogPurchases** - número de compras feitas usando catálogo
- **NumStorePurchases** - número de compras feitas diretamente em lojas
- **NumWebPurchases** - número de compras feitas através do site da empresa
- **NumWebVisitsMonth** - número de visitas ao site da empresa no último mês
- **Recency** - número de dias desde a última compra

### **Objetivo Geral:** 
Fazer uma análise completa do perfil dos clientes do conjunto de dados. A análise se dá em três partes:
- Análise Exploratória de Dados
- Análise de Segmentação
- Análise Preditiva

### **Objetivos Específicos:**
- Utilizar métodos de *Aprendizado de Máquina não Supervisionados* para agrupamento e segmentação inicial de clientes;
- Prever se um dado cliente irá ou não aceitar alguma campanha de marketing da empresa baseado no seu perfil utilizando métodos de *Aprendizado de Máquina Supervisionados*;
- Comparar resultados da previsão de aceite de campanha nas seguintes situações:
    - com o conjunto de dados original
    - adicionando uma nova coluna *clusters* ao conjunto de dados inicial, a partir da clusterização feita com os métodos Aprendizado de Máquina não Supervisionados

### **Metodologia:**
- Análise exploratória de dados
    - Verificação e tratamento de dados faltantes
    - Verificação e tratamento de *outliers*
    - Engenharia de *features*
    - Tratamento de dados numéricos e categóricos
    - Verificação da distribuição dos dados de colunas de interesse
    - Verificação de correlações
    - Análise univariada de perfil de clientes 
    - Análise bivariada de perfil de clientes
- Aprendizado de Máquina não Supervisionado:
    - [KMeans](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html)
    - [AgglomerativeClustering](https://scikit-learn.org/stable/modules/generated/sklearn.cluster.AgglomerativeClustering.html)
- Aprendizado de Máquina Supervisionado:
    - [GradientBoostingClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingClassifier.html)
    - Métrica de avaliação do teste: acurácia e f1-score

---
**Fim do projeto**
