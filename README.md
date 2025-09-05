# Atividade 3 – Ciência de Dados  

Este repositório contém a solução da **Atividade 3** da disciplina de **Ciência de Dados (Engenharia de Software)**.  

## 📂 Conteúdo  
- **Atividade3.ipynb** → Notebook Jupyter com todo o código e explicações.  
- **base_limpa.csv** → Base de dados já tratada e pronta para análises.  

## ⚙️ Etapas realizadas  

### 🔹 Leitura e inspeção  
- Corrigido problema de formatação (dados vinham em uma única coluna).  
- Verificados tipos de dados, valores nulos e duplicados.  

### 🔹 Tratamento de valores ausentes  
- **ID**: linhas com valor nulo removidas.  
- **Nome, Cidade, Produto**: preenchidos com `"Desconhecido"`.  
- **Idade, Preço, Quantidade**: preenchidos com a **mediana**.  
- **Data_Compra**: mantida como nula (`NaT`) quando ausente.  

### 🔹 Remoção de duplicados  
- 9 registros duplicados foram removidos.  

### 🔹 Correções adicionais  
- Conversão de tipos numéricos e datas (`dayfirst=True`).  
- Normalização de **Cidade** (ex.: `SP → SÃO PAULO`, `RJ → RIO DE JANEIRO`).  
- Padronização de **Produto** em *Title Case*.  

### 🔹 Exploração inicial  
- Estatísticas descritivas (média, mediana, desvio padrão etc.).  
- Gráficos:  
  - Histograma de **Preço**.  
  - Matriz de **correlação** entre variáveis numéricas.  

### 🔹 Desafio  
- Criadas novas colunas:  
  - **Faixa_Etaria** → classificação por idade.  
  - **Ticket_Total** = Preço × Quantidade.  

## ✅ Resultado  
A base final contém **501 registros limpos e consistentes**, prontos para análises futuras.  
