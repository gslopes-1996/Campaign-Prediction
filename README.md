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

### **Conclusão do Projeto:**
Este projeto visou a identificação de perfis de clientes utilizando dados de 2014, com o objetivo de melhorar a performance de modelos preditivos em campanhas de marketing. Foram utilizados dois métodos de modelagem: aprendizado de máquina não supervisionado (para identificar grupos de clientes com comportamentos semelhantes) e aprendizado de máquina supervisionado, para prever a aceitação de ofertas de campanhas.    

**Conclusões:**

- Identificação de Perfis de Clientes:
    - Utilizando dados de campanhas anteriores e características dos clientes, identificamos três grandes perfis de clientes. Isso foi alcançado através de técnicas de aprendizado de máquina não supervisionado (clusterização).

- Melhoria da Performance do Modelo:
    - A inclusão da coluna 'cluster', derivada da clusterização, no modelo preditivo supervisionado resultou em um pequeno aumento em todas as métricas de performance.

- Métricas de Performance:
    - Precisão (Precision): Aumentou de 0.86 para 0.88.
    - Recall: Aumentou de 0.96 para 0.97.
    - F1-score: Aumentou de 0.91 para 0.92.
    - Acurácia: Aumentou de 0.85 para 0.87.

Esses resultados demonstram que a segmentação dos clientes em clusters antes da aplicação do modelo preditivo supervisionado pode fornecer informações de modo a contribuir para a melhoria da eficácia das campanhas de marketing.

---
**Fim do projeto**
