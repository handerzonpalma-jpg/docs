# Estruturas de Decisão na Lógica de Programação

As estruturas de decisão (ou condicionais) são os componentes que permitem que um algoritmo "escolha" qual caminho seguir. Elas são a base da inteligência de qualquer software, permitindo que o código reaja a diferentes entradas e situações.

---

## 1. O Conceito Fundamental
Uma estrutura de decisão avalia uma **condição** (uma expressão que resulta em `Verdadeiro` ou `Falso`) e executa um bloco de código específico baseando-se nesse resultado.

### Operadores Relacionais
Para criar condições, utilizamos comparadores:
* `==` : Igual a
* `!=` : Diferente de
* `>`  : Maior que
* `<`  : Menor que
* `>=` : Maior ou igual a
* `<=` : Menor ou igual a

### Operadores Lógicos
Para combinar múltiplas condições:
* **AND (E):** Verdadeiro apenas se todas as condições forem verdadeiras.
* **OR (OU):** Verdadeiro se pelo menos uma condição for verdadeira.
* **NOT (NÃO):** Inverte o valor da condição.

---

## 2. Tipos de Estruturas

### 🟢 Estrutura Simples (`if`)
Executa uma ação apenas se a condição for atendida. Se for falsa, o programa simplesmente ignora o bloco.

```python
if saldo >= valor_saque:
    print("Saque realizado com sucesso!")