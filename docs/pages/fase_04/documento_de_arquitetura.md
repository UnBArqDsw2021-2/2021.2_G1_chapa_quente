# Documento de Arquitetura de Software - DAS

## Versionamento

| Versão |    Data    |            Modificação             |                Autor                |                             Revisor                             |
| ------ | :--------: | :--------------------------------: | :---------------------------------: | :-------------------------------------------------------------: |
| 1.0    | 09/04/2022 |        Criação do Documento        |         Giulia Lobo Barros e Guilherme Daniel Fernandes          |                  A definir                |
| 1.1    | 11/04/2022 |        Alteração de tópicos da estrutura do documento        |         Giulia Lobo Barros e Guilherme Daniel Fernandes          |                  A definir                |
| 1.2    | 12/04/2022 |        Adição das metas e restrições        |         Giulia Lobo Barros e Pedro Lima          |                  A definir                |
| 1.3    | 12/04/2022 |        Adição dos casos de uso        |         Giulia Lobo Barros e Philipe Serafim          |                  A definir                |
| 1.4    | 13/04/2022 |        Adição da visão de processos        |         Giulia Lobo Barros e Murilo Gomes          |                  A definir                |
| 1.5    | 13/04/2022 |        Adição de frames para visualização dos diagramas        |         Giulia Lobo Barros e Dafne Moretti          |                  A definir                      |
| 1.6    | 15/04/2022 |    Adição da Visão de Dados   |  Liverson Paulo e Rodrigo Lima  | A definir |
| 1.7 | 15/04/2022 | Adição da Visão de Implementação| Rodrigo Lima e Lucas Andrade | A definir |

## 1. Introdução

### 1.1. Objetivo

### 1.2. Escopo

### 1.3. Definições, Acrônimos e Abreviações

### 1.4. Referências

### 1.5. Visão Geral

## 2. Representação Arquitetural

### 2.1. Padrões

### 2.2. Tecnologias

#### 2.2.1. Banco de Dados

#### 2.2.2. Backend

#### 2.2.3. Frontend

## 3. Metas Arquiteturais e Restrições da Arquitetura

### 3.1. Restrições

|  Restrições   | Descrição  |
| :-----------: | :--------: |
| Conectividade |   É necessário estabelecer conexão com internet para utilização do Chapa Quente.   |
| Idioma        |   O sistema deve ser desenvolvido para o idioma português do Brasil.   |
| Público       |   O aplicativo deve ser desenvolvido para administradores, entregadores e clientes da Lanchonete Chapa Quente.   |
| Plataforma    |   A aplicação terá suporte para browsers no computador, tablet e celular.   |  
| Prazo Final   |   	O escopo proposto deve ser terminado até o dia 18/04/2022.   |

### 3.2. Requisitos Não Funcionais

|      Metas       | Descrição  |
| :--------------: | :--------: |
|     Deploy       | A aplicação deve possuir deploy automatizado. |
| Escalabilidade   | O código deve ser estruturado e escalável o suficiente para estar aberto a futuras evoluções com o crescimento do projeto e a futuros usuários aderentes à aplicação. |
| Manutenibilidade | O código e as documentações realizadas pelo grupo devem estar em um nível de qualidade, seguindo os padrões de projeto e bibliografia, onde a sua manutenção seja fácil de ser realizada. |
| Responsividade   | A aplicação deve ser responsiva e se adaptar a todas as interfaces sem que haja comprometimento nas funções da aplicação. |
| Segurança        | O sistema deve ser seguro e lidar com os dados confidenciais dos usuários com segurança. |
| Suportabilidade  | Deve ser possível utilizar a plataforma em qualquer navegador web. |
| Usabilidade      | O sistema deve ser intuitivo e de simples uso, de forma que a curva de aprendizado para utilização dele seja fácil e clara. |

## 4. Visão Lógica

### 4.1. Visão Geral

### 4.2. Pacotes de Design Significativos do Ponto de Vista da Arquitetura

## 5. Visão de Casos de Uso

Nesta seção, apresentamos a **visão de casos de uso**, definida como aquela que descreve um modelo de alto nível com significância em relação às funcionalidades do sistema. Normalmente, essa visão é representada pelo **diagrama de casos de uso**, que auxilia no entendimento das relações entre atores do sistema, descrevendo cenários de uso da aplicação.

