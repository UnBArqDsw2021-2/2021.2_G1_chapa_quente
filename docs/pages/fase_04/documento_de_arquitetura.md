# Documento de Arquitetura de Software - DAS

## Versionamento

| Versão |    Data    |                    Modificação                      |                      Autor                      |
| ------ | :--------: | :-------------------------------------------------: | :---------------------------------------------: |
| 1.0    | 09/04/2022 | Criação do Documento                                | Giulia Lobo Barros e Guilherme Daniel Fernandes |
| 1.1    | 11/04/2022 | Alteração de tópicos da estrutura do documento      | Giulia Lobo Barros e Guilherme Daniel Fernandes |
| 1.2    | 12/04/2022 | Adição das metas e restrições                       | Giulia Lobo Barros e Pedro Lima                 |
| 1.3    | 12/04/2022 | Adição dos casos de uso                             | Giulia Lobo Barros e Philipe Serafim            |
| 1.4    | 13/04/2022 | Adição da visão de processos                        | Giulia Lobo Barros e Murilo Gomes               |
| 1.5    | 13/04/2022 | Adição de frames para visualização dos diagramas    | Giulia Lobo Barros e Dafne Moretti              |
| 1.6    | 15/04/2022 | Adição da Visão de Dados                            | Liverson Paulo e Rodrigo Lima                   |
| 1.7    | 15/04/2022 | Adição da Visão de Implementação                    | Rodrigo Lima e Lucas Andrade                    |
| 1.8    | 15/04/2022 | Adição da parte de Tamanho e Desempenho do Software | Giulia Lobo e João Pedro Chaves                 |
| 1.9    | 15/04/2022 | Adição da parte de Visão Lógica                     | Rodrigo Lima e Murilo Gomes                     |
| 1.10   | 15/04/2022 | Adição introdução e representação arquitetural      | Guilherme Daniel Fernandes e Philipe Serafim    |
| 1.11   | 15/04/2022 | Adição de Visão de Implantação                      | Dafne Moretti e Rodrigo Lima                    |
| 1.12   | 15/04/2022 | Correções no documento de arquitetura               | Giulia Lobo Barros e Murilo Gomes               |

*Obs*: A revisão do documento foi feita em conjunto por todo o grupo.

## 1. Introdução

###  1.1. Finalidade

Esse documento tem como finalidade descrever os aspectos gerais referentes à arquitetura do projeto. Dessa forma, objetiva-se evidenciar as decisões arquiteturais tomadas, bem como os padrões adotados ao longo do densenvolvimento do projeto Chapa Quente.

### 1.2. Escopo

A finalidade desse documento é apresentar uma visão arquitetural geral do sistema desenvolvido para o projeto Chapa Quente. O documento será composto por padrões de software utilizados, componentes de software, frameworks de desenvolvimento, casos de uso e persistência de dados. Além disso, esse documento tem como objetivo descrever tecnicamente a solução adotada, tornando o projeto manutenível e apresentando os padrões a serem utilizados ao longo do seu desenvolvimento. 

###  1.3. Definições, Acrônimos e Abreviações 

| Abreviação | Acrônimo | Definição |
| :---------:| :-------:| :--------:|
| MVC | Model View Controller | Padrão de arquitetura de software, dividindo a solução em Model(M) que é a parte de regras de negócio, View(V) que é a parte responsável pela interface visualizável e Controller(C) que é responsável pelo controle dos dados. |
| JSON | JavaScript Object Notation | Formato compacto, de padrão aberto independente, de troca de dados simples e rápida entre sistemas. |
| NPM | Node Package Manage | Gerenciador de pacotes para o Node.js. |


### 1.4. Referências

