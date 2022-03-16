# GOF Comportamental Visitor

## Versionamento

| Versão |    Data    |     Modificação      | Autor | Revisor |
| ------ | :--------: | :------------------: | :---: | :-----: |
| 1.0    | 25/02/2022 | Criação do Documento | Murilo Gomes e Rodrigo Lima | Lucas Andrade e Dafne Moretti |
| 1.1    | 16/03/2022 | Adição de Exemplo | Rodrigo Lima |     |

<!-- NÃO ESQUECER DE ADICIONAR AO "/_sidebar.md" -->

## Introdução
O Visitor é um padrão comportamental GOF que tem como objetivo executar e adicionar diferentes operações em objetos de tipos similares, sem ter que alterá-los. 

## Metodologia
Para a implementação é preciso:
 - Existir uma classe abstrata ou interface Visitante.
 - Existir uma classe abstrata ou interface Elemento.
 - Cada classe advinda de Visitante deve executar uma operação específica para cada classe baseada em Elemento.
 - Cada classe baseada em Elemento terá um método para aceitar um Visitante, em que dentro desse método o Visitante executa a sua operação baseada na classe concreta que o aceita.

![Exemplo de Visitor](../../assets/images/visitor.png)

<figcaption style="text-align: center"><a href="../../assets/images/visitor.png" >Figura 1 </a>: Exemplo de Visitor. Fonte: <a href="https://sourcemaking.com/design_patterns/visitor" > Visitor Design Pattern</a>. Acesso em: 25/02/2022 </figcaption>

Exemplo de código de Visitor em Java retirado de [link](https://refactoring.guru/pt-br/design-patterns/visitor):

```
interface Shape is
    method move(x, y)
    method draw()
    method accept(v: Visitor)

class Dot implements Shape is
    method accept(v: Visitor) is
        v.visitDot(this)

class Circle implements Shape is
    method accept(v: Visitor) is
        v.visitCircle(this)

class Rectangle implements Shape is
    method accept(v: Visitor) is
        v.visitRectangle(this)

class CompoundShape implements Shape is
    method accept(v: Visitor) is
        v.visitCompoundShape(this)

interface Visitor is
    method visitDot(d: Dot)
    method visitCircle(c: Circle)
    method visitRectangle(r: Rectangle)
    method visitCompoundShape(cs: CompoundShape)

class XMLExportVisitor implements Visitor is
    method visitDot(d: Dot) is

    method visitCircle(c: Circle) is

    method visitRectangle(r: Rectangle) is

    method visitCompoundShape(cs: CompoundShape) is

class Application is
    field allShapes: array of Shapes

    method export() is
        exportVisitor = new XMLExportVisitor()

        foreach (shape in allShapes) do
            shape.accept(exportVisitor)
```


## Conclusão
Analisando as características do Visitor, percebemos que, a princípio, não é um padrão que se encaixe no projeto Chapa Quente.

## Bibliografia
* SOURCE MAKING - Visitor Design Pattern. Disponível em: https://sourcemaking.com/design_patterns/visitor . Acesso em: 25 de fevereiro de 2022.
* REFACTORING GURU - Visitor. Disponível em: https://refactoring.guru/pt-br/design-patterns/visitor. Acessi em: 16 de março de 2022.
