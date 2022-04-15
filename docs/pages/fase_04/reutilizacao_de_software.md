# Reutilização de Software

## Versionamento

| Versão |    Data    |            Modificação             |                Autor                |                             Revisor                             |
| ------ | :--------: | :--------------------------------: | :---------------------------------: | :-------------------------------------------------------------: |
| 1.0    | 11/04/2022 |        Criação do Documento        |         Liverson Paulo, Giulia Lobo Barros e Guilherme Daniel Fernandes          |                  A definir                |

## 1.Introdução

A reutilização de software se baseia no uso de conceitos, produtos ou soluções previamente elaboradas ou adquiridas para criação de um novo software, visando melhorar significativamente a qualidade e a produtividade.
A reutilização pode ser introduzida em diferentes fases e níveis do desenvolvimento de software: requisitos, design, código. É mais comum a reutilização de porções de código, design e testes, do que a reutilização de requisitos. A reutilização em fases com maior nível de abstração aumenta os benefícios da mesma e facilita a reutilização em fases mais avançadas do ciclo de vida do produto.

## 2.Backend

### Middlewares

Os middlewares desenvolvidos na API conferem uma ótima forma de reutilização de software visto que um middleware pode ser utilizado de forma desacoplada em diferentes rotas e em diferentes contextos.

### Controllers

As Controllers são responsáveis por controlar todo o fluxo de informação que passa pelo sistema. Define quais informações devem ser geradas, quais regras devem ser acionadas e para onde as informações devem ir, ou seja, executa regras de negócio e repassa as informações.

## 3.Frontend

### Components

Os components têm como principal objetivo dividir a interface em partes independentes e reutilizáveis, onde cada parte é tratada de forma isolada livre de dependências externas. Eles recebem entradas e têm como retorno elementos react que vão aparecer na tela.

### Services

As services têm como funcionalidade a conexão com o Backend, neste caso foi utilizado Axios para poder realizar essa conexão e facilitar a comunicação entre o Back e o Front

## 4.Docker e Docker-compose

Docker é uma plataforma aberta, criada com o objetivo de facilitar o desenvolvimento, a implantação e a execução de aplicações em ambientes isolados. Foi desenhada especialmente para disponibilizar uma aplicação da forma mais rápida possível.

Já o Docker-compose vai orquestrar o funcionamento dos containers Docker, onde os desenvolvedores serão como maestros orquestrando uma banda, porém neste caso será o comportamento da aplicação, utilizando essa ferramenta para fazer com que isso seja viável.

Ao utilizar o Docker e Docker-compose foi possível alcançar uma maior padronização em relação aos recursos utilizados pelos desenvolvedores, assim houve uma facilitação no fluxo de trabalho, fato que resulta em um empacotamento de maior qualidade por causa da uniformidade entre os ambientes utilizados pelos desenvolvedores.

No Backend foram utilizados no Node.js e para fazer a conexão com o banco de dados mongoDB.

Já no Frontend foi utilizado para o desenvolvimento utilizando React.js.

## 5.Bibliografia

[1] SERRANO, M; Arquitetura e Desenho de Software, Aula - Reutilização de Software. UnB-FGA. Acesso em: 11/04/2022.
[2] DEVMEDIA. Reutilização de Software - Revista Engenharia de Software Magazine 39. Disponível em: https://www.devmedia.com.br/reutilizacao-de-software-revista-engenharia-de-software-magazine-39/21956. Acesso em: 15/04/2022
[3]Desenvolvedor expert - O que é docker? Disponível em: https://stack.desenvolvedor.expert/appendix/docker/oquee.html. Acesso em: 15/04/2022
[4] Trucco, Cristian. Docker Compose: O que é? Para que serve? O que come?. Disponível em: https://imasters.com.br/banco-de-dados/docker-compose-o-que-e-para-que-serve-o-que-come. Acesso em: 15/04/2022
[5] Axios. O que é Axios? Disponível em: https://axios-http.com/ptbr/docs/intro Acesso em: 15/04/2022