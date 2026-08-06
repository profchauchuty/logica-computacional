# Operações Matemáticas em Binário

## 1. Conceito

Os computadores realizam operações matemáticas utilizando apenas dois valores:

0 e 1

Esses valores são chamados de bits.

As quatro operações básicas são:

- Soma
- Subtração
- Multiplicação
- Divisão

Assim como no sistema decimal, as operações possuem regras próprias, porém utilizando apenas números binários.

---

# 2. Soma Binária

A soma binária funciona de forma semelhante à soma decimal.

## Regras:

| A | B | Resultado |
|---|---|---|
|0|0|0|
|0|1|1|
|1|0|1|
|1|1|10|

A regra mais importante:

1 + 1 = 10

O resultado possui dois valores:

- 0 permanece na posição atual.
- 1 é enviado para a próxima posição.

Esse valor enviado é chamado de:

**Carry (vai-um)**

---

## Exemplo:

      10
    + 10
    ----

Primeira posição:

0 + 0 = 0


Segunda posição:

1 + 1 = 10


Resultado:

      10
    + 10
    ----
     100


Convertendo:

10₂ = 2₁₀

100₂ = 4₁₀


Portanto:

10₂ + 10₂ = 100₂

---

# 3. Subtração Binária

A subtração segue as mesmas ideias da matemática decimal.

## Regras:

| A | B | Resultado |
|---|---|---|
|0|0|0|
|1|0|1|
|1|1|0|
|0|1|Precisa emprestar|

A principal diferença ocorre quando:

0 - 1

Nesse caso precisamos pegar um valor emprestado da próxima posição.

Esse valor é chamado de:

**Borrow (empréstimo)**

---

## Exemplo:

      10
    + 01
    ----

Na primeira posição:

0 - 1

Não é possível.

Então realizamos um empréstimo.

Resultado:

      10
    + 01
    ----
       1


Convertendo:

10₂ = 2₁₀

01₂ = 1₁₀

Resultado:

1₂ = 1₁₀

---

# 4. Multiplicação Binária

A multiplicação binária funciona igual à multiplicação decimal.

As regras são:

| A | B | Resultado |
|---|---|---|
|0|0|0|
|0|1|0|
|1|0|0|
|1|1|1|

Observe:

Qualquer número multiplicado por 0 resulta em 0.

Qualquer número multiplicado por 1 permanece igual.

---

## Exemplo:

      101
    x  10
    -----
       1

Multiplicando pelo 0:

101 × 0 = 000


Multiplicando pelo 1:

101 × 1 = 101

Como o 1 está na segunda posição, deslocamos uma casa:

    101
   000
  -----
   1010


Resultado:

101₂ × 10₂ = 1010₂


Convertendo:

101₂ = 5₁₀

10₂ = 2₁₀

1010₂ = 10₁₀


Portanto:

5 × 2 = 10

---

# 5. Divisão Binária

A divisão binária funciona da mesma forma que a divisão decimal.

Ela utiliza:

- Divisão
- Subtração
- Deslocamento de bits

---

## Exemplo:
      100
    ÷  10
    -----
        1

Convertendo:

100₂ = 4₁₀

10₂ = 2₁₀


Então:

4 ÷ 2 = 2


Resultado:

100₂ ÷ 10₂ = 10₂


---

# 6. Circuitos Lógicos das Operações

## Soma

Circuito:

Meio Somador (Half Adder)

Utiliza:

XOR → Soma

AND → Carry


---

## Subtração

Circuito:

Meio Subtrator (Half Subtractor)

Utiliza:

XOR → Diferença

AND + NOT → Borrow


---

## Multiplicação

Normalmente utiliza:

- Portas AND
- Somadores

A multiplicação é feita através de somas repetidas.

---

## Divisão

Utiliza:

- Subtratores
- Comparadores
- Controle lógico

A divisão é uma sequência de subtrações.

---

# 7. Resumo das Operações

|Operação|Ideia principal|Conceito importante|
|-|-|-|
|Soma|Adicionar valores|Carry (vai-um)|
|Subtração|Retirar valores|Borrow (empréstimo)|
|Multiplicação|Somas repetidas|Deslocamento|
|Divisão|Subtrações repetidas|Quociente e resto|

Os computadores realizam todas essas operações utilizando circuitos digitais formados por portas lógicas.
