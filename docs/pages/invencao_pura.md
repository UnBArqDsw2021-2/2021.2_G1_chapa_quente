# Nome do Artefato

## Versionamento

| Versão |    Data    |     Modificação      | Autor | Revisor |
| ------ | :--------: | :------------------: | :---: | :-----: |
| 1.0    | 03/03/2022 | Criação do Documento |  Dafne Moretti Moreira     |         |

## Introdução

O padrão GRASP Invenção Pura aborda o conceito de criação de uma classe "fictícia" ou inventada que não representa um conceito de domínio do problema para favorecer o baixo acoplamento, alta coesão e reutilização. As classes criadas a partir da Invenção Pura têm o funcionamento prestadoras de serviços e por isso, muitas vezes, são discutidas como "serviços" no software

Abaixo é possível visualizar um exemplo de GRASP de Invenção Pura sendo utilizado.

(imagem de invenção pura 1)

## Conclusão

Ao verificar o diagrama de classe do projeto, foi possível perceber que esse GRASP será bastante utilizado quando forem criadas classes por invenção do grupo, visando facilitar a reutilização, uma vez que a classe criada nesse padrão agrupa métodos utilizados por muitas classes.

Por exemplo, para criar uma classe geral que englobará alguns métodos que na versão atual do diagrama constam em diversas classes (bebida, sanduiche, acompanhamento e sobremesa) repetidamente.


## Bibliografia
http://www.facom.ufu.br/~bacala/ESOF/05a-Padr%C3%B5es%20GRASP.pdf

https://medium.com/@leandrovboas/padr%C3%B5es-grasp-padr%C3%B5es-de-atribuir-responsabilidades-1ae4351eb204

http://nelsonbassetto.com/blog/tags/grasp/

http://mykportela.blogspot.com/2008/06/aulas-28-e-29.html

https://slideplayer.com/slide/9635829/