# Estimativas

## Versionamento

| Versão |    Data    |       Modificação        |       Autor        |        Revisor        |
| ------ | :--------: | :----------------------: | :----------------: | :-------------------: |
| 1.0    | 14/02/2022 |   Criação do Documento   | Giulia Lobo Barros | Murilo Gomes de Souza |
| 1.1    | 15/02/2022 | Atualização do Documento | Giulia Lobo Barros |      Pedro Lima       |
| 1.2    | 16/02/2022 | Alterações na conclusão | Pedro Lima |      Giulia Lobo       |
| 1.3    | 17/02/2022 | Últimas alterações na conclusão | Giulia Lobo Barros |      Philipe Serafim, Murilo Gomes, Dafne Moretti e  Liverson Paulo      |

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
* *Posteriormente, é necessário saber que ele também pode ser aplicado em três classes de projeto, que são:*
    * **Modo Orgânico**: projetos simples, relativamente pequenos, com conjuntos de requisitos não tão rígidos, com equipes pequenas e experientes;
    * **Modo Semidestacado**: projetos intermediários (em tamanho e complexidade), com alguns requisitos rígidos e outros não tão rígidos, com níveis mistos de experiência nas equipes;
    * **Modo Embutido**: projetos com conjunto rígido de restrições operacionais, tanto de hardware, quanto de software.

*E que essas possuem coeficientes, representados pela tabela a seguir:*
<iframe src="https://docs.google.com/spreadsheets/d/1-C-9O3lvICseggB15Jxzs70cJPvZhf7DRFDAx0HvvOs/edit?usp=sharing" frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
<figcapction>Tabela 1 - Coeficientes do COCOMO Intermediário. Autora: Giulia Lobo</figcapction>

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

## Cálculo de Estimativas

Para calcular as estimativas em questão, o primeiro passo é conhecer a escala do **COCOMO Intermediário**.Essa escala possui valores conhecidos como *Multiplicadores de Esforço*, que, multiplicados dão origem ao *Fator de Ajustamento de Esforço*, que também faz parte do cálculo.

<iframe src="https://docs.google.com/spreadsheets/d/1lsQ5bkc4ZBrkWmeHm4pupgHVwWO-IIwQN0YuB98Lnug/edit?usp=sharing" frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
<figcapction>Tabela 2 - Direcionadores de Custo. Autora: Giulia Lobo</figcapction>

Tendo essa escala, o grupo pôde fazer uma avaliação do esforço de cada um dos atributos e definir os valores dos *Multiplicadores de Esforço* que utilizaríamos nos cálculos. Esses são os que estão destacados na tabela.

### Estimativa de Linhas de Código

Para iniciar o cálculo, o grupo se reuniu e definiu a estimativa de linhas de código que seriam utilizadas no projeto, com o intuito de colaborar para o cálculo da estimativa de esforço, posteriormente.

Sendo assim, a estimativa ficou da seguinte forma:

<iframe src="https://docs.google.com/spreadsheets/d/1Qi5qJ4j2LwqRw88c44caZQEb6-nHBVf8ucPGEpeemEY/edit?usp=sharing" frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
<figcapction>Tabela 3 - Estimativa de Linhas de Código. Autora: Giulia Lobo</figcapction>

De acordo com essa tabela e após discussão entre o grupo, podemos definir uma média total de linhas em, aproximadamente, **2128 linhas = 2128 Loc**, ou seja **2,128 KLoc**, que pode ser aproximado para **2 KLoc**.

### Estimativa de Esforço

Para calcular o esforço de um projeto de software, o cálculo que deve ser considerado é:

*E = a x S^b x fae*

Sendo as variáveis descritas como:

* **E:** Esforço aplicado (Pessoas/mês);
* **S:** Número estimado de linhas de código (1 Kloc = 1000 Loc);
* **a:** Coeficiente fornecido pela tabela de coeficientes das classes do COCOMO;
* **b:** Coeficiente fornecido pela tabela de coeficientes das classes do COCOMO;
* **fae:** Fator de Ajuste de Esforço.

Considerando essa fórmula, a escolha do **Modo Semidestacado**, os valores definidos na escala do **COCOMO Intermediário** e a estimativa de linhas de código feita pela equipe, podemos dizer que:

* **S** = 2 KLoc;
* **a** = 3,00;
* **b** = 1,12;
* **fae** = 1,40.

Substituindo na fórmula, temos:

*E = 3 x 2^1,12 x 1,40*

*E = 9,13 pessoas/mês*

Aproximando: 

*E = 9 pessoas/mês*

### Estimativa de Tempo

Já tendo obtido a estimativa de esforço para o projeto, podemos calcular a estimativa de tempo usando a fórmula:

*T = c x E^d*

Sendo as variáveis descritas como:

* **T:** Tempo de desenvolvimento (mês);
* **E:** Esforço aplicado (Pessoas/mês);
* **S:** Número estimado de linhas de código (1 Kloc = 1000 Loc);
* **c:** Coeficiente fornecido pela tabela de coeficientes das classes do COCOMO;
* **d:** Coeficiente fornecido pela tabela de coeficientes das classes do COCOMO.

Considerando essa fórmula, a escolha do **Modo Semidestacado**, os valores definidos na escala do **COCOMO Intermediário**, a estimativa de linhas de código feita pela equipe e o esforço encontrado, podemos dizer que:

* **E** = 9;
* **c** = 2,50;
* **d** = 0,35.

Substituindo na fórmula, temos:

*T = 2,50 x 9^0,35*

*T = 5,39 meses*

Aproximando: 

*T = 5 meses*

### Estimativa de Custo

A estimativa de custo deve levar em conta os custo de infraestrutura que o time vai ter para o desenvolvimento do projeto. Levando em conta as ferramentas que são necessárias ao cenário do projeto temos o seguinte parâmetro:

* **Internet**: Após um busca de mercado a *Internet Banda larga* da Vivo foi a que mais se adequou aos membros do grupo.
  
| Ferramenta | Quantidade | Valor unitário | Valor mensal | Tempo de uso necessário (meses) |  Total   |
| ---------- | :--------: | :------------: | :----------: | :-----------------------------: | :------: |
| Internet   |     10     |     112,00     |    99.99     |                5                | 6.119,50  |

Considerando que já foram definidas as estimativas de esforço e de tempo, podemos calcular a estimativa do custo da mão de obra:

*Custo = T(horas) x custo-aluno x E*

Sendo que:

* **T (horas)** = 1200 (considerando 8hs trabalhadas por dia);
* **custo-aluno** = 2,04;
* **E** = 9.

Substituindo na fórmula, temos:

*Custo = 1200 x 2,04 x 9*

*Custo = R$ 22.032,00*

Logo, temos:

|  Recursos   |  Valor   |
| :---------: | :------: |
|  Internet   | 6.119,50  |
| Mão de obra | 22.032,00 |
|  **Total**  | 28.151,50 |

## Conclusão

Com a estimativa de custo do projeto feitas é possível ter mais controle dos recursos que estão ao alcance do grupo e assim ter certa prudencia e maturidade no decorrer do desenvolvimento. Isso acaba por tornar o cenário do projeto mais proximo da realidade do mercado atual.

## Bibliografia

* SERRANO, Milene; Arquitetura e Desenho de Software - AULA - PROJETO E DESENHO DE SOFTWARE; Disponível em: https://aprender3.unb.br/pluginfile.php/1558828/mod_label/intro/Arquitetura%20e%20Desenho%20de%20software%20-%20Aula%20Projeto-DSW%20-%20Profa.%20Milene.pdf;

* MELLER, Maristela Corrêa. Modelos Para Estimar Custos De Software: Estudo Comparativo Com Softwares De Pequeno Porte. 2002. Disponível em: https://repositorio.ufsc.br/xmlui/handle/123456789/82351 Acessado em 16 de fevereiro de 2022.

* Estimativas de Custos e Esforços. Disponível em: https://unbarqdsw2021-1.github.io/2021.1_G5_ProjetoDonner/pages/base/estimativa_de_custos_esforços. Acessado em 15 de fevereiro de 2022.

* ESTIMATIVAS DE CUSTO. Disponível em: https://2019-2-arquitetura-desenho.github.io/wiki/dinamica_seminario_I/estimativas_de_custo. Acessado em 15 de fevereiro de 2022.

* Notebook Lenovo, Submarino. Disponível em: https://www.submarino.com.br/produto/3171318128?epar=zoom. Acessado em 15 de fevereiro de 2022.

* Internet Banda larga, Vivo. Disponível em: https://www.vivo.com.br/para-voce/produtos-e-servicos/para-casa/internet. Acessado em 15 de fevereiro de 2022.