* Documento de Arquitetura. Animalesco. Disponível em: https://unbarqdsw2021-1.github.io/2021.1_G01_Animalesco_docs/#/pages/das-documento-de-arquitetura?id=_12-escopo. Acesso em: 15/04/2022.
* Documento de Arquitetura. Ta na Mesa. Disponível em: https://unbarqdsw2021-1.github.io/2021.1_G02_TaNaMesa_docs/4-DAS/DAS/. Acesso em: 15/04/2022
* Documento de Arquitetura. Easy Coffe. Disponível em: https://unbarqdsw2020-2.github.io/2020.2_G5_EasyCoffee/#/entrega4/das. Acesso em: 15/04/2022
* Documento de Arquitetura. Curumim. Disponível em: https://unbarqdsw2021-1.github.io/2021.1_G6_Curumim/arquitetura-reutilizacao/arquitetura/. Acesso em: 15/04/2022.
* AULA - ARQUITETURA & DAS - PARTE II. Disponível em: https://aprender3.unb.br/pluginfile.php/1558855/mod_label/intro/Arquitetura%20e%20Desenho%20de%20Software%20-%20Aula%20Arquitetura%20e%20DAS%20-%20Parte%20II%20-%20Profa.%20Milene.pdf. Acesso em: 15/04/2022
* JSON. Disponível em: https://json.org/json-pt.html. Acesso em 15/04/2022.

### 1.5. Visão Geral

Este documento foi dividido em 7 partes com o objetivo de melhorar seu entendimento. Esse documento fica estruturado da seguinte forma:

| Tópico | Definição |
| :----: | :-------: |
| Representação Arquitetural | Tem como objetivo descrever a arquitetura da solução |
| Metas e Restrições da Arquitetura | Tem como objetivo descrever os requisitos e os objetivos do software que impactam na arquitetura |
| Visão Lógica | Tem como objetivo descrever as partes significativas do ponto de vista da arquitetura do modelo de design |
| Visão de Casos de Uso | Tem como objetivo descrever um modelo de alto nível com alta significância em relação às funcionalidades do sistema |
| Visão de Implantação | Tem como objetivo descrever a estrutura geral do modelo de implementação, a divisão do software em camadas e os subsistemas no modelo de implementação e todos os componentes significativos do ponto de vista da arquitetura |
| Visão de Processos | Tem como objetivo descrever a decomposição do sistema em processos leves e processos pesados |
| Visão de Dados | Tem como objetivo descrever a perspectiva de armazenamento de dados persistentes do sistema |
| Tamanho e Desempenho | Tem como objetivo descrever o tamanho da solução, bem como os requisitos mínimos para executá-la. |

## 2. Representação arquitetural

### **Banco de dados**
**MongoDB:** O MongoDB é um banco de dados opensource, de alta performance e flexível, sendo popular entre os bancos NoSQL. Ele tem como vantagens: maior escalabilidade e flexibilidade, bom desempenho e maior facilidade para consultas. Além disso, outra característica dele é que é orientado a documentos, ou seja, os dados são armazenados nele como documentos, diferente dos bancos relacionais que trabalham com registros de linhas e colunas. O uso do MongoDB permite uma maior tolerância a falhas, visto que esta é feita de forma automática. Outra característica importante é que o MongoDB funciona bem com Javascript, linguagem que utilizamos para o desenvolvimento da solução.

### **Backend**
**Node.js:** O Node.js é um software que permite a execução de código Javascript sem a necessidade de um navegador. Ele tem como vantagens a flexibilidade, visto que é possível realizar a instalação de outros pacotes pelo NPM e a leveza, visto que exige poucos recursos computacionais para execução. Além disso, utilizá-lo trás a vantagem de ter-se a mesma linguagem para o front e backend.

### **Frontend**

**React.js:** O React.js é uma biblioteca para Javascript que tem como foco a criação de UIs para páginas web de forma declaratica. É um framework amplamente utilizado na indústria e tem como características a facilidade para criação de UIs, extensa documentação, baixa curva de aprendizado e uma comunidade grande.

## 3. Metas Arquiteturais e Restrições da Arquitetura

### 3.1. Restrições

|  Restrições   | Descrição  |
| :-----------: | :--------: |
| Conectividade |   É necessário estabelecer conexão com internet para utilização do Chapa Quente.   |
| Idioma        |   O sistema deve ser desenvolvido para o idioma português do Brasil.   |
| Público       |   O aplicativo deve ser desenvolvido para administradores, entregadores e clientes da Lanchonete Chapa Quente.   |
| Plataforma    |   A aplicação terá suporte para browsers no computador.   |  
| Prazo Final   |   O escopo proposto deve ser terminado até o dia 18/04/2022.   |

### 3.2. Requisitos Não Funcionais

