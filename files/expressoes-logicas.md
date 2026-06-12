# Expressões Lógicas

Uma **expressão lógica** é uma combinação de valores lógicos (entradas) e operadores lógicos que produz um único resultado.

Uma expressão lógica sempre produz um resultado VERDADEIRO (V) ou FALSO (F).

Exemplo:

```text
A = B = VERDADEIRO
S = A ∧ B
S = VERDADEIRO
```

Onde:

- `A` e `B` são entradas lógicas;
- `∧` é o operador lógico;
- `S` é a saída (resultado) da expressão.

---

# Operadores Fundamentais

## 1. NOT (NÃO)

Inverte o valor lógico da entrada.

### Símbolos

```text
NOT
¬
!
~
```

### Expressão

```text
S = ¬A
```

### Tabela Verdade

| A | ¬A|
|---|---|
| V | F |
| F | V |

---

## 2. AND (E)

Verdadeiro somente quando todas as entradas forem verdadeiras.

### Símbolos

```text
AND
∧
&&
.
```

### Expressão

```text
S = A ∧ B
```

### Tabela Verdade

| A | B | A ∧ B |
|---|---|---|
| V | V | V |
| V | F | F |
| F | V | F |
| F | F | F |

---

## 3. OR (OU)

Verdadeiro quando pelo menos uma entrada for verdadeira.

### Símbolos

```text
OR
∨
||
+
```

### Expressão

```text
S = A ∨ B
```

### Tabela Verdade

| A | B | A ∨ B |
|---|---|---|
| V | V | V |
| V | F | V |
| F | V | V |
| F | F | F |

---

# Operadores Derivados

## 4. XOR (OU Exclusivo)

Verdadeiro quando as entradas forem diferentes.

### Símbolos

```text
XOR
⊕
^
```

### Expressão

```text
S = A ⊕ B
```

### Tabela Verdade

| A | B | A ⊕ B |
|---|---|---|
| V | V | F |
| V | F | V |
| F | V | V |
| F | F | F |

### Interpretação

```text
Um ou outro, mas não ambos.
```

---

## 5. NAND

Negação do operador AND.

### Símbolos

```text
NAND
↑
```

### Expressão

```text
S = ¬(A ∧ B)
```

### Tabela Verdade

| A | B | ¬(A ∧ B) |
|---|---|---|
| V | V | F |
| V | F | V |
| F | V | V |
| F | F | V |

---

## 6. NOR

Negação do operador OR.

### Símbolos

```text
NOR
↓
```

### Expressão

```text
S = ¬(A ∨ B)
```

### Tabela Verdade

| A | B | ¬(A ∨ B) |
|---|---|---|
| V | V | F |
| V | F | F |
| F | V | F |
| F | F | V |

---

## 7. XNOR (NXOR)

Negação do XOR.

### Símbolos

```text
XNOR
NXOR
≡
↔
```

### Expressão

```text
S = A ↔ B
```

### Tabela Verdade

| A | B | A ↔ B |
|---|---|---|
| V | V | V |
| V | F | F |
| F | V | F |
| F | F | V |

### Interpretação

```text
Verdadeiro quando as entradas forem iguais.
```

---

# Operadores de Implicação

## 8. Implicação

Representa uma condição lógica.

### Símbolos

```text
→
=>
IMPLICA
```

### Expressão

```text
S = A → B
```

### Leitura

```text
Se A, então B.
```

### Tabela Verdade

| A | B | A → B |
|---|---|---|
| V | V | V |
| V | F | F |
| F | V | V |
| F | F | V |

### Equivalência

```text
S = ¬A ∨ B
```

---

## 9. Implicação Inversa

### Símbolos

```text
←
<=
```

### Expressão

```text
S = A ← B
```

### Equivalência

```text
S = B → A
```

### Tabela Verdade

| A | B | A ← B |
|---|---|---|
| V | V | V |
| V | F | V |
| F | V | F |
| F | F | V |

---

## 10. Bicondicional

Também chamado de dupla implicação.

### Símbolos

```text
↔
⇔
SE E SOMENTE SE
```

### Expressão

```text
S = A ↔ B
```

### Tabela Verdade

| A | B | A ↔ B |
|---|---|---|
| V | V | V |
| V | F | F |
| F | V | F |
| F | F | V |

### Equivalência

```text
S = A ≡ B
```

---

## 11. Não-Implicação

Negação da implicação.

### Símbolo

```text
↛
```

### Expressão

```text
S = ¬(A → B)
```

### Tabela Verdade

| A | B | S = ¬(A → B) |
|---|---|---|
| V | V | F |
| V | F | V |
| F | V | F |
| F | F | F |

---

## 12. Não-Implicação Inversa

### Símbolo

```text
↚
```

### Expressão

```text
S = ¬(B → A)
```

### Tabela Verdade

| A | B | ¬(B → A) |
|---|---|---|
| V | V | F |
| V | F | F |
| F | V | V |
| F | F | F |

---

# Constantes Lógicas

## Verdadeiro

### Símbolos

```text
1
⊤
TRUE
V
```

### Expressão

```text
S = 1
```

### Tabela Verdade

| S = 1 |
|---|
| V |

---

## Falso

### Símbolos

```text
0
⊥
FALSE
F
```

### Expressão

```text
S = 0
```

### Tabela Verdade

| S = 0 |
|---|
| F |

---

# Equivalência Lógica

Indica que duas expressões possuem exatamente a mesma tabela verdade.

### Símbolo

```text
≡
```

### Exemplo

```text
S = (A → B)
S = (¬A ∨ B)
```

As duas expressões geram exatamente os mesmos resultados.

---

# Resumo Geral

| Operador | Nome | Expressão |
|-----------|---------|---------|
| ¬ | NOT | S = ¬A |
| ∧ | AND | S = A ∧ B |
| ∨ | OR | S = A ∨ B |
| ⊕ | XOR | S = A ⊕ B |
| ↑ | NAND | S = ¬(A ∧ B) |
| ↓ | NOR | S = ¬(A ∨ B) |
| ≡ | XNOR (NXOR) | S = A ≡ B |
| → | Implicação | S = A → B |
| ← | Implicação Inversa | S = A ← B |
| ↔ | Bicondicional | S = A ↔ B |
| ↛ | Não-Implicação | S = ¬(A → B) |
| ↚ | Não-Implicação Inversa | S = ¬(B → A) |
| ⊤ | Verdadeiro | S = 1 |
| ⊥ | Falso | S = 0 |

---
