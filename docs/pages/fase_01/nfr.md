# NFR Framework

## Versionamento

| Versão |    Data    |                Modificação                 |              Autor               |     Revisor     |
| ------ | :--------: | :----------------------------------------: | :------------------------------: | :-------------: |
| 1.0    | 08/02/2022 |            Criação do Documento            | João Pedro Alves da Silva Chaves | Philipe Serafim |
| 1.1    | 10/02/2022 |   Adição da Introdução e imagens do NFR    | João Pedro Alves da Silva Chaves | Philipe Serafim |
| 1.2    | 10/02/2022 | Mudanças nos diagramas e adição da legenda | João Pedro Alves da Silva Chaves | Philipe Serafim |
| 1.3    | 10/02/2022 |  Adicionado os requisitos não funcionais   |         Philipe Serafim          |  Lucas Andrade  |
| 1.4    | 16/02/2022 |    Realizada as alterações solicitadas     |         Philipe Serafim          |  Lucas Andrade  |

<!-- NÃO ESQUECER DE ADICIONAR AO "/_sidebar.md" -->

## Introdução

O NFR Framework é uma técnica desenvolvida para modelagem de requisitos não funcionais, como o nome já sugere: Non Functional Requirements Framework, que traduzido significa framework de requisitos não funcionais. A abordagem utiliza SIGs(Softgoal Interdependency Graphs) que é uma representação gráfica proposta em (Chung et al. 2000) com objetivo de decompor os requisitos não funcionais em outros não funcionais visando alcançar uma operacionalização deles.

## Metodologia

### Legenda

![NFR Legenda](../../assets/images/NFR-Chapa-Quente-Legenda.drawio.png)

### NFR Geral

![NFR Geral](../../assets/images/NFR-Chapa-Quente-Geral.drawio.png)

### NFR Manutenibilidade

![NFR Manutenibilidade](../../assets/images/NFR-Chapa-Quente-Manutenibilidade.drawio.png)

#### Propagação

![NFR Manutenibilidade - Propagação](../../assets/images/NFR-Chapa-Quente-Manutenibilidade_Propagação.drawio.png)

### NFR Performance

![NFR Performance](../../assets/images/NFR-Chapa-Quente-Performance.drawio.png)

#### Propagação

![NFR Performance - Propagação](../../assets/images/NFR-Chapa-Quente-Performance_Propagação.drawio.png)

### NFR Segurança

![NFR Segurança](../../assets/images/NFR-Chapa-Quente-Segurança.drawio.png)

#### Propagação

![NFR Segurança - Propagação](../../assets/images/NFR-Chapa-Quente-Segurança_Propagação.drawio.png)

### NFR Usabilidade

![NFR Usabilidade](../../assets/images/NFR-Chapa-Quente-Usabilidade.drawio.png)

#### Propagação

![NFR Usabilidade - Propagação](../../assets/images/NFR-Chapa-Quente-Usabilidade_Propagação.drawio.png)

## Conclusão

Concluída a decomposição e propagação dos softgoals, foi possível identificar os seguintes requisitos não funcionais em seu nível mais técnico:

<table thead>
  <tr>
    <th >Requisito Não Funcional</th>
    <th >Operacionalização</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td  rowspan="3">Manutenibilidade</td>
    <td ><strong>RNF01</strong> - Componentes simples e reutilizáveis</td>
  </tr>
  <tr>
    <td ><strong>RNF02</strong> - Testes unitários</td>
  </tr>
  <tr>
    <td ><strong>RNF03</strong> - Ferramentas de análise de código</td>
  </tr>
  <tr>
    <td  rowspan="2">Performance</td>
    <td ><strong>RNF04</strong> - Interface leve</td>
  </tr>
  <tr>
    <td ><strong>RNF05</strong> - Banco de dados eficiente</td>
  </tr>
  <tr>
    <td  rowspan="3">Segurança</td>
    <td ><strong>RNF06</strong> - Criptografia dos dados</td>
  </tr>
  <tr>
    <td ><strong>RNF07</strong> - Enviar uma nova senha</td>
  </tr>
  <tr>
    <td ><strong>RNF08</strong> - Alteração de senha</td>
  </tr>
  <tr>
    <td  rowspan="3">Usabilidade</td>
    <td ><strong>RNF09</strong> - Funcionalidades intuitivas</td>
  </tr>
  <tr>
    <td ><strong>RNF10</strong> - Linguagem Simples</td>
  </tr>
  <tr>
    <td ><strong>RNF11</strong> - Fontes de texto grandes</td>
  </tr>
</tbody>
</table>

## Bibliografia

CHUNG, Lawrence; NIXON, Brian. Nixon, YU, Eric; MYLOPOULOS, John. "Non-Functional Requirements in Software Engineering". Springer US, 2000.

SILVA, Reinaldo Antônio da. NFR4ES: Um Catálogo de Requisitos Não-Funcionais para Sistemas Embarcados. 2019
