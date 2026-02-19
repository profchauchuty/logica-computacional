# Tabela Verdade

Uma **proposição composta** pode ser verdadeira ou falsa, dependendo das proposições simples que a formam. As operações entre essas proposições são expressas na **tabela verdade**.

---

## 1. Resumo sobre Tabela Verdade

A tabela verdade é um instrumento lógico que apresenta **todos os valores lógicos de uma proposição composta**. Ela é usada na **lógica matemática** para analisar proposições formadas por operações entre proposições simples.

As principais operações lógicas são:  

- **Negação (~)**  
- **Conjunção (˄)**  
- **Disjunção (˅)**  
- **Condicional (→)**  
- **Bicondicional (↔)**  

---

## 2. Principais Conectivos Lógicos

| Operação       | Símbolo | Significado           |
|----------------|---------|---------------------|
| Negação        | ~       | não                 |
| Conjunção      | ˄       | e                   |
| Disjunção      | ˅       | ou                  |
| Condicional    | →       | se... então         |
| Bicondicional  | ↔       | se e somente se     |

**Modo de ler:**  
- `~p` — “não p”  
- `p ˄ q` — “p e q”  
- `p ˅ q` — “p ou q”  
- `p → q` — “se p então q”  
- `p ↔ q` — “p se e somente se q”  

> Observação: A bicondicional `p ↔ q` equivale à condicional nos dois sentidos: `p → q` e `q → p`.

---

## 3. Tabelas Verdade dos Conectivos

### 3.1 Negação (~)

**Tabela Pura:**

| p | ~p |
|---|----|
| V | F  |
| F | V  |

**Com exemplo:**

| Está chovendo (p) | Não está chovendo (~p) |
|------------------|------------------------|
| V                | F                      |
| F                | V                      |

---

### 3.2 Conjunção (˄)

**Tabela Pura:**

| p | q | p ˄ q |
|---|---|-------|
| V | V | V     |
| V | F | F     |
| F | V | F     |
| F | F | F     |

**Com exemplo:**

| Estudei para a prova (p) | Entreguei o trabalho (q) | Fiz as duas coisas? (p ˄ q) |
|---------------------------|-------------------------|------------------|
| V                         | V                       | V (fiz os dois) |
| V                         | F                       | F (só estudei)  |
| F                         | V                       | F (só entreguei)|
| F                         | F                       | F (não fiz nenhum)|

---

## 3. Tabelas Verdade dos Conectivos

### 3.1 Negação (~)

**Tabela Pura:**

| p | ~p |
|---|----|
| V | F  |
| F | V  |

**Com exemplo:**

| Está chovendo (p) | Não está chovendo (~p) | Resultado |
|------------------|------------------------|-----------|
| V                | F                      | F         |
| F                | V                      | V         |

---

### 3.2 Conjunção (˄)

**Tabela Pura:**

| p | q | p ˄ q |
|---|---|-------|
| V | V | V     |
| V | F | F     |
| F | V | F     |
| F | F | F     |

**Com exemplo:**

| Estudei para a prova (p) | Entreguei o trabalho (q) | Fiz as duas coisas? (p ˄ q) | Resultado |
|---------------------------|-------------------------|-----------------------------|-----------|
| V                         | V                       | Sim                         | V         |
| V                         | F                       | Não                         | F         |
| F                         | V                       | Não                         | F         |
| F                         | F                       | Não                         | F         |

---

### 3.3 Disjunção (˅)

**Tabela Pura:**

| p | q | p ˅ q |
|---|---|-------|
| V | V | V     |
| V | F | V     |
| F | V | V     |
| F | F | F     |

**Com exemplo:**

| Vou ao cinema (p) | Vou ao shopping (q) | Pelo menos uma atividade? (p ˅ q) | Resultado |
|------------------|-------------------|----------------------------------|-----------|
| V                | V                 | Sim                              | V         |
| V                | F                 | Sim                              | V         |
| F                | V                 | Sim                              | V         |
| F                | F                 | Não                              | F         |

---

### 3.4 Condicional (→)

**Tabela Pura:**

| p | q | p → q |
|---|---|-------|
| V | V | V     |
| V | F | F     |
| F | V | V     |
| F | F | V     |

**Com exemplo:**

| Estudei para a prova (p) | Passei na prova (q) | Consequência? (p → q) | Resultado |
|---------------------------|-------------------|-----------------------|-----------|
| V                         | V                 | Passei porque estudei | V         |
| V                         | F                 | Estudei mas não passei | F        |
| F                         | V                 | Passei sem estudar    | V         |
| F                         | F                 | Não estudei e não passei | V      |

---

### 3.5 Bicondicional (↔)

**Tabela Pura:**

| p | q | p ↔ q |
|---|---|-------|
| V | V | V     |
| V | F | F     |
| F | V | F     |
| F | F | V     |

**Com exemplo:**

| Tenho ingresso para o cinema (p) | Entrei no cinema (q) | Situação correta? (p ↔ q) | Resultado |
|---------------------------------|--------------------|---------------------------|-----------|
| V                               | V                  | Tudo certo                | V         |
| V                               | F                  | Não entrei mesmo com ingresso | F      |
| F                               | V                  | Entrei sem ingresso       | F         |
| F                               | F                  | Tudo certo                | V         |

---

## 4. Construção de uma Tabela Verdade Composta

**Exemplo:** `~(p ˄ q)`

| Estudei para a prova (p) | Entreguei o trabalho (q) | Estudei e entreguei (p ˄ q) | Não estudei ou não entreguei (~(p ˄ q)) | Resultado |
|---------------------------|-------------------------|-----------------------------|---------------------------------------|-----------|
| V                         | V                       | Sim                         | Não                                   | F         |
| V                         | F                       | Não                         | Sim                                   | V         |
| F                         | V                       | Não                         | Sim                                   | V         |
| F                         | F                       | Não                         | Sim                                   | V         |

---

**Referência Bibliográfica:**  
RIZZO, Maria Luiza Alves. *Tabela verdade*. Brasil Escola. Disponível em: [https://brasilescola.uol.com.br/matematica/tabela-verdade.htm](https://brasilescola.uol.com.br/matematica/tabela-verdade.htm). Acesso em 18 de fevereiro de 2026.
