# Nome do Artefato

## Versionamento

| Versão |    Data    |     Modificação      | Autor | Revisor |
| ------ | :--------: | :------------------: | :---: | :-----: |
| 1.0    | 07/02/2022 | Criação do Documento |  João Pedro Chaves e Murilo Gomes     | Lucas Andrade e Dafne Moretti |

<!-- NÃO ESQUECER DE ADICIONAR AO "/_sidebar.md" -->

## Introdução

MVC é um padrão de arquitetura de software proposto por Trygve Reenskaug nos anos 70 dentro da linguagem Smalltalk, que foi uma das primeiras linguagens de programação puramente orientada a objetos. O MVC consiste em dividir o código em três diferentes camadas conectadas entre si, visando separar os conceitos e as responsabilidades de cada uma, são elas: Modelo(Model), Visão(View) e Controladora(Controller).

## Metodologia

<p style="text-align: center"><img src="assets/images/mvc.png"></p>
<figcaption style="text-align: center"><a href="../assets/images/mvc.png">Figura 1:</a> Diagrama do MVC. Disponível em: <a href="https://blog.taller.net.br/mvc-vs-pac-diferenca-entre-arquiteturas/">https://blog.taller.net.br/mvc-vs-pac-diferenca-entre-arquiteturas/</a></figcaption>

### Modelo (Model)

É a camada lógica da aplicação, responsável por implementar comportamentos, restrições e validações do negócio. Tem como objetivo gerenciar e controlar a maneira na qual os dados se comportam através de funções, lógicas e as regras de negócio estabelecidas.

### Visão (View)

Camada responsável por mostrar as informações ao usuário de forma visual. É utilizada para receber entrada de dados e apresentar visualmente o resultado. Sua implementação deve consistir apenas em componentes visuais, sem implementar nenhuma lógica e/ou regra de negócio, já que essas são responsabilidades do Modelo. 

### Controladora (Controller)

É a camada que faz a gerência das outras duas camadas. É responsável por receber dados inseridos pelo usuário através da Visão, manipular os mesmos e enviar para o Modelo fazer a validação, também é reponsável por buscar dados do Modelo para serem demonstrados na Visão.

## Conclusão

Dada as explicações mostradas acima, foi decidido em grupo utilizar o padrão MVC pelos seguintes motivos:

* Facilidade de reaproveitamento do código
* Facilidade de manutenção e adição de novas funcionalidades
* Proteção das regras de negócio contidas na camada Modelo de alterações feitas na camada de Visão
* Maior integração da equipe e/ou divisão de tarefas
* Facilidade em manter o código limpo

### Implementações:

## Bibliografia

BASTOS, Daniel Flores. O que é Model-view-controller (MVC)?. [S. l.], 28 mar. 2011. Disponível em: https://www.oficinadanet.com.br/artigo/desenvolvimento/o_que_e_model-view-controller_mvc. Acesso em: 7 mar. 2022.

Wikipedia. MVC. Disponível em: https://pt.wikipedia.org/wiki/MVC. Acesso em: 7 mar. 2022.

CAMPOZANO, Nelson Nunes. As Camadas MVC. [S. l.], 19 jun. 2013. Disponível em: http://fabrica.ms.senac.br/2013/06/as-camadas-mvc/. Acesso em: 7 mar. 2022.

ZUCHER, Vitor. O que é padrão MVC? Entenda arquitetura de softwares!. [S. l.], 17 jul. 2022. Disponível em: https://www.lewagon.com/pt-BR/blog/o-que-e-padrao-mvc#:~:text=O%20MVC%20%C3%A9%20uma%20sigla,sejam%20mais%20r%C3%A1pidas%20e%20din%C3%A2micas. Acesso em: 7 mar. 2022.

ZANLUCA, Marcel Luiz. MVC vs. PAC: qual a diferença entre as arquiteturas?. [S. l.], 12 abr. 2018. Disponível em: https://blog.taller.net.br/mvc-vs-pac-diferenca-entre-arquiteturas/. Acesso em: 7 mar. 2022.

MASSARI, Jorge. Padrão MVC | Arquitetura Model-View-Controller. [S. l.], 2018. Disponível em: https://www.portalgsti.com.br/2017/08/padrao-mvc-arquitetura-model-view-controller.html. Acesso em: 7 mar. 2022.