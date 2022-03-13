# GOF Criacional Factory Method

## Versionamento

| Versão |    Data    |     Modificação      | Autor | Revisor |
| ------ | :--------: | :------------------: | :---: | :-----: |
| 1.0 | 25/02/2022 | Criação do Documento | João Pedro Alves da Silva Chaves e Pedro Lima | Lucas Andrade e Dafne Moretti |

<!-- NÃO ESQUECER DE ADICIONAR AO "/_sidebar.md" -->

## Introdução

O padrão GOF criacional factory method é um padrão que tem como objetivo melhorar o desempenho do software em situações em que uma hierarquia está sendo muito acessada e também são demandadas muitas criações de instância, principalmente se isso for um gargalo. 

## Metodologia

O factory method funciona da seguinte forma: é criada uma hierarquia espelho que será dedicada à instanciação. Geralmente a classe abstrata da hierarquia espelho é referenciada como **Creator** e tem no mínimo uma relação de dependência com a classe abstrata da hierarquia "original"(para facilitar a compreensão vamos chamar de **Product**). 
A classe **Creator** tem um método abstrato de criação referenciado geralmente como factory Method (por isso o nome do padrão), porém pode possuir outros métodos e operações. A classe concreta que herda do **Creator** é chamada **ConcreteCreator**, que por meio da sobrescrita modifica o corpo do método factory Method para atender ao objetivo que é criar a instância do **Concrete Product**(classe que herda do **Product**).



## Conclusão

## Bibliografia
* SERRANO, Milene. Módulo Padrões de Projeto GoF(s) Criacionais - Material em Slides.
* Higor Medreiros. 2012. Padrão de Projeto Factory Method em Java. Disponível em https://www.devmedia.com.br/padrao-de-projeto-factory-method-em-java/26348. Acesso em 25 de fevereiro de 2022.