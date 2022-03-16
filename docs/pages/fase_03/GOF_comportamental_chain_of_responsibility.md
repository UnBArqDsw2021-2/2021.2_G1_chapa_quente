# GOF comportamental Chain of responsibility

## Versionamento

| Versão | Data       | Modificação          | Autor                        |Revisor|
| ------ | :--------: | :------------------: | :--------------------------: | :---: |
| 1.0    | 25/01/2022 | Criação do Documento | Liverson Paulo e Lucas Andrade | Dafne Moretti e João Pedro |

## Introdução e Metodologia

É um padrão comportamental, cujo o propósito é evitar que hajam dependência entre um objeto receptor e um objeto solicitante. Portanto ele vai permitir que passe pedidos por uma corrente de handlers, em que ao receber um pedido, cada handler vai decidir se processa ou passa um pedido para o handler adiante na corrente.

Abaixo há um exemplo do funcionamento de Chain of Responsibility associando com o mundo real.

![](../../assets/images/chainofresponsibility.png)

<figcaption> Exemplo de Chain of Responsibility. Tirado de https://refactoring.guru/pt-br/design-patterns/chain-of-responsibility<figcaption>

## Conclusão

Este GOF comportamental pode ser extremamente importante para o projeto, já que em um sistema de lanchonete há pedidos com os quais é necessário lidar o tempo inteiro, portanto este GOF comportamental é bem-vindo na aplicação do projeto.

## Bibliografia

Chain of responsibility. Disponível em: https://pt.wikipedia.org/wiki/Chain_of_Responsibility. Acesso 02/03/2022

Design Patterns - Chain of responsibility. Disponível em: https://refactoring.guru/pt-br/design-patterns/chain-of-responsibility. Disponível em: 04/03/2022
