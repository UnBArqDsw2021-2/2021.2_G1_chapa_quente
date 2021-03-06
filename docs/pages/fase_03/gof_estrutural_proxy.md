# GOF Estrutural Proxy

## Versionamento

| Versão |    Data    |     Modificação      | Autor | Revisor |
| ------ | :--------: | :------------------: | :---: | :-----: |
| 1.0    | 04/03/2022 | Criação do Documento | Dafne Moretti e Rodrigo Lima   | Lucas Andrade e Dafne Moretti |
| 1.1    | 16/03/2022 | Adição de exemplo de código |  Rodrigo Lima   | Murilo Gomes e Giulia Lobo |
| 1.2    | 16/03/2022 |   Correção do path   |       Philipe Serafim        | Lucas Andrade e Dafne Moretti |

<!-- NÃO ESQUECER DE ADICIONAR AO "/_sidebar.md" -->

## Introdução

O padrão Proxy baseia-se em encapsular um objeto através de um outro objeto que implementa a mesma interface, de forma que o segundo objeto, conhecido como “Proxy”, controla o acesso ao primeiro, que é o objeto real.

- Um proxy virtual é um marcador de espaço para objetos "caros de criar". O objeto real só é criado quando é feita a primeira requisição ou acesso ao objeto.
- Um proxy remoto fornece um representante local para um objeto que reside em um espaço de endereço diferente.
- Um proxy de proteção controla o acesso a um objeto mestre sensível. O objeto intermediário verifica se o aquele que faz a chamada tem as permissões de acesso necessárias antes de encaminhar a requisição.
- Um proxy inteligente interpõe ações adicionais quando um objeto é acessado. Os usos típicos incluem:
  - Contando o número de referências ao objeto real para que ele possa ser liberado automaticamente quando não houver mais referências (também conhecido como ponteiro inteligente),
  - Carregando um objeto persistente na memória quando é referenciado pela primeira vez,
  - Verificar se o objeto real está bloqueado antes de ser acessado para garantir que nenhum outro objeto possa alterá-lo.


## Metodologia

### Exemplo de Diagrama e Código

Ao definir uma interface Subject, a presença do objeto Proxy no lugar do RealSubject é transparente para o cliente.

![Exemplo de Proxy](../../assets/images/proxy.png)

<figcaption style="text-align: center"><a href="./assets/images/proxy.png" >Figura 1 </a>: Exemplo de Proxy. Fonte: <a href="https://sourcemaking.com/design_patterns/proxy" > Proxy Design Pattern
 </a>. Acesso em: 04/03/2022 </figcaption>

 Um exemplo bem rudimentar feito em C# em uma aplicação do escopo seria:

 ![Exemplo de Código de Proxy](../../assets/images/proxyCode.png)
 <figcaption> Figura 2 - Exemplo de código de Proxy em C#. Adaptado de: DevMedia. </figcaption>

## Conclusão

O padrão Proxy tem diversas utilidades desde melhorar o desempenho do software criando um proxy para um objeto "pesado" a melhorar a segurança usando o proxy no processo de checar se há a permissão para acesso do objeto real. Apesar de ser muito útil o uso do proxy em aplicações, ele não será implementado no projeto Chapa Quente, visto que sua implementação pode ser complexa e atrapalharia o escopo do projeto, já que a ausência dele não faria muita falta para o escopo proposto.

## Bibliografia

- SERRANO, Milene. Padrões de Projeto - Gofs - Estruturais. Acesso em: 04 de março de 2022.

- SOURCE MAKING - Proxy Design Pattern. Disponível em: https://sourcemaking.com/design_patterns/proxy . Acesso em: 04 de março de 2022.

- DevMedia - Conheça o Pattern Proxy - GoF (Gang of Four). Disponível em: https://www.devmedia.com.br/conheca-o-pattern-proxy-gof-gang-of-four/4066 . Acesso em: 04 de março de 2022.
