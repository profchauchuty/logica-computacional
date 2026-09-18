# Atividade — Tratamento de Erros e Exceções em TypeScript

> **“O tratamento de erros é importante, mas se obscurece a lógica, está errado.”**
> — Robert C. Martin, *Código Limpo (Clean Code)*

Pesquise sobre **Tratamento de Erros e Exceções em Programação** e responda às 5 questões propostas, utilizando **TypeScript** nos exemplos práticos.

As respostas devem demonstrar compreensão dos conceitos pesquisados.

**A atividade será complementada por uma AVALIAÇÃO ORAL em sala de aula, sem consulta. O aluno deverá responder perguntas básicas sobre o conteúdo e explicar os códigos apresentados. Caso não demonstre conhecimento básico sobre a atividade entregue, a nota da atividade será zero.**

### Entrega

Responda às questões em um arquivo **`atividade-erros-excecoes.md`**, publique-o em um repositório no **GitHub** e entregue o **link do arquivo** no **Sala de Aula**.

## Questões

### 1. Tratamento de erros e exceções

Explique:

* O que é **tratamento de erros**?
* O que é uma **exceção**?
* Qual a diferença entre **erro** e **exceção**?
* Por que é importante tratar erros e exceções?

Apresente um exemplo em **TypeScript**.

### 2. Tratamento de exceções

Explique a finalidade do tratamento de exceções.

Apresente um exemplo em **TypeScript** utilizando `try` e `catch` e explique seu funcionamento.

### 3. `try`, `catch` e `finally`

Explique a função de:

* `try`
* `catch`
* `finally`

Apresente um exemplo em **TypeScript** utilizando as três estruturas.

### 4. `throw`

Explique para que serve o `throw`.

Crie um exemplo em **TypeScript** que identifique uma situação inválida, lance uma exceção e faça seu tratamento.

### 5. Aplicação prática

Crie, em **TypeScript**, uma função para realizar uma transferência bancária.

A função deve:

* Rejeitar valores menores ou iguais a zero;
* Rejeitar transferências maiores que o saldo;
* Lançar uma exceção para situações inválidas;
* Tratar as exceções.

Demonstre pelo menos **duas situações de erro** e explique o funcionamento do código.
