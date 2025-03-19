# 🔎 Relatório de Qualidade de Dados

<span style="color:red">Obs: </span>Projeto em desenvolvimento


Este projeto tem como objetivo realizar uma checagem de qualidade dos dados entre um arquivo CSV e uma tabela SQL. Através deste processo, simulei um cenário típico do ambiente de trabalho, no qual é necessário verificar se os dados importados de um arquivo CSV para uma tabela SQL foram transferidos corretamente. O foco principal é a validação das colunas e a comparação entre as duas fontes de dados, garantindo que a integridade e a consistência das informações estejam preservadas durante o processo de importação.

No nosso caso de estudo a importação do CSV para o Banco de dados foi realizado de forma errada propositalmente no intuito de verificar este erro.

## 🚀 Funcionalidades

- **Carregamento de dados**: Carrega dados de um arquivo CSV e de uma tabela SQL Server.
- **Normalização de colunas**: Padroniza os nomes das colunas para garantir uma comparação adequada.
- **Verificação de qualidade de dados**:
  - Contagem de duplicatas e valores nulos.
  - Estatísticas descritivas para colunas numéricas (mínimo, máximo, média, mediana, desvio padrão).
  - Comparação entre as duas fontes de dados (CSV e SQL Server), incluindo número de linhas, colunas, tipos de dados, somatórios e valores faltantes.
- **Geração de Relatório**: Gera um relatório detalhado em formato Markdown sobre a qualidade dos dados.

---

## 🛠️ Tecnologias Utilizadas

- **Python**: Para manipulação dos dados e geração do relatório.
- **Pandas**: Para carregar, manipular e analisar os dados.
- **NumPy**: Para manipulação de dados numéricos.
- **pyodbc**: Para conexão e interação com o banco de dados SQL Server.
- **Markdown**: Para formatação do relatório de qualidade.

---

## 📈 Funcionalidades do Relatório

### 1. Checagem de Qualidade Individual
O relatório inclui uma checagem detalhada de cada fonte de dados (CSV e SQL), verificando:
- **Duplicatas**: Quantidade de registros duplicados.
- **Valores nulos**: Contagem de valores ausentes.
- **Estatísticas descritivas**: Mínimo, máximo, média, mediana e desvio padrão para colunas numéricas.

### 2. Comparação entre CSV e SQL Server
O relatório também compara os dados entre as duas fontes, com informações sobre:
- **Número de linhas**: Comparação do número de registros entre as fontes.
- **Colunas em comum**: Quais colunas existem em ambas as fontes.
- **Tipos de dados**: Comparação dos tipos de dados para as colunas em comum.
- **Somatórias**: Comparação dos valores somados para colunas numéricas.
- **Valores faltantes**: Quantidade de valores ausentes em ambas as fontes.
- **Estatísticas descritivas**: Comparação das estatísticas para colunas numéricas.

### 3. Erros
O relatório apresenta um resumo de erros.

---