|      Metas       | Descrição  |
| :--------------: | :--------: |
|     Deploy       | A aplicação deve possuir deploy automatizado. |
| Escalabilidade   | O código deve ser estruturado e escalável o suficiente para estar aberto a futuras evoluções com o crescimento do projeto e a futuros usuários aderentes à aplicação. |
| Manutenibilidade | O código e as documentações realizadas pelo grupo devem estar em um nível de qualidade, seguindo os padrões de projeto e bibliografia, onde a sua manutenção seja fácil de ser realizada. |
| Responsividade   | A aplicação deve ser responsiva e se adaptar a todas as interfaces sem que haja comprometimento nas funções da aplicação. |
| Segurança        | O sistema deve ser seguro e lidar com os dados confidenciais dos usuários com segurança. |
| Suportabilidade  | Deve ser possível utilizar a plataforma em qualquer navegador web. |
| Usabilidade      | O sistema deve ser intuitivo e de simples uso, de forma que a curva de aprendizado para utilização dele seja fácil e clara. |

## 4. Visão Lógica

A **Visão Lógica** procura mostrar a organização do projeto decompondo certas em partes gerais para fácil compreensão, seguindo essa ideia, pode-se utilizar certos diagramas para fazer essa demonstração:

### 4.1. Diagrama de Pacote

Esse diagrama já foi desenvolvido pela equipe para uma entrega anterior, e pode ser facilmente acessado por meio do documento atual: [Diagrama de Pacote](pages/fase_02/diagrama_de_pacote.md).

<center><iframe height="600" width="700" src="https://unbarqdsw2021-2.github.io/2021.2_G1_chapa_quente/#/pages/fase_02/diagrama_de_pacote?id=vis%c3%a3o-geral"></iframe>
</center>

### 4.2. Diagrama de Classes
Esse diagrama já foi desenvolvido pela equipe para uma entrega anterior, e pode ser facilmente acessado por meio do documento atual: [Diagrama de Classes](pages/fase_02/diagrama_de_classes.md).

<center><iframe height="600" width="700" src="https://unbarqdsw2021-2.github.io/2021.2_G1_chapa_quente/#/pages/fase_02/diagrama_de_classes?id=diagrama-de-classes-1"></iframe>
</center>


### 4.3. Diagrama de Comunicação 
Esse diagrama já foi desenvolvido pela equipe para uma entrega anterior, e pode ser facilmente acessado por meio do documento atual: [Diagrama de Comunicação](pages/fase_02/diagrama_comunicacao.md).

<center><iframe height="600" width="700" src="https://unbarqdsw2021-2.github.io/2021.2_G1_chapa_quente/#/pages/fase_02/diagrama_comunicacao?id=diagramas-de-comunica%c3%a7%c3%a3o"></iframe>
</center>

### 4.4. Diagrama de Estados

Esse diagrama já foi desenvolvido pela equipe para uma entrega anterior, e pode ser facilmente acessado por meio do documento atual: [Diagrama de Estados](pages/fase_02/diagrama_de_estados.md).

<center><iframe height="600" width="700" src="https://unbarqdsw2021-2.github.io/2021.2_G1_chapa_quente/#/pages/fase_02/diagrama_de_estados?id=diagrama-de-login"></iframe>
</center>


## 5. Visão de Casos de Uso

Nesta seção, apresentamos a **visão de casos de uso**, definida como aquela que descreve um modelo de alto nível com significância em relação às funcionalidades do sistema. Normalmente, essa visão é representada pelo **diagrama de casos de uso**, que auxilia no entendimento das relações entre atores do sistema, descrevendo cenários de uso da aplicação.

### 5.1. Diagrama de Casos de Uso

Esse diagrama já foi desenvolvido pela equipe para uma entrega anterior, juntamente com a descrição de todos os seus casos de uso e pode ser facilmente acessado por meio do documento atual: [Diagrama de Casos de Uso](pages/fase_01/casos_de_uso.md).

<center><iframe height="600" width="700" src="https://unbarqdsw2021-2.github.io/2021.2_G1_chapa_quente/#/pages/fase_01/casos_de_uso?id=diagrama-de-casos-de-uso"></iframe>
</center>

*Obs.:* Importante destacar que todas as alterações necessárias relacionadas a esse diagrama já foram feitas para a entrega final.

## 6. Visão de Implementação
A **Visão de Implementação** procura mostrar como o sistema será desenvolvido e organizado. Pode-se então utilizar o Diagrama de Componetes para tal demonstração.

### 6.1. Diagrama de Componentes

