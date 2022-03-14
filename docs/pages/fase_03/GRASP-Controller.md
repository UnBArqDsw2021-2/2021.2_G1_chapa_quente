# Controller

## Versionamento

| Versão | Data       | Modificação          | Autor                        |Revisor|
| ------ | :--------: | :------------------: | :--------------------------: | :---: |
| 1.0    | 24/02/2022 | Criação do Documento | Lucas Andrade e Philipe Serafim | Dafne Moretti  |

## Introdução

O padrão Controller, ou Controlador, delega a classes **não-visuais** o dever de responder, interpretar e validar as interações dos usuários, que ocorrem na camada de interface (UI), com o sistema, delegando as atribuições aos objetos. Esse padrão possui uma semelhança presente MVC (Model, View e Controller), onde o Controller funciona como uma ponte entre as camadas Model e View

É dito que os casos de uso são separados em controllers, dividindo as tarefas para cada classe, diminuindo as suas tarefas e responsabilidades, visando um baixo acoplamento. Dizemos que uma classe não-visual que possui muitas atribuições é considerada "inchada".

## Metodologia

![Interação Usuario com UI](./../../../assets/images/user-controller_interaction.png)
<figcaption style="text-align: center">Interação do usuario com a UI e o papel da Controller. Autores: Lucas Andrade</figcaption>

O exemplo mostra a interação do cliente com a interface de usuário (UI), e como a Controller funciona como uma ponte, fornecendo as funcionalidades da aplicação para serem exibidas aos usuários na UI.  

![Exemplos de Controller](./../../../assets/images/GRASP-Controller.png)
<figcaption style="text-align: center">Exemplo de controllers que estão dentro da ideia da aplicação. Autores: Lucas Andrade</figcaption>

Acima temos dois exemplos de Controllers, a responsável pelas atividades relacionadas aos usuários e uma relacionada ao menu da aplicação. Visando um baixo acoplamento, cada Controller deve possui poucas atribuições.

## Conclusão

Esse padrão funciona como uma camada, interpretando os eventos realizados na camada de interface. Uma controller bem implementada  facilita futuras manutenções no sistema. 

## Bibliografia

- SERRANO, Milene. AULA - GRASP_A - COMPLEMENTAR. Acesso em: 23 de fev. de 2022.
- GRASP – General Responsibility Assignment Software Patterns Explained. [S. l.], 8 abr. 2019. Disponível em: http://www.kamilgrzybek.com/design/grasp-explained/. Acesso em: 24 fev. 2022.