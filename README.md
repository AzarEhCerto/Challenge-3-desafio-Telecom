# 📊 Telecom X - Análise de Evasão de Clientes

## 📖 Descrição do Projeto
Este projeto faz parte de um desafio da **Alura** em que você atua como **assistente de análise de dados** na empresa fictícia **Telecom X**.  

O objetivo é entender os fatores que levam os clientes a cancelar o serviço (**Churn**) e propor estratégias de retenção baseadas em análise de dados.  

---

## 🛠️ Tecnologias Utilizadas
- Python  
- Pandas  
- Numpy  
- Matplotlib / Seaborn  
- Scikit-learn  
- Jupyter Notebook  

---

## 📈 Análise e Resultados

### 🔹 1. Desempenho e Escolha do Modelo
- Foram testados dois modelos: **Regressão Logística** e **Random Forest**.  
- Após a remoção de variáveis redundantes e tratamento da multicolinearidade:  
  - O **Random Forest** apresentou melhor equilíbrio entre métricas.  
  - Seu **Recall** (capacidade de identificar quem realmente evadiu) se destacou, tornando-o o modelo preferencial.  

---

### 🔹 2. Principais Fatores de Evasão
Com base na **importância das variáveis do Random Forest**, os fatores mais relevantes para o churn foram:  
- **Tempo de Contrato (customer_tenure):** clientes recentes são os mais propensos a sair.  
- **Cobrança Mensal (account_charges_monthly):** valores altos aumentam fortemente o risco de churn.  
- **Tipo de Contrato (Mês a Mês):** ausência de vínculo de longo prazo aumenta a evasão.  
- **Método de Pagamento (Cheque Eletrônico):** indicador de maior risco.  
- **Serviço de Internet Fibra Ótica:** apesar de premium, apresentou taxa elevada de evasão.  

---

### 🔹 3. Recomendações Estratégicas
Com base nos resultados do modelo, as recomendações para a **Telecom X** são:  
- **Contratos Mensais:** migrar clientes para planos anuais com incentivos (descontos ou upgrades).  
- **Novos Clientes:** criar programa de boas-vindas (primeiros 3–6 meses) com suporte proativo e pesquisa de satisfação.  
- **Fibra Ótica:** investigar causas da evasão nesse serviço (preço, instabilidade, atendimento).  
- **Meio de Pagamento:** incentivar a troca do **cheque eletrônico** por débito automático ou cartão com descontos únicos.  

---

## 🚀 Como Executar o Projeto
1. Clone este repositório:  
   ```bash
   git clone https://github.com/AzarEhCerto/Challenge-3-desafio-Telecom.git
