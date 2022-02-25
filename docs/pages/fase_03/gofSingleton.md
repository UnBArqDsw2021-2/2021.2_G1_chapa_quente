# GoF Singleton

## Versionamento

| Versão |    Data    |     Modificação      | Autor | Revisor |
| ------ | :--------: | :------------------: | :---: | :-----: |
| 1.0    | 25/02/2022 | Criação do Documento |  Guilherme Fernandes     |         |

<!-- NÃO ESQUECER DE ADICIONAR AO "/_sidebar.md" -->

## Introdução
Os padrões de projeto descrevem uma solução geral para um problema que acontece recorrentemente dentro de um projeto de software. Este documento tem como objetivo explicar sobre o padrão GoF Singleton e suas aplicações. 

## Metodologia
O Singleton é um GoF criacional que permite que uma classe disponha de apenas uma instância, podendo ser acessada globalmente em outras classes. Dessa forma, uma classe será responsável por gerenciar a própria instância, além de evitar que novas instâncias sejam criadas. Abaixo, um exemplo de Singleton em C#:
```
 public sealed class Singleton {

        private Singleton() { }

        private static Singleton _instance;

        public static Singleton GetInstance() {
            if (_instance == null) {
                _instance = new Singleton();
            }

            return _instance;
        }
 }
```
## Aplicabilidade

O padrão Singleton é utilizado quando uma classe no programa deve ter apenas uma instância disponível para todos. Uma aplicação que poderia ser feita dentro do projeto Chapa Quente seria da utilização do Singleton na classe do usuário, pois, dessa forma, seria possível acessar utilizar as informações do usuário nas diferentes telas que compõem a aplicação sem a necessidade de criação de instâncias da classe a cada nova tela. Além disso, as alterações realizadas no objeto global seriam homogeneas, afetando todas as telas que fizessem uso dele. Outra aplicação seria no banco de dados. Dessa forma, o singleton relacionado ao banco estaria disponível em outras classes da aplicação, sem que fosse necessário criar um objeto do banco a cada classe em que ele fosse necessário.

## Vantagens e desvantagens

| Vantagens | Desvantagens |
| :-------: | :----------: |
| Certeza de que uma classe terá somente uma instância| Viola o princípio de responsabilidade única |
| Dispõe de um ponto de acesso global para aquela instância | Pode mascarar um design ruim, pois, dentre outras coisas, os componentes do programa sabem muito sobre os outros |
| O singleton é iniciado somente na primeira vez que for invocado | Requer, em algumas linguagens, tratamento especial para que múltiplas threads não possam criar um objeto singleton várias vezes |
| | Pode dificultar na criação de testes unitários, pois alguns frameworks dependem de herança para a produção de objetos simulados. Como o construtor da classe é privado e a maioria das linguagens não sobrescrevem métodos estáticos, é necessário ser criativo na criação de testes. |

## Conclusão

O padrão Singleton é amplamente utilizado na indústria e soluciona problemas recorrentes em diversas aplicações. Todavia, deve ser utilizado com cautela para que não se torne um antipadrão devido, principalmente, ao fato dele violar o princípio de responsabilidade única.

## Bibliografia

- Padrão de Projeto Singleton em Java. Disponível em: <https://www.devmedia.com.br/padrao-de-projeto-singleton-em-java/26392>. (último acesso em 25/02/2022)
- Singleton. Disponível em: <https://refactoring.guru/design-patterns/singleton>. (último acesso em 25/02/2022)
- Singleton Design Pattern. Disponível em: <https://www.geeksforgeeks.org/singleton-design-pattern/>. (último acesso em 25/02/2022)

