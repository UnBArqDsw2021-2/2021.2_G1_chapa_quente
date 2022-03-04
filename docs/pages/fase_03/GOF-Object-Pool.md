# GOF Object Pool

## Versionamento

| Versão | Data       | Modificação          | Autor                        |Revisor|
| ------ | :--------: | :------------------: | :--------------------------: | :---: |
| 1.0    | 02/03/2022 | Criação do Documento | Lucas Andrade | Dafne Moretti Moreira |

## Introdução

O padrão criacional **Object Pool** é usado quando estamos lidando com classes com um alto custo de inicialização. A ideia é colocar as classes instanciadas em uma "pool", e quando for necessário elas são chamadas.

Os objetos possuem o ciclo de vida de **criação**, **validação** e **destruição**.

Também é possivel fazer um paralelo com a ideia de um cache.

## Metodologia

O Object Pool funciona como um local que reune as instâncias das classes, e quando necessário, é feito uma chamada pela instância desejada. É desejado que todos os objetos instanciados estejam na mesma pool, e por isso é recomendado que a classe do pool seja uma classe Singleton.

<img
    src="../../assets/images/GOF-Object_Pool-Example.png"
    style="background-color: white"
/>
<figcaption style="text-align: center">Interação entre o cliente e a pool. Fonte: https://sourcemaking.com/</figcaption>

## Conclusão

O padrão Object Pool tem a capacidade de oferecer um bom ganho de performance para o projeto, porém possui casos de uso bastante específicos e são, normalmente, implementadas como singleton. A equipe não viu, até o momento, nenhum cenário de utilização do padrão Object Pool no projeto.

## Bibliografia

- Object Pool Design Pattern. [S. l.]. Disponível em: https://sourcemaking.com/design_patterns/object_pool. Acesso em: 02 de março de 2022.

- Object Pool Design Pattern. [S. l.]. Disponível em: https://www.geeksforgeeks.org/object-pool-design-pattern/. Acesso em: 02 de março de 2022.