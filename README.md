# Order Management System

## Sobre o projeto

Este projeto consiste em um sistema de gerenciamento de pedidos desenvolvido em Java, como parte dos estudos de Programação Orientada a Objetos.

A aplicação permite cadastrar os dados de um cliente, criar um pedido, adicionar produtos com suas respectivas quantidades e preços e, ao final, apresentar um resumo completo do pedido no terminal.

O exercício tem como objetivo praticar a construção de classes, o relacionamento entre objetos e a organização de responsabilidades dentro de uma aplicação Java.

## Funcionalidades

- Leitura dos dados do cliente: nome, e-mail e data de nascimento.
- Registro do status do pedido.
- Registro automático do instante de criação do pedido.
- Inclusão de uma quantidade variável de itens no pedido.
- Associação de cada item a um produto.
- Cálculo do subtotal de cada item.
- Cálculo do valor total do pedido.
- Exibição de um resumo com os dados do pedido, cliente e produtos.

## Estrutura do projeto

O projeto está organizado em dois pacotes principais:

- `application`: contém a classe responsável pela execução do programa.
- `entities`: contém as classes que representam as entidades do sistema.

### Classes e enumerações

| Classe / Enum | Responsabilidade                                                                  |
| ------------- | --------------------------------------------------------------------------------- |
| `Program`     | Executa a aplicação e realiza a leitura dos dados informados pelo usuário.        |
| `Client`      | Representa o cliente, armazenando nome, e-mail e data de nascimento.              |
| `Order`       | Representa o pedido, mantendo seus dados, o cliente associado e a lista de itens. |
| `OrderItem`   | Representa um item do pedido, com quantidade, preço e produto associado.          |
| `Product`     | Representa um produto, com nome e preço.                                          |
| `OrderStatus` | Define os possíveis estados de um pedido.                                         |

## Conceitos de Java praticados

- Programação Orientada a Objetos (POO).
- Criação de classes, atributos, construtores e métodos.
- Encapsulamento.
- Composição e associação entre objetos.
- Enumerações (`enum`).
- Manipulação de listas com `ArrayList`.
- Estruturas de repetição (`for`).
- Entrada de dados com `Scanner`.
- Manipulação de datas com `LocalDate` e `LocalDateTime`.
- Formatação de datas com `DateTimeFormatter`.
- Sobrescrita do método `toString()`.
- Construção de textos com `StringBuilder`.

## Exemplo de execução

```text
Enter cliente data:
Name: Alex Green
Email: alex@gmail.com
Birth date (DD/MM/YYYY): 15/03/1985

Enter order data:
Status: PROCESSING

How many items to this order? 2

Enter #1 item data:
Product name: TV
Product price: 1000.00
Quantity: 1

Enter #2 item data:
Product name: Mouse
Product price: 40.00
Quantity: 2

ORDER SUMMARY:
Order moment: 20/04/2018 11:25
Order status: Processing
Client: Alex Green (15/03/1985) - alex@gmail.com
Order items:
TV, $1000.00, Quantity: 1, Subtotal: $1000.00
Mouse, $40.00, Quantity: 2, Subtotal: $80.00
Total price: $1080.00
```

## Tecnologias utilizadas

- Java
- Java Collections Framework (`ArrayList`)
- Java Time API (`LocalDate`, `LocalDateTime` e `DateTimeFormatter`)

## Como executar

1. Clone este repositório.
2. Abra o projeto em uma IDE compatível com Java, como IntelliJ IDEA ou Eclipse.
3. Execute a classe `Program`, localizada no pacote `application`.
4. Informe os dados solicitados pelo terminal.

---

Projeto desenvolvido para fins de estudo e prática de Programação Orientada a Objetos com Java.
