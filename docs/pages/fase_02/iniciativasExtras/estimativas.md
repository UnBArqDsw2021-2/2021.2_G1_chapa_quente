# Estimativas

## Versionamento

| Versão | Data       | Modificação          | Autor                        |Revisor|
| ------ | :--------: | :------------------: | :--------------------------: | :---: |
| 1.0    | 14/02/2022 | Criação do Documento | Giulia Lobo Barros | Murilo Gomes de Souza |

<!-- NÃO ESQUECER DE ADICIONAR AO "/_sidebar.md" -->

## Introdução

Uma das ações mais importantes para a execução de um projeto é fazer estimativas que ajudam na tomada de decisões de líderes e liderados. Essas estimativas podem ajudar a evitar grandes riscos, impedimentos e problemas no futuro e por isso são de grande valia.

Tendo isso em consideração, o grupo decidiu que as estimativas que mais fariam sentido para a equipe seriam as de **esforço**, **tempo** e **custo** e que elas ajudariam a mapear um projeto realista, não muito complexo, dentro do prazo acordado com a professora e de baixo custo.

Por esse motivo, o método que mais se encaixou com as propostas e acabou por ser o escolhido para auxiliar o projeto, foi o **Construtive Cost Model**, mais conhecido como **COCOMO**.

Esse método de estimativa do tempo e esforço de desenvolvimento de um software, que foi criado por Barry Boehm, por ser baseado no esforço de linhas de código de um software, auxilia na criação de deduções, constantes e atributos para cada situação e, por esse motivo, funciona muito bem para projetos de software em geral.

## Metodologia

Tendo o método **COCOMO** apresentado, podemos mostrar como será utilizado pelo grupo e detalhá-lo da seguinte forma:

* *Primeiramente, é importante destacar que o COCOMO é dividido em três implementações, sendo elas:*
    * **COCOMO Básico (Basic)**: Que computa o esforço e o custo de desenvolvimento considerando uma estimativa do tamanho do programa;
    * **COCOMO Intermediário (Intermediate)**: Que computa o esforço e o custo de desenvolvimento considerando uma estimativa do tamanho do programa e um conjunto de direcionadores de custo (avaliações subjetivas do produto, do hardware, do pessoal e dos atributos do projeto);
    * **COCOMO Detalhado (Detailed)**: Que, além das características do COCOMO intermediário, inclui uma avaliação do impacto dos direcionadores de custo sobre cada etapa do desenvolvimento.
* *Posteriomente, é necessário saber que ele também pode ser aplicado em três classes de projeto, que são:*
    * **Modo Orgânico**: projetos simples, relativamente pequenos, com conjuntos de requisitos não tão rígidos, com equipes pequenas e experientes;
    * **Modo Semidestacado**: projetos intermediários (em tamanho e complexidade), com alguns requisitos rígidos e outros não tão rígidos, com níveis mistos de experiência nas equipes;
    * **Modo Embutido**: projetos com conjunto rígido de restrições operacionais, tanto de hardware, quanto de software.
* *E, por fim, é necessário avaliar onde o projeto em questão se classifica e quais seriam as implementações e classes de projetos adequadas:*
    * Considerando que o objetivo da equipe é calcular esforço, tempo e custo, a opção de implementação que mais se encaixa é o **COCOMO Intermediário**;
    * E, tendo em vista que o time é formado de pessoas menos experientes e esse tende a ser um projeto de complexidade média, a classe de projeto mais adequada é o **Modo Semidestacado**.

### COCOMO Intermediário

Por conta da escolha feita, antes de partir para as estimativas, é importante apenas detalhar as categorias do COCOMO Intermediário e apresentar os direcionadores de custo associados a elas.

*As quatro categorias do COCOMO Intermediário são:*
* **Atributos do Produto** - Com os direcionadores de custo sendo:
    * Confiabilidade exigida do software;
    * Tamanho do banco de dados;
    * Complexidade do Produto.
* **Atributos do Hardware** - Com os direcionadores de custo sendo:
    * Restrições ao tempo de execução;
    * Restrições de Memória;
    * Volatilidade do ambiente de máquina virtual;
    * Tempo de Turnaround (tempo para completar o ciclo) exigido.
* **Atributos de Pessoal** - Com os direcionadores de custo sendo:
    * Capacidade do analista;
    * Experiência em aplicações;
    * Capacidade do programador;
    * Experiência em máquina virtual;
    * Experiência com a linguagem de programação.
* **Atributos do Projeto** - Com os direcionadores de custo sendo:
    * Uso de práticas modernas de programação;
    * Uso de ferramentas de software;
    * Cronograma exigido de desenvolvimento.

Essas categorias e direcionadores de custo são de fundamental importância para o início do cálculo das estimativas, pois servirão de base para uma classificação que dará os valores necessários, como será mostrado no próximo tópico.

## Conclusão

Com a finalização desse documento pode-se obter uma vasta lista de símbolos e palavras pertencentes ao contexto da aplicação que está sendo desenvolvida. Este documento pode servir para auxiliar o entendimento de membros da equipe e até mesmo usuários sobre a linguagem utilizada dentro do site Chapa Quente.

## Bibliografia

SERRANO, Milene; Arquitetura e Desenho de Software - AULA - PROJETO E DESENHO DE SOFTWARE; Disponível em: https://aprender3.unb.br/pluginfile.php/1558828/mod_label/intro/Arquitetura%20e%20Desenho%20de%20software%20-%20Aula%20Projeto-DSW%20-%20Profa.%20Milene.pdf;