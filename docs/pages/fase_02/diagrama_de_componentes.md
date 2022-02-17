# Nome do Artefato

## Versionamento

| Versão |    Data    |     Modificação      | Autor | Revisor |
| ------ | :--------: | :------------------: | :---: | :-----: |
| 1.0    | 16/02/2022 | Criação do Documento | João Pedro Alves da Silva Chaves |         |
| 1.1    | 16/02/2022 | Adição de introdução e tabela com legenda | Dafne Moretti Moreira |         |
| 1.2    | 17/02/2022 | Adição da metodologia e item da legenda | João Pedro Alves da Silva Chaves |   |

## Introdução

O diagrama de componentes é um diagrama estático cuja função principal é apresentar os componentes (módulos mais “gerais” do sistema) e suas relações com os demais subsistemas e componentes. A utilização do diagrama de componentes favorece a visualização geral do sistema e a percepção das partes que podem ser reutilizadas. 

É criado em linguagem de modelagem unificada (UML) e apresenta dependências, interfaces, portas e os próprios componentes. A ideia é que não fique um diagrama muito específico para que seja de fácil entendimento e identificação dos principais aspectos da aplicação, no entanto, existem diagramas com diferentes níveis de granularidade.

## Legenda

| Símbolo |  Nome  |  Descrição |
| ------ | ---------- | ------------ |
| ![Componente](./../../assets/images/componente.png ":size=200") </br> Fonte: Autoria própria  | Componente | Ilustra os componentes do sistema |
| ![Dependência](./../../assets/images/dependencia.png ":size=200") </br> Fonte: Autoria própria    | Dependência | Representa a relação de dependência entre partes do sistema. |
| ![Porta](./../../assets/images/porta.png ":size=200") </br> Fonte: Autoria própria   | Porta |  Simboliza a comunicação entre o ambiente externo e os componentes. |
| ![Interface](./../../assets/images/interface.png ":size=200") </br> Fonte: Autoria própria   | Interface |  Simboliza a interface necessária para o relacionamento entre os componentes. |

## Metodologia

O desenvolvimento do diagrama de componentes foi feito com base a documentação do **Chapa Quente** e chegamos nos seguintes subsistemas: Autenticação, Lanchonete, Pedido, Cardápio. A plataforma utilizada para o desenvolvimento do diagrama foi o [draw.io](https://app.diagrams.net), pois é uma ferramenta gratuita e com os elementos necessários para a tarefa desejada.

![Diagrama de Componentes](../../assets/images/diagrama_de_componentes.png)
<figcaption>Figura 01. Imagem que contém o diagrama de componentes da aplicação.</figcaption>

![Subsistema Autenticação](../../assets/images/subsistema_autenticacao.png)
<figcaption>Figura 02. Imagem que contém o subsistema Autenticação do diagrama de componentes da aplicação.</figcaption>

![Subsistema Lanchonete](../../assets/images/subsistema_lanchonete.png)
<figcaption>Figura 03. Imagem que contém o subsistema Lanchonete do diagrama de componentes da aplicação.</figcaption>

![Subsistema Pedido](../../assets/images/subsistema_pedido.png)
<figcaption>Figura 04. Imagem que contém o subsistema Pedido do diagrama de componentes da aplicação.</figcaption>

![Subsistema Cardápio](../../assets/images/subsistema_cardapio.png)
<figcaption>Figura 05. Imagem que contém o subsistema Cardápio do diagrama de componentes da aplicação.</figcaption>

## Bibliografia

DIAGRAMAS de Componentes. In: Rational Software Architect Standard Edition. Disponível em: https://www.ibm.com/docs/pt-br/rsas/7.5.0?topic=services-component-diagrams. Acesso em: 16 fev. 2022.

Lucidchart. O que é diagrama de componentes UML?. Disponível em: <https://www.lucidchart.com/pages/pt/diagrama-de-componentes-uml>. Acesso em: 16 fev. 2022.
