# GoF Observer

## Versionamento

| Versão |    Data    |     Modificação      | Autor | Revisor |
| ------ | :--------: | :------------------: | :---: | :-----: |
| 1.0    | 25/02/2022 | Criação do Documento | Guilherme Fernandes |         |

<!-- NÃO ESQUECER DE ADICIONAR AO "/_sidebar.md" -->

## Introdução
Os padrões GoF buscam solucionar problemas recorrentes em projetos da Engenharia de Software. Neste documento será tratado acerca do padrão Observer, um padrão comportamental amplamente utilizado em aplicações e APIs disponíveis no mercado.

## Metodologia
O Observer é um padrão GoF comportamental que consiste na criação de um mecanismo de assinatura que notifica múltiplos objetos quando qualquer evento que eles estão observando acontece. Dessa forma, é possível para um objeto observar os eventos que ocorrem em N objetos aos quais ele está observando. 

No padrão Observer há dois papéis:
- Subject: a entidade que faz a publicação dos eventos.
- Observer: a entidade que recebe os eventos, ou seja, recebe atualizações quando os dados do subject são alterados.

## Aplicação
Este padrão GoF é amplamente utilizado, principalmente quando se fala sobre programação reativa. Há diversas APIs que implementam esse padrão, dentre elas: RxJS, RxSwift etc. O padrão Observer é extremamente útil quando mudanças em um objeto podem precisar mudar outros objetos e o conjunto atual de objetos é desconhecido ou muda dinamicamente. Dois exemplos de aplicações muito utilizados é em interfaces de usuário e em APIs REST que enviam dados dinamicamente.

## Vantagens e desvantagens

| Vantagens | Desvantagens |
| :--------:| :-----------:|
| Você pode induzir novas classes subscriber sem ter que mudar o código do publisher | Subscribers são notificados em ordem aleatória |
| É possível estabelecer conexões entre objetos em runtime | |

## Conclusão
O padrão Observer é útil em vários tipos de aplicação. Dessa forma, é necessário verificar os prós e contras da sua aplicação. No contexto da aplicação Chapa Quente, este padrão pode ser utilizado em telas que dependem da atualização de informações do back-end para que sejam atualizadas. Um exemplo a ser utilizado é o da tela de rastreamento do pedido, onde ela estará sempre observando a atualização da localização do entregador para apresentar ao usuário.

## Bibliografia
- **Observer.** Disponível em: <https://refactoring.guru/design-patterns/observer>. (último acesso em 25/02/2022)
- **Design Patterns - Observer Pattern.** Disponível em: <https://www.tutorialspoint.com/design_pattern/observer_pattern.htm>. (último acesso em 25/02/2022)
- **Reactive Extensions Library for JavaScript.** Disponível em: <https://rxjs.dev>. (último acesso em 25/02/2022)
- **5 Things to Know About Reactive Programming.** Disponível em: <https://developers.redhat.com/blog/2017/06/30/5-things-to-know-about-reactive-programming> (último acesso em 25/02/2022)