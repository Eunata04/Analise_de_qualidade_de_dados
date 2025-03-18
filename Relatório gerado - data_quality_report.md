# 📄 Relatório de Qualidade de Dados

## 🔎 Checagem Individual das Tabelas
### Checagem de Qualidade - CSV
- **Duplicadas**: 0
- **Total de valores nulos**: 6

#### 📈 Estatísticas Descritivas (Colunas Numéricas)
| Coluna | Mínimo | Máximo | Média | Mediana | Desvio Padrão |
|--------|--------|--------|-------|---------|---------------|
| age | 18.0 | 92.0 | 38.92 | 37.0 | 10.49 |
| creditscore | 350 | 850 | 650.54 | 652.0 | 96.66 |
| customerid | 15565701 | 15815690 | 15690934.31 | 15690733.0 | 71935.31 |
| exited | 0 | 1 | 0.2 | 0.0 | 0.4 |
| numofproducts | 1 | 4 | 1.53 | 1.0 | 0.58 |
| tenure | 0 | 10 | 5.01 | 5.0 | 2.89 |

### Checagem de Qualidade - SQL
- **Duplicadas**: 0
- **Total de valores nulos**: 0

#### 📈 Estatísticas Descritivas (Colunas Numéricas)
| Coluna | Mínimo | Máximo | Média | Mediana | Desvio Padrão |
|--------|--------|--------|-------|---------|---------------|
| age | 18 | 85 | 38.71 | 37.0 | 10.7 |
| balance | 0.0 | 221532.8 | 76609.71 | 98252.42 | 62295.99 |
| creditscore | 410 | 850 | 646.63 | 650.0 | 95.6 |
| customerid | 15565701 | 15815690 | 15573451.57 | 15572796.5 | 11081.88 |
| estimatedsalary | 236.45 | 199420.41 | 97810.81 | 96099.64 | 58268.0 |
| numofproducts | 1 | 4 | 1.52 | 1.0 | 0.57 |
| tenure | 0 | 10 | 5.1 | 5.0 | 2.84 |

## ⚖️ Comparação de Dados
### 📋 Overview
- **Número de linhas no CSV**: **10001**
- **Número de linhas na tabela SQL**: **558**

### 🔠 Comparação de Colunas
#### Colunas em comum:
age, balance, creditscore, customerid, estimatedsalary, exited, gender, geography, hascrcard, isactivemember, numofproducts, surname, tenure

Não há colunas ausentes no CSV.

### 🔄 Comparação de Tipos de Dados
| Coluna | Tipo no CSV | Tipo no SQL |
|--------|-------------|-------------|
| age | float64 | int64 |
| balance | object | float64 |
| creditscore | int64 | int64 |
| customerid | int64 | int64 |
| estimatedsalary | object | float64 |
| exited | int64 | bool |
| gender | object | object |
| geography | object | object |
| hascrcard | object | bool |
| isactivemember | object | bool |
| numofproducts | int64 | int64 |
| surname | object | object |
| tenure | int64 | int64 |

### 💰 Comparação de Somatórias (Colunas Numéricas)
| Coluna | Soma no CSV | Soma no SQL | Diferença |
|--------|-------------|-------------|-----------|
| age | 389132.0 | 21599 | 367533.0 |
| creditscore | 6506080 | 360820 | 6145260 |
| customerid | 156925034013 | 8689985977 | 148235048036 |
| exited | 2038 | 114 | 1924 |
| numofproducts | 15303 | 846 | 14457 |
| tenure | 50132 | 2845 | 47287 |

### 🕳️ Valores Faltantes (Comparativo)
| Coluna | Faltantes no CSV | Faltantes no SQL |
|--------|------------------|------------------|
| age | 3 | 0 |
| balance | 0 | 0 |
| creditscore | 0 | 0 |
| customerid | 0 | 0 |
| estimatedsalary | 0 | 0 |
| exited | 0 | 0 |
| gender | 0 | 0 |
| geography | 0 | 0 |
| hascrcard | 0 | 0 |
| isactivemember | 0 | 0 |
| numofproducts | 0 | 0 |
| surname | 3 | 0 |
| tenure | 0 | 0 |

### 📊 Estatísticas Descritivas (Comparativo)
| Coluna | Média CSV | Média SQL | Desvio Padrão CSV | Desvio Padrão SQL |
|--------|----------|-----------|-------------------|-------------------|
| age | 38.92 | 38.71 | 10.49 | 10.7 |
| creditscore | 650.54 | 646.63 | 96.66 | 95.6 |
| customerid | 15690934.31 | 15573451.57 | 71935.31 | 11081.88 |
| exited | 0.2 | 0.2 | 0.4 | 0.4 |
| numofproducts | 1.53 | 1.52 | 0.58 | 0.57 |
| tenure | 5.01 | 5.1 | 2.89 | 2.84 |

### ⚠️ Resumo de Erros
- Diferença no número de linhas: CSV possui 10001 linhas, enquanto SQL possui 558.
- Diferença na somatória da coluna **customerid**: CSV = 156925034013, SQL = 8689985977.
- Diferença na somatória da coluna **creditscore**: CSV = 6506080, SQL = 360820.
- Diferença na somatória da coluna **age**: CSV = 389132.0, SQL = 21599.
- Diferença na somatória da coluna **tenure**: CSV = 50132, SQL = 2845.
- Diferença na somatória da coluna **numofproducts**: CSV = 15303, SQL = 846.
- Diferença na somatória da coluna **exited**: CSV = 2038, SQL = 114.
