# GOF Criacional Multiton

## Versionamento

| Versão |    Data    |     Modificação      |              Autor              | Revisor |
| ------ | :--------: | :------------------: | :-----------------------------: | :-----: |
| 1.0    | 28/02/2022 | Criação do Documento | Philipe Serafim e Lucas Andrade |         |

<!-- NÃO ESQUECER DE ADICIONAR AO "/_sidebar.md" -->

## Introdução

Sendo uma extensão do Singleton, o Multiton tem por objetivo instanciar um número _n_ de objetos de uma determinada classe atribuindo uma chave identificadora para cada instanciação.

## Metodologia

O construtor do Multiton deve ser privado, afim de evitar que instanciações que não seriam criadas dentro do dicionário já estabelecido. Também deve existir, um método que retorne um objeto do dicionário a partir de uma chave identificadora passada como argumento.

![](../../assets/images/multiton.png)

<figcaption>Figura 1 - Classe multiton. (CARR)</figcaption>

## Conclusão

O acesso centralizado a partir da chave informada, permite com que o Multiton exerça diversos papeis em projetos distintos. Entretanto deve-se prestar atenção ao fato de que o Multiton nunca irá retornar um valor nulo, caso não exista instanciação para a chave indicada, uma nova instância será criada para a chave em questão, podendo causa um uso inesperado de memória.

## Bibliografia

CARR, Richard. **Multiton Design Pattern**. Disponível em: http://www.blackwasp.co.uk/multiton.aspx. Acessado em: 28/02/2022.
