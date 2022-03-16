# GRASP Indireção

## Versionamento

| Versão | Data       | Modificação          | Autor                        |Revisor|
| ------ | :--------: | :------------------: | :--------------------------: | :---: |
| 1.0    | 04/03/2022 | Criação do Documento | Liverson Paulo, Lucas Andrade | João Pedro |
| 1.1    | 16/03/2022 | Melhorias no texto   | Lucas Andrade | João Pedro Chaves |

## Introdução

O GRASP de Indireção busca promover um baixo acoplamento e alta coesão entre classes, visando assim facilitar o reuso dessas classes na aplicação, além de promover uma melhor organização de código. Para isso é utilizado uma objeto auxiliar, que será responsavel por manter uma comunicação entre as classes envolvidas.

## Metodologia

O objeto intermediário envolvido será responsável por um conjunto responsabilidades, e será aquele que realizará uma comunicação entre componentes ou serviços. Assim, evita-se um cenário em que as duas classes estejam diretamente acopladas.

O GRASP de Indireção possui uma certa similaridade com o GRASP de Invenção Pura, podemos inclusive dizer que o segundo é uma espécie de variação do primeiro. A principal distinção entre ambos é que o GRASP de Invenção Pura é, por definição, extremamente coeso em relação as suas responsabilidades.

## Conclusão

O padrão de indireção permite uma maior flexibilidade no código, e quando aplicado, permite a utilização de quase qualquer GoF, sem exigir a necessidade de se realizar um refatoramento nas classes. Este padrão, se aplicado de forma conjunta com o de invenção pura, tem o potencial de ser muito útil para a equipe no desenvolvimento do projeto, promovendo o baixo acomplamento e alta coesão no código, além de facilitar a aplicação de demais GoFs.

## Bibliografia

- GRASP Patterns: Polymorphism, Pure Fabrication, Indirection, Protected Variations. Disponível em: https://prog.world/grasp-patterns-polymorphism-pure-fabrication-indirection-protected-variations/.  Acesso em: 16/03/2022

- GRASP: 9 Must-Know Design Principles for Code. [S. l.], 23 jun. 2021. Disponível em: https://www.fluentcpp.com/2021/06/23/grasp-9-must-know-design-principles-for-code/. Acesso em: 16 mar. 2022.

- SOFTWARE patterns - GRASP (Part IX – Indirection). [S. l.]: Vishwas Sutar, 9 ago. 2011. Disponível em: https://www.dotnetfunda.com/articles/show/1578/software-patterns-grasp-part-ix-indirection. Acesso em: 16 mar. 2022.
