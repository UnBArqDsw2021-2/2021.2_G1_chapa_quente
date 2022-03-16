# GoF Mediator

 ## Versionamento

 | Versão |    Data    |     Modificação      | Autor | Revisor |
 | ------ | :--------: | :------------------: | :---: | :-----: |
 | 1.0    | 07/03/2022 | Criação do Documento |  Guilherme Fernandes  | Giulia Lobo e Lucas Andrade |
 | 1.1    | 16/03/2022 | Adição do código em forma de imagem | João Pedro Chaves | Giulia Lobo e Lucas Andrade |

 <!-- NÃO ESQUECER DE ADICIONAR AO "/_sidebar.md" -->

 ## Introdução
 Os padrões de projeto descrevem uma solução geral para um problema que acontece recorrentemente dentro de um projeto de software. Este documento tem como objetivo explicar sobre o padrão GoF comportamental Mediator e suas aplicações. 

 ## Metodologia
 O Mediator é um GoF comportamental que permite que haja uma redução das dependências caóticas entre classes. Ele consiste na restrição de comunicação direta entre objetos e exige que eles interajam entre si apenas por meio de um objeto mediador. Abaixo, um exemplo de Mediator em C#:
 
<div style="text-align: center"><img src="./assets/images/mediator_code.png">
<figcaption><a href="../../assets/images/mediator_code.png">Figura 1:</a> Exemplo de aplicação do Mediator. Autor: Guilherme Fernandes </figcaption></div>

 ## Aplicabilidade

 É possível utilizar o GoF comportamental Mediator é aplicado em diversos contextos, sendo principalmente utilizado em soluções onde é necessário que classes se comuniquem sem que seja necessário um alto acoplamento entre elas. Por utilizar uma interface como mediador, é interessante para implementações que utilizam classes que contém as mesmas funções, mas com implementação diferente. Um exemplo é classes que realizam autenticação de serviços, pois é possível definir um protocolo chamado Autenticação e passar para o mediador qual serviço será utilizado (ex: Firebase, Facebook, Google Sign In, etc). Dessa forma, é possível reduzir o acoplamento entre classes, aumentar a testabilidade e a manutenibilidade da solução, além de permitir que o código seja reutilizado em outras partes da aplicação. 

 ## Vantagens e desvantagens

 | Vantagens | Desvantagens |
 | :-------: | :----------: |
 | Respeita o princípio da responsabilidade única. | Pode evoluir para um Objeto Deus com o tempo. 
 | Respeita o princípio aberto/fechado |
 | Reduz o acoplamento entre os componentes do programa. |  |
 | Permite a reutilização de código mais facilmente. |  |

 ## Conclusão

O padrão Mediator é amplamente utilizado por reduzir o acoplamento entre classes. Dessa forma, seu uso é extremamente interessante para que haja um aumento da qualidade da aplicação. Todavia, esse padrão deve ser arquitetado cautelosamente na solução para que não haja a criação de um Objeto Deus. Além disso, é um padrão recomendado em soluções que apresentem classes com comportamentos parecidos, mas que fazem implementações distintas. Sendo assim, no contexto do nosso projeto, não há aplicações aparentes para a utilização do Mediator pois ele adiciona uma camada de abstração desnecessária no escopo do projeto, visto que se trata de um projeto menos robusto e complexo. 

 ## Bibliografia

 - Mediator. Disponível em: <https://refactoring.guru/pt-br/design-patterns/mediator>. (último acesso em 07/03/2022)
 - Mediator em C#. Disponível em: <https://refactoring.guru/pt-br/design-patterns/mediator/csharp/example>. (último acesso em 07/03/2022)

