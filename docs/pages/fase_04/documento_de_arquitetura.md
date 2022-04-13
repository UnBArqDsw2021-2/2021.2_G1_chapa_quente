# Documento de Arquitetura de Software - DAS

## Versionamento

| Versão |    Data    |            Modificação             |                Autor                |                             Revisor                             |
| ------ | :--------: | :--------------------------------: | :---------------------------------: | :-------------------------------------------------------------: |
| 1.0    | 09/04/2022 |        Criação do Documento        |         Giulia Lobo Barros e Guilherme Daniel Fernandes          |                  A definir                |
| 1.1    | 11/04/2022 |        Alteração de tópicos da estrutura do documento        |         Giulia Lobo Barros e Guilherme Daniel Fernandes          |                  A definir                |
| 1.2    | 12/04/2022 |        Adição das metas e restrições        |         Giulia Lobo Barros e Pedro Lima          |                  A definir                |
| 1.3    | 12/04/2022 |        Adição dos casos de uso        |         Giulia Lobo Barros e Philipe Serafim          |                  A definir                |

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

Esse diagrama já foi desenvolvido pela equipe para uma entrega anterior, juntamente com a descrição de todos os seus casos de uso e pode ser facilmente acessado por meio do documento atual: [Diagrama de Casos de Uso](pages/fase_01/casos_de_uso.md). 

### 5.1. Diagrama de Casos de Uso

## 6. Visão de Implementação

### 6.1. Diagrama de Componentes

## 7. Visão de Implantação

## 8. Visão de Processos

## 9. Visão de Dados

## 10. Tamanho e Desempenho

## 11. Qualidade

## Conclusão

Este padrão pode ser bem valioso no contexto de algumas aplicações, pois ajudará com classes que possuem a mesma base, porém têm algumas particularidades diferentes umas das outras, diminuindo, assim, a repetição exacerbada, além de também, colaborar para uma melhor eficiência do sistema em geral.

Apesar de ser útil, o Template Method não deve ser implementado no projeto Chapa Quente, visto que adicionaria uma camada a mais desnecessária de abstração, sendo que a maioria dos problemas que o Template Method resolve já serão resolvidos por outros padrões que serão implementados.

## Bibliografia

- REFACTORING GURU. TEMPLATE METHOD. Disponível em: https://refactoring.guru/pt-br/design-patterns/template-method Acesso em: 23/02/2022

- GITBOOK. PADRÃO TEMPLATE METHOD. Disponível em: https://diogomoreira.gitbook.io/padroes-de-projeto/padroes-gof-comportamentais/padrao-template-method Acesso em: 23/02/2022

- DEVMEDIA. DESIGN PATTERNS: PADRÕES "GOF". Disponível em: https://www.devmedia.com.br/design-patterns-padroes-gof/16781 Acesso em: 23/02/2022

- GALDINO, Gabriel. AS VANTAGENS E DESVANTAGENS DA APLICAÇÃO DE PADRÕES DE PROJETO. Disponível em: https://pt.slideshare.net/gawiga/as-vantagens-e-desvantagens-da-aplicao-de-padres-de-projeto#:~:text=Template%20Method%20VANTAGEM%20%E2%80%A2%20Reutiliza%2Dse%20o%20c%C3%B3digo.&text=Conduz%20a%20uma%20estrutura%20de,de%20chamar%20a%20opera%C3%A7%C3%A3o%20herdada. Acesso em: 23/02/2022

- DOFACTORY. JAVASCRIPT TEMPLATE METHOD. Disponível em: https://www.dofactory.com/javascript/design-patterns/template-method Acesso em: 23/02/2022