### 5.1. Diagrama de Casos de Uso (Já estará com as alterações necessárias feitas)

Esse diagrama já foi desenvolvido pela equipe para uma entrega anterior, juntamente com a descrição de todos os seus casos de uso e pode ser facilmente acessado por meio do documento atual: [Diagrama de Casos de Uso](pages/fase_01/casos_de_uso.md).

<center><iframe height="600" width="700" src="https://unbarqdsw2021-2.github.io/2021.2_G1_chapa_quente/#/pages/fase_01/casos_de_uso?id=diagrama-de-casos-de-uso"></iframe>
</center>

*Obs.:* Importante destacar que todas as alterações necessárias relacionadas a esse diagrama já foram feitas para a entrega final.

## 6. Visão de Implementação
A Visão de Implementação procura mostrar como o sistema será desenvolvido e organizado. Pode-se então utilizar o Diagrama de Componetes para tal demonstração.

### 6.1. Diagrama de Componentes

Esse diagrama já está disponível no escopo do nosso projeto, basta acessar: [Diagrama de Componentes](pages/fase_02/diagrama_de_componentes.md).
<center><iframe height="600" width="700" src="https://unbarqdsw2021-2.github.io/2021.2_G1_chapa_quente/#/pages/fase_02/diagrama_de_componentes?id=diagrama-de-componentes"></iframe>
</center>

## 7. Visão de Implantação

## 8. Visão de Processos

A **visão de processos** descreve como o sistema de tempo-de-execução é estruturado na forma de um conjunto de elementos que têm interações e comportamento de tempo-de-execução. A estrutura de tempo-de-execução normalmente tem pouca semelhança com a estrutura de código. Além disso, permite a visualização das partes dinâmicas do sistema, onde são evidenciados os processos, as threads e as interações entre elas.

Nessa visão, nós podemos ter 2 representações que auxiliam em seu entendimento:

### 8.1. Diagrama de Atividades (Já estará com as alterações necessárias feitas)

Esse diagrama já está disponível no escopo do nosso projeto, basta acessar: [Diagrama de Atividades](pages/fase_02/diagrama_de_atividade.md).

<center><iframe height="600" width="700" src="https://unbarqdsw2021-2.github.io/2021.2_G1_chapa_quente/#/pages/fase_02/diagrama_de_atividade?id=diagrama-de-atividade"></iframe>
</center>

*Obs.:* Importante destacar que todas as alterações necessárias relacionadas a esse diagrama já foram feitas para a entrega final.

### 8.2. Diagrama de Sequência (Já estará com as alterações necessárias feitas)

Esse diagrama já está disponível no escopo do nosso projeto, basta acessar: [Diagrama de Sequência](pages/fase_02/diagrama_de_sequencia.md).

<center><iframe height="600" width="700" src="https://unbarqdsw2021-2.github.io/2021.2_G1_chapa_quente/#/pages/fase_02/diagrama_de_sequencia?id=diagrama-de-sequ%c3%aancia"></iframe>
</center>

*Obs.:* Importante destacar que todas as alterações necessárias relacionadas a esse diagrama já foram feitas para a entrega final.

## 9. Visão de Dados
Visão de Dados é um tópico que se dispõe a mostrar quais são os dados persistentes na aplicação, geralmente utiliza-se ferramentas como um Modelo Entidade-Relacionamento e/ou Diagrama Entidade-Relacionamento para isso, entretanto no projeto Chapa Quente foi utilizado um sistema não-relacional, tornando essas ferramentas inoportunas nesse contexto. Como foi utilizado o MongoDB, que é um banco de dados orientado a documentos JSON, foi preferivel utilizar um sistema que mostra os objetos da camada "Model", pois esses são os objetos que são mapeados para a camada persistente, ou seja, para o banco de dados.

Para melhor visualização, as tabelas que mostram os objetos supracitados foram dividos em duas imagens:
### Imagem 1:
![Visao de dados - pedido](../../assets/images/visao_de_dados_pedido.png)

### Imagem 2:  
![Visao de dados - pessoa](../../assets/images/visao_de_dados_pessoa.png)

## 10. Tamanho e Desempenho

## 11. Qualidade

## Conclusão

## Bibliografia

- 