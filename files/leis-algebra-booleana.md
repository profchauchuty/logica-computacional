# Leis da Álgebra Booleana

A Álgebra Booleana é um sistema matemático criado por **George Boole** para representar operações lógicas utilizando apenas dois valores: **0 (falso)** e **1 (verdadeiro)**. Ela é a base da Computação e da Eletrônica Digital, sendo utilizada na construção de circuitos, processadores, memórias e sistemas computacionais.

Para simplificar expressões lógicas e reduzir a complexidade dos circuitos digitais, utilizamos as **Leis da Álgebra Booleana**. Essas leis permitem transformar expressões complexas em expressões equivalentes mais simples, facilitando a análise, o desenvolvimento e a otimização de sistemas digitais.

---

## Lei da Identidade

### Explicação

A Lei da Identidade mostra que existem valores que não alteram o resultado de uma operação lógica. Na operação OR, o valor **0** é considerado neutro, pois não interfere no valor da variável. Dessa forma, o resultado permanece exatamente igual ao valor original.

### Expressão

```text
A + 0 = A
```

### Exemplo

```text
1 + 0 = 1
0 + 0 = 0
```

---

## Lei da Dominância (Anulação)

### Explicação

Os valores **1** e **0** dominam completamente a operação. Em uma operação OR, basta existir um valor 1 para que o resultado seja 1. Em uma operação AND, basta existir um valor 0 para que o resultado seja 0.

### Expressão

```text
A + 1 = 1
A · 0 = 0
```

### Exemplo

```text
0 + 1 = 1
1 · 0 = 0
```

---

## Lei da Idempotência

### Explicação

Repetir a mesma variável em uma expressão não altera o resultado. Como os dois termos possuem exatamente o mesmo valor, a saída continua sendo a própria variável.

### Expressão

```text
A + A = A
A · A = A
```

### Exemplo

```text
1 + 1 = 1
0 · 0 = 0
```

---

## Lei do Complemento

### Explicação

A Lei do Complemento relaciona uma variável ao seu valor oposto (negado). Como uma variável e seu complemento sempre possuem valores contrários, em uma operação OR pelo menos um dos termos será verdadeiro, produzindo resultado 1. Já em uma operação AND, um dos termos será sempre falso, produzindo resultado 0. Essa lei demonstra que uma variável combinada com sua negação gera sempre um resultado previsível.

### Expressão

```text
A + ¬A = 1
A · ¬A = 0
```

### Exemplo

```text
1 + ¬1 = 1
1 · ¬1 = 0
```

---

## Lei da Dupla Negação

### Explicação

Aplicar a negação duas vezes faz com que a variável retorne ao seu valor original. A segunda negação cancela completamente o efeito da primeira.

### Expressão

```text
¬(¬A) = A
```

### Exemplo

```text
¬(¬1) = 1
¬(¬0) = 0
```

---

## Lei da Comutatividade

### Explicação

A ordem das variáveis não altera o resultado da operação. Podemos trocar a posição dos termos sem modificar o valor final da expressão.

### Expressão

```text
A + B = B + A
A · B = B · A
```

### Exemplo

```text
1 + 0 = 0 + 1
1 · 0 = 0 · 1
```

---

## Lei da Associatividade

### Explicação

A forma de agrupar as variáveis não interfere no resultado. Os parênteses podem ser reorganizados sem alterar a lógica da expressão.

### Expressão

```text
(A + B) + C = A + (B + C)
(A · B) · C = A · (B · C)
```

### Exemplo

```text
(1 + 0) + 1 = 1 + (0 + 1)

(1 · 1) · 0 = 1 · (1 · 0)
```

---

## Lei da Distributividade

### Explicação

Permite expandir ou fatorar expressões booleanas. Essa propriedade é muito utilizada na simplificação de circuitos e expressões lógicas.

### Expressão

```text
A · (B + C) = A·B + A·C
A + (B · C) = (A + B) · (A + C)
```

### Exemplo

```text
X · (Y + Z) = X·Y + X·Z
```

---

## Lei da Absorção

### Explicação

Quando uma variável já é suficiente para determinar o resultado, os demais termos tornam-se desnecessários. Dizemos que a variável absorve a expressão complementar.

### Expressão

```text
A + A·B = A
A · (A + B) = A
```

### Exemplo

```text
A + A·B = A
```

---

## Leis de De Morgan

### Explicação

Ao distribuir uma negação sobre uma expressão composta, cada variável é negada individualmente e o operador lógico é invertido. O operador AND transforma-se em OR e o operador OR transforma-se em AND. Essas leis são amplamente utilizadas na simplificação de circuitos digitais.

### Expressão

```text
¬(A · B) = ¬A + ¬B
¬(A + B) = ¬A · ¬B
```

### Exemplo

```text
¬(X + Y) = ¬X · ¬Y
```

---

## Lei do Consenso

### Explicação

Alguns termos podem ser redundantes porque já estão representados pelos demais termos da expressão. Essa lei permite eliminar esses termos sem alterar o resultado lógico.

### Expressão

```text
A·B + ¬A·C + B·C = A·B + ¬A·C
```

### Exemplo

```text
X·Y + ¬X·Z + Y·Z = X·Y + ¬X·Z
```

---

## Lei da Simplificação

### Explicação

Permite reduzir expressões booleanas eliminando termos desnecessários. É amplamente utilizada em conjunto com outras leis para simplificar circuitos digitais.

### Expressão

```text
A · (¬A + B) = A·B
A + (¬A · B) = A + B
```

### Exemplo

```text
X · (¬X + Y) = X·Y
```