Esse diagrama já está disponível no escopo do nosso projeto, basta acessar: [Diagrama de Componentes](pages/fase_02/diagrama_de_componentes.md).
<center><iframe height="600" width="700" src="https://unbarqdsw2021-2.github.io/2021.2_G1_chapa_quente/#/pages/fase_02/diagrama_de_componentes?id=metodologia"></iframe>
</center>

## 7. Visão de Implantação
**Visão de Implantação** trata-se de explicar de forma simplificada como os componentes se relacionam e dependem entre si.
No diagrama abaixo cada seta significa que a parte apontada depende da parte que aponta de alguma forma.

![Diagrama de Implantação](../../assets/images/diagrama_de_implantacao.png)
> Figura 1: Diagrama de Implantação. Autor: Rodrigo Lima. 

## 8. Visão de Processos

A **visão de processos** descreve como o sistema de tempo-de-execução é estruturado na forma de um conjunto de elementos que têm interações e comportamento de tempo-de-execução. A estrutura de tempo-de-execução normalmente tem pouca semelhança com a estrutura de código. Além disso, permite a visualização das partes dinâmicas do sistema, onde são evidenciados os processos, as threads e as interações entre elas.

Nessa visão, nós podemos ter 2 representações que auxiliam em seu entendimento:

### 8.1. Diagrama de Atividades

Esse diagrama já está disponível no escopo do nosso projeto, basta acessar: [Diagrama de Atividades](pages/fase_02/diagrama_de_atividade.md).

<center><iframe height="600" width="700" src="https://unbarqdsw2021-2.github.io/2021.2_G1_chapa_quente/#/pages/fase_02/diagrama_de_atividade?id=diagramas-de-atividade"></iframe>
</center>

*Obs.:* Importante destacar que todas as alterações necessárias relacionadas a esse diagrama já foram feitas para a entrega final.

### 8.2. Diagrama de Sequência

Esse diagrama já está disponível no escopo do nosso projeto, basta acessar: [Diagrama de Sequência](pages/fase_02/diagrama_de_sequencia.md).

<center><iframe height="600" width="700" src="https://unbarqdsw2021-2.github.io/2021.2_G1_chapa_quente/#/pages/fase_02/diagrama_de_sequencia?id=vis%c3%a3o-geral"></iframe>
</center>

*Obs.:* Importante destacar que todas as alterações necessárias relacionadas a esse diagrama já foram feitas para a entrega final.

## 9. Visão de Dados
A **visão de Dados** é um tópico que se dispõe a mostrar quais são os dados persistentes na aplicação, geralmente utiliza-se ferramentas como um Modelo Entidade-Relacionamento e/ou Diagrama Entidade-Relacionamento para isso, entretanto no projeto Chapa Quente foi utilizado um sistema não-relacional, tornando essas ferramentas inoportunas nesse contexto. Como foi utilizado o MongoDB, que é um banco de dados orientado a documentos JSON, foi preferivel utilizar um sistema que mostra os objetos da camada "Model", pois esses são os objetos que são mapeados para a camada persistente, ou seja, para o banco de dados.

Para melhor visualização, as tabelas que mostram os objetos supracitados foram dividos em duas imagens:

![Visao de dados - pedido](../../assets/images/visao_de_dados_pedido.png)
> Figura 2: Visão de dados - pedido. Autor: Rodrigo Lima. 

![Visao de dados - pessoa](../../assets/images/visao_de_dados_pessoa.png)
> Figura 3: Visão de dados - pessoa. Autor: Rodrigo Lima. 

## 10. Tamanho e Desempenho

### 10.1. Requisitos Mínimos

* É necessário possuir conexão com a internet;
* Navegador com suporte a HTML 5, CSS e JavaScript;
* Para desenvolvimento possuir: Windows, Linux ou MacOS.

### 10.2. Visão Geral

O tamanho da aplicação, tendo como base todos os repositórios, juntos dão menos que 1GB, sendo que não é necessária a instalação de nenhum outro programa para seu funcionamento. Já quanto ao desempenho, para o uso do sistema, é necessário conexão com a internet, além disso, a opção de dispositivo é flexível, podendo ser utilizado tanto em todos os tipos de computadores. O desempenho também considera a grande gama de pessoas que utiliza o aplicativo diariamente, contando com cliente, cozinheiros, funcionários em geral e entregadores.