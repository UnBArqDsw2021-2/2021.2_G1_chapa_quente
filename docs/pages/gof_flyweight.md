# GOF Flyweight 

## Versionamento

| Versão |    Data    |     Modificação      | Autor | Revisor |
| ------ | :--------: | :------------------: | :---: | :-----: |
| 1.0    | 25/02/2022 | Criação do Documento |  Dafne Moretti Moreira   |         |

## GOF Flyweight

O GOF Flyweight é um padrão de projeto que lida com objetos e segundo GAMMA, seu objetivo é suportar, com eficiência, muitos objetos utilizando o conceito de compartilhamento. A ideia, é que o estado intrínseco dos objetos seja compartilhado entre vários visando reduzir o uso da memória RAM.

Sua aplicabilidade acontece quando objetos são utilizados para construir outros objetos ou quando a aplicação usa um grande número de objetos.

A Figura 1 apresenta de um modo didático como funciona o pool de objetos imutáveis.

![Ilustração do funcionamento do flyweight](./assets/images/casinhas.png ":size=200") </br> Figura 1 - Persona. Fonte: [https://thispersondoesnotexist.com/](ThisPersonDoesNotExist) |

A Figura 2, mostra um exemplo de diagrama de objetos que ilustra o flyweight.

![Diagrama que apresenta o flyweight](./../../assets/images/flyweight_diagrama.png ":size=200") </br> Figura 2 - Persona. Fonte: [https://thispersondoesnotexist.com/](ThisPersonDoesNotExist) |


## Conclusão

Após o estudo e percepção do que seria o padrão de projeto flyweight, percebeu-se que é possível utilizá-lo no projeto Chapa Quente, uma vez que haverá muitos objetos iguais na aplicação, sendo esses muitos sandhuíches, por exemplo, ou muitas bebidas. 

## Bibliografia

Erich Gamma ... [and others]. Design Patterns : Elements of Reusable Object-Oriented Software. Reading, Mass. :Addison-Wesley, 1995.

FLYWEIGHT Teoria - Padrões de Projeto - Parte 25/45. [S. l.: s. n.], 2020. Disponível em: https://www.youtube.com/watch?v=WPQa64bdQbk. Acesso em: 25 fev. 2022.

ROCHA, Helder. Padrões de Design com aplicações em Java. 2005. Apresentação do Power Point. Disponível em: https://www.inf.ufpr.br/andrey/ci163/Design_Patterns.pdf. Acesso em: 25 fev. 2022.

JOHNSON, Thienne. Padrões de Projeto de Software Orientado a Objetos. 2005. Apresentação do Power Point. Disponível em: http://www.usp.br/thienne/coo/material/aula17-introducaoPP.pdf. Acesso em: 25 fev. 2022.
