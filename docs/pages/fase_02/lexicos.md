# Léxicos

## Versionamento

| Versão | Data       | Modificação          | Autor                        |Revisor|
| ------ | :--------: | :------------------: | :--------------------------: | :---: |
| 1.0    | 10/02/2022 | Criação do Documento | Murilo Gomes de Souza | Giulia Lobo |

<!-- NÃO ESQUECER DE ADICIONAR AO "/_sidebar.md" -->

## Introdução

O léxico é uma técnica que consiste em descrever os símbolos de uma linguagem específica. Para o contexto de Engenharia de Software, o objetivo é identificar frases e palavras específicas do contexto da aplicação sobre estudo. Cada símbolo é descrito com **noção** e **impacto**:

* **Noção** é o que significa o símbolo dentro da aplicação (denotação)
* **Impacto** descreve o efeito/uso/ocorrência do símbolo na aplicação (conotação)

Os símbolos podem possuir 4 classificações diferentes: _objeto_, _estado_, _sujeito_ e _verbo_.

## Metodologia

Para a criação desse documento foram criados vários léxicos relacionados com o contexto do site Chapa Quente em forma de tabelas contendo as seguintes informações: Nome, Noção, Impacto, Classificação e Sinônimos.

### Índice

* [L01 - Adicional](pages/fase_02/lexicos#adicional)
* [L02 - Avaliação](pages/fase_02/lexicos#avaliacao)
* [L03 - Busca](pages/fase_02/lexicos#busca)
* [L04 - Cadastro](pages/fase_02/lexicos#cadastro)
* [L05 - Cardápio](pages/fase_02/lexicos#cardapio)
* [L06 - Carrinho](pages/fase_02/lexicos#carrinho)
* [L07 - Categoria](pages/fase_02/lexicos#categoria)
* [L08 - Chapa Quente](pages/fase_02/lexicos#chapa_quente)
* [L09 - Código de Confirmação](pages/fase_02/lexicos#codigo_confirmacao)
* [L10 - Confirmar Pedido](pages/fase_02/lexicos#confirmar_pedido)
* [L11 - Cozinheiro](pages/fase_02/lexicos#cozinheiro)
* [L12 - Cupom de Desconto](pages/fase_02/lexicos#cupom_desconto)
* [L13 - Efetuar Pagamento](pages/fase_02/lexicos#efetuar_pagamento)
* [L14 - Endereço](pages/fase_02/lexicos#endereco)
* [L15 - Entregador](pages/fase_02/lexicos#entregador)
* [L16 - Funcionário](pages/fase_02/lexicos#funcionario)
* [L17 - Lanche](pages/fase_02/lexicos#lanche)
* [L18 - Lanchonete](pages/fase_02/lexicos#lanchonete)
* [L19 - Localização](pages/fase_02/lexicos#localizacao)
* [L20 - Pedido](pages/fase_02/lexicos#pedido)
* [L21 - Rastrear](pages/fase_02/lexicos#rastrear)
* [L22 - Retirada no Local](pages/fase_02/lexicos#retirada_local)
* [L23 - Site](pages/fase_02/lexicos#site)
* [L24 - Status do Pedido](pages/fase_02/lexicos#status)
* [L25 - Usuário](pages/fase_02/lexicos#usuario)

<span id="adicional"></span>

### L01 - Adicional

| Nome          | Adicional |
| ------------- | --------- |
| Noção         | Acompanhamento, bebida, sobremesa ou quantidade extra de algum ingrediente oferecido ao [usuário](pages/fase_02/lexicos#usuario) junto ao [lanche](pages/fase_02/lexicos#lanche) relacionado |
| Impacto(s)    | 1) Os adicionais são oferecidos junto com o [lanche](pages/fase_02/lexicos#lanche). <br> 2) O [usuário](pages/fase_02/lexicos#usuario) pode acrescentar adicionais ao [lanche](pages/fase_02/lexicos#lanche). |
| Classificação | Objeto |
| Sinônimo(s)   | Acompanhamento, extra |

<span id="avaliacao"></span>

### L02 - Avaliação

| Nome          | Avaliação |
| ------------- | --------- |
| Noção         | Opinião do [usuário](pages/fase_02/lexicos#usuario) sobre um [pedido](pages/fase_02/lexicos#pedido) específico feito por ele |
| Impacto(s)    | 1) Os [funcionários](pages/fase_02/lexicos#funcionario) da [lanchonete](pages/fase_02/lexicos#lanchonete) conseguem ver as avaliações dos [usuários](pages/fase_02/lexicos#usuario). <br> 2) Os [usuários](pages/fase_02/lexicos#usuario) conseguem avaliar [pedidos](pages/fase_02/lexicos#pedido) ao receber ou cancelar um [pedido](pages/fase_02/lexicos#pedido). <br> 3) Os [usuários](pages/fase_02/lexicos#usuario) devem conseguir ver as avaliações feitar por outros [usuários](pages/fase_02/lexicos#usuario). |
| Classificação | Objeto |
| Sinônimo(s)   | Opinião |

<span id="busca"></span>

### L03 - Busca

| Nome          | Busca |
| ------------- | --------- |
| Noção         | Pesquisa sobre algum item específico dentro do [site](pages/fase_02/lexicos#site) e do contexto do [usuário](pages/fase_02/lexicos#usuario) atual |
| Impacto(s)    | 1) Os [funcionários](pages/fase_02/lexicos#funcionario) da [lanchonete](pages/fase_02/lexicos#lanchonete) conseguem buscar entre os [usuários](pages/fase_02/lexicos#usuario). <br> 2) Os [usuários](pages/fase_02/lexicos#usuario) conseguem buscar entre os [lanches](pages/fase_02/lexicos#lanche) existentes no [cardápio](pages/fase_02/lexicos#cardapio). |
| Classificação | Objeto |
| Sinônimo(s)   | Pesquisa |

<span id="cadastro"></span>

### L04 - Cadastro

| Nome          | Cadastro |
| ------------- | --------- |
| Noção         | Registro do [usuário](pages/fase_02/lexicos#usuario) dentro do [site](pages/fase_02/lexicos#site) |
| Impacto(s)    | 1) Os [usuários](pages/fase_02/lexicos#usuario) cadastram suas informações pessoais dentro do [site](pages/fase_02/lexicos#site) <br> |
| Classificação | Objeto |
| Sinônimo(s)   | Registro |

<span id="cardapio"></span>

### L05 - Cardápio

| Nome          | Cardápio |
| ------------- | --------- |
| Noção         | Lista com os [lanches](pages/fase_02/lexicos#lanche) disponíveis da [lanchonete](pages/fase_02/lexicos#lanchonete) [Chapa Quente](pages/fase_02/lexicos#chapa_quente) |
| Impacto(s)    | 1) Os [usuários](pages/fase_02/lexicos#usuario) visualizam o cardápio <br> 2) Os [usuários](pages/fase_02/lexicos#usuario) adicionam [lanches](pages/fase_02/lexicos#lanche) do cardápio ao [carrinho](pages/fase_02/lexicos#carrinho) <br> 3) Os [funcionários](pages/fase_02/lexicos#funcionario) atualizam o cardápio de tempos em tempos |
| Classificação | Objeto |
| Sinônimo(s)   | Lista |

<span id="carrinho"></span>

### L06 - Carrinho

| Nome          | Carrinho |
| ------------- | --------- |
| Noção         | Onde se encontram todos os [lanches](pages/fase_02/lexicos#lanche) escolhidos pelo [usuário](pages/fase_02/lexicos#usuario) para fazer o [pedido](pages/fase_02/lexicos#pedido) |
| Impacto(s)    | 1) Os [usuários](pages/fase_02/lexicos#usuario) adicionam [lanches](pages/fase_02/lexicos#lanche) ao carrinho <br> 2) Os [usuários](pages/fase_02/lexicos#usuario) removem [lanches](pages/fase_02/lexicos#lanche) do carrinho <br> 3) Os [usuários](pages/fase_02/lexicos#usuario) fazem o [pedido](pages/fase_02/lexicos#pedido) baseado no conteúdo do carrinho |
| Classificação | Objeto |
| Sinônimo(s)   |  |

<span id="categoria"></span>

### L07 - Categoria

| Nome          | Categoria |
| ------------- | --------- |
| Noção         | Forma em que os [lanches](pages/fase_02/lexicos#lanche) do [cardápio](pages/fase_02/lexicos#cardapio) são organizados baseados em suas características |
| Impacto(s)    | 1) Os [usuários](pages/fase_02/lexicos#usuario) conseguem filtrar o [cardápio](pages/fase_02/lexicos#cardapio) por categoria <br> 2) Os [funcionários](pages/fase_02/lexicos#funcionario) conseguem associar um [lanche](pages/fase_02/lexicos#lanche) a uma categoria |
| Classificação | Objeto |
| Sinônimo(s)   | Tipo |

<span id="chapa_quente"></span>

### L08 - Chapa Quente

| Nome          | Chapa Quente |
| ------------- | --------- |
| Noção         | Nome do [site](pages/fase_02/lexicos#site) e da [lanchonete](pages/fase_02/lexicos#lanchonete) |
| Impacto(s)    | 1) Os usuários conseguem acessar o [site](pages/fase_02/lexicos#site) Chapa Quente para fazer [pedidos](pages/fase_02/lexicos#pedido). <br> 2) Os [funcionários](pages/fase_02/lexicos#funcionario) da lanchonete Chapa Quente conseguem acessar o [site](pages/fase_02/lexicos#site) para monitorar [pedidos](pages/fase_02/lexicos#pedido), usuários e [cardápio](pages/fase_02/lexicos#cardapio). |
| Classificação | Objeto |
| Sinônimo(s)   | |

<span id="codigo_confirmacao"></span>

### L09 - Código de Confirmação


| Nome          | Código de Confirmação |
| ------------- | --------- |
| Noção         | Código usado para a confirmação do recebimento de um [pedido](pages/fase_02/lexicos#pedido) |
| Impacto(s)    | 1) O usuário recebe o código de confirmação ao [confirmar pedido](pages/fase_02/lexicos#confirmar_pedido) <br> 2) O [entregador](pages/fase_02/lexicos#entregador) confirma com o usuário o código de confirmação no ato de entrega <br> 3) O usuário informa o código de confirmação ao fazer [retirada no local](pages/fase_02/lexicos#retirada_local) do [pedido](pages/fase_02/lexicos#pedido) |
| Classificação | Objeto |
| Sinônimo(s)   | |

<span id="confirmar_pedido"></span>

### L10 - Confirmar Pedido

| Nome          | Confirmar Pedido |
| ------------- | --------- |
| Noção         | Quando um usuário decide sobre tudo o que quer no seu [pedido](pages/fase_02/lexicos#pedido) e confirma |
| Impacto(s)    | 1) O usuário consegue confirmar pedido baseado nos itens que se encontram no seu [carrinho](pages/fase_02/lexicos#carrinho). |
| Classificação | Verbo |
| Sinônimo(s)   | Realizar Pedido |

<span id="cozinheiro"></span>

### L11 - Cozinheiro

| Nome          | Cozinheiro |
| ------------- | --------- |
| Noção         | Funcionário da [lanchonete](pages/fase_02/lexicos#lanchonete) [Chapa Quente](pages/fase_02/lexicos#chapa_quente) responsável por preparar os [pedidos](pages/fase_02/lexicos#pedido) que chegam pelo [site](pages/fase_02/lexicos#site) |
| Impacto(s)    | 1) Os cozinheiros recebem os [pedidos](pages/fase_02/lexicos#pedido) feitos pelo [site](pages/fase_02/lexicos#site). <br> 2) Os cozinheiros preparam os [pedidos](pages/fase_02/lexicos#pedido) recebidos. <br> 3) Os cozinheiros notificam o [entregador](pages/fase_02/lexicos#entregador) quando o [pedido](pages/fase_02/lexicos#pedido) está pronto |
| Classificação | Sujeito |
| Sinônimo(s)   | |

<span id="cupom_desconto"></span>

### L12 - Cupom de Desconto

| Nome          | Cupom de Desconto |
| ------------- | --------- |
| Noção         | Códigos que permitem que o usuário tenha desconto em algum [pedido](pages/fase_02/lexicos#pedido) feito |
| Impacto(s)    | 1) Os [funcionários](pages/fase_02/lexicos#funcionario) disponibilizam cupons de desconto no [site](pages/fase_02/lexicos#site). <br> 2) Os usuários utilizam os cupons de desconto na hora de [confirmarem o pedido](pages/fase_02/lexicos#confirmar_pedido) |
| Classificação | Objeto |
| Sinônimo(s)   | |

<span id="efetuar_pagamento"></span>

### L13 - Efetuar Pagamento 

| Nome          | Efetuar Pagamento |
| ------------- | --------- |
| Noção         | Quando o usuário realiza o pagamento após [confirmar pedido](pages/fase_02/lexicos#confirmar_pedido) |
| Impacto(s)    | 1) O usuário efetua o pagamento via PIX pelo [site](pages/fase_02/lexicos#site) <br> 2) O usuário efetua o pagamento na entrega do [pedido](pages/fase_02/lexicos#pedido) |
| Classificação | Verbo |
| Sinônimo(s)   | Realizar Pagamento |

<span id="endereco"></span>

### L14 - Endereço

| Nome          | Endereço |
| ------------- | --------- |
| Noção         | Local que o usuário registra para a entrega de [lanches](pages/fase_02/lexicos#lanche) |
| Impacto(s)    | 1) O usuário registra seu endereço quando o [cadastro](pages/fase_02/lexicos#cadastro) é feito. <br> 2) O [entregador](pages/fase_02/lexicos#entregador) acessa as informações do endereço do usuário que fez o [pedido](pages/fase_02/lexicos#pedido) a ser entregue |
| Classificação | Objeto |
| Sinônimo(s)   | Local |

<span id="entregador"></span>

### L15 - Entregador

| Nome          | Entregador |
| ------------- | --------- |
| Noção         | Pessoa responsável por entregar os [lanches](pages/fase_02/lexicos#lanche) aos usuários |
| Impacto(s)    | 1) O entregador visualiza quando um [pedido](pages/fase_02/lexicos#pedido) é preparado pelo [site](pages/fase_02/lexicos#site) <br> 2) O entregador visualiza as informações do [endereço](pages/fase_02/lexicos#endereco) do usuário <br> 3) O entregador entrega o [pedido](pages/fase_02/lexicos#pedido) ao usuário e atualiza o [status do pedido](pages/fase_02/lexicos#status) |
| Classificação | Sujeito |
| Sinônimo(s)   | |

<span id="funcionario"></span>

### L16 - Funcionário

| Nome          | Funcionário |
| ------------- | --------- |
| Noção         | Pessoa que trabalha diretamente na [lanchonete](pages/fase_02/lexicos#lanchonete) |
| Impacto(s)    | 1) O funcionário pode ver as informações dos usuários <br> 2) O funcionário pode ver informações de [pedidos](pages/fase_02/lexicos#pedido). <br> 3) O funcionário consegue atualizar o [cardápio](pages/fase_02/lexicos#cardapio). |
| Classificação | Sujeito |
| Sinônimo(s)   | Trabalhador |

<span id="lanche"></span>

### L17 - Lanche

| Nome          | Lanche |
| ------------- | --------- |
| Noção         | Opções de refeição oferecidas no [cardápio](pages/fase_02/lexicos#cardapio) da [lanchonete](pages/fase_02/lexicos#lanchonete) |
| Impacto(s)    | 1) O usuário adiciona lanches ao [carrinho](pages/fase_02/lexicos#carrinho) <br> 2) Os lanches são organizados em [categoria](pages/fase_02/lexicos#categoria) <br> 3) O [funcionário](pages/fase_02/lexicos#funcionario) retira ou adiciona lanches ao [cardápio](pages/fase_02/lexicos#cardapio). |
| Classificação | Objeto |
| Sinônimo(s)   | Prato |

<span id="lanchonete"></span>

### L18 - Lanchonete

| Nome          | Lanchonete |
| ------------- | --------- |
| Noção         | Tipo de estabelecimento onde são preparados os [lanches](pages/fase_02/lexicos#lanche) |
| Impacto(s)    | 1) O usuário [retira](pages/fase_02/lexicos#retirada_local) [pedidos](pages/fase_02/lexicos#pedido) no local da lanchonete. <br> 2) O [entregador](pages/fase_02/lexicos#entregador) busca [pedidos](pages/fase_02/lexicos#pedido) na lanchonete. <br> 3) O [cozinheiro](pages/fase_02/lexicos#cozinheiro) prepara [pedidos](pages/fase_02/lexicos#pedido) dentro da lanchonete. |
| Classificação | Objeto |
| Sinônimo(s)   | |

<span id="localizacao"></span>

### L19 - Localização


| Nome          | Localização |
| ------------- | --------- |
| Noção         | Posição atualizada em tempo real do [entregador](pages/fase_02/lexicos#entregador) responsável por um [lanche](pages/fase_02/lexicos#lanche) |
| Impacto(s)    | 1) O [entregador](pages/fase_02/lexicos#entregador) compartilha sua localização com o usuário e com os [funcionários](pages/fase_02/lexicos#funcionario) do restaurante. <br> 2) O usuário pode [rastrear](pages/fase_02/lexicos#rastrear) a localização do [entregador](pages/fase_02/lexicos#entregador) responsável por um [pedido](pages/fase_02/lexicos#pedido). |
| Classificação | Objeto |
| Sinônimo(s)   | Posição |

<span id="pedido"></span>

### L20 - Pedido

| Nome          | Pedido |
| ------------- | --------- |
| Noção         | Escolha definitiva dos [lanches](pages/fase_02/lexicos#lanche) que foram adicionados ao [carrinho](pages/fase_02/lexicos#carrinho) |
| Impacto(s)    | 1) O usuário [confirma pedido](pages/fase_02/lexicos#confirmar_pedido) ao terminar de escolher seus [lanches](pages/fase_02/lexicos#lanche) <br> 2) Os [cozinheiros](pages/fase_02/lexicos#cozinheiro) preparam o pedido feito. <br> 3) O [entregador](pages/fase_02/lexicos#entregador) acessa as informações do pedido. |
| Classificação | Objeto |
| Sinônimo(s)   | |

<span id="rastrear"></span>

### L21 - Rastrear

| Nome          | Rastrear |
| ------------- | --------- |
| Noção         | Opção de acompanhar a [localização](pages/fase_02/lexicos#localizacao) do [entregador](pages/fase_02/lexicos#entregador) em tempo real |
| Impacto(s)    | 1) O usuário rastreia a [localização](pages/fase_02/lexicos#localizacao) do [entregador](pages/fase_02/lexicos#entregador) |
| Classificação | Verbo |
| Sinônimo(s)   | Acompanhar |

<span id="retirada_local"></span>

### L22 - Retirada no Local

| Nome          | Retirada no Local |
| ------------- | --------- |
| Noção         | Opção para um usuário retirar o [pedido](pages/fase_02/lexicos#pedido) diretamente na [lanchonete](pages/fase_02/lexicos#lanchonete) |
| Impacto(s)    | 1) O usuário escolhe a opção de retirada no local ao [confirmar pedido](pages/fase_02/lexicos#confirmar_pedido). <br> 2) O [cozinheiro](pages/fase_02/lexicos#cozinheiro) notifica que o [pedido](pages/fase_02/lexicos#pedido) está pronto para retirada |
| Classificação | Objeto |
| Sinônimo(s)   | |

<span id="site"></span>

### L23 - Site

| Nome          | Site |
| ------------- | --------- |
| Noção         | Plataforma de interação entre os usuários, [funcionários](pages/fase_02/lexicos#funcionario), [cozinheiros](pages/fase_02/lexicos#cozinheiro) e [entregadores](pages/fase_02/lexicos#entregador) com a [Chapa Quente](pages/fase_02/lexicos#chapa_quente) |
| Impacto(s)    | 1) O usuário acessa o site para fazer [pedidos](pages/fase_02/lexicos#pedido). <br> 2) O [funcionário](pages/fase_02/lexicos#funcionario) acessa o site para ver informações e/ou atualizar [cardápio](pages/fase_02/lexicos#cardapio). <br> 3) O [cozinheiro](pages/fase_02/lexicos#cozinheiro) acessa o site para ver informações sobre o [pedido](pages/fase_02/lexicos#pedido) e atualizar o [status do pedido](pages/fase_02/lexicos#status). <br> 4) O [entregador](pages/fase_02/lexicos#entregador) acessa o site para ver [pedidos](pages/fase_02/lexicos#pedido) prontos para entrega. |
| Classificação | Objeto |
| Sinônimo(s)   | |

<span id="status"></span>

### L24 - Status do Pedido

| Nome          | Status do Pedido |
| ------------- | --------- |
| Noção         | Estado no qual o [pedido](pages/fase_02/lexicos#pedido) se encontra atualmente |
| Impacto(s)    | 1) O [cozinheiro](pages/fase_02/lexicos#cozinheiro) atualiza o status de em espera para preparando. <br> 2) O [cozinheiro](pages/fase_02/lexicos#cozinheiro) atualiza o status de preparando para pronto para entrega/[retirada](pages/fase_02/lexicos#retirada_local). <br> 3) O [entregador](pages/fase_02/lexicos#entregador) atualiza o status de pronto para entrega para à caminho. <br> 4) O [entregador](pages/fase_02/lexicos#entregador) atualiza o status de à caminho para entregue. <br> 5) O usuário acompanha o status do pedido. |
| Classificação | Estado |
| Sinônimo(s)   | Estado |

<span id="usuario"></span>

### L25 - Usuário

| Nome          | Usuário |
| ------------- | --------- |
| Noção         | Pessoa que utiliza o [site](pages/fase_02/lexicos#site) para realizar [pedidos](pages/fase_02/lexicos#pedido) de [lanches](pages/fase_02/lexicos#lanche)  |
| Impacto(s)    | 1) O usuário realiza um [pedido](pages/fase_02/lexicos#pedido). <br> 2) O usuário navega pelo [site](pages/fase_02/lexicos#site). <br> 3) O usuário acompanha o status do pedido. <br> 4) O usuário [avalia](pages/fase_02/lexicos#avaliacao) [pedidos](pages/fase_02/lexicos#pedido) feitos. <br> 5) O usuário [cadastra](pages/fase_02/lexicos#cadastro) e atualiza suas informações. <br> 6) O usuário adiciona [lanches](pages/fase_02/lexicos#lanche) e [adicionais](pages/fase_02/lexicos#adicional) ao seu [carrinho](pages/fase_02/lexicos#carrinho). |
| Classificação | Sujeito |
| Sinônimo(s)   | Cliente |


## Bibliografia

SERRANO, Milene; Arquitetura e Desenho de Software - AULA - PROJETO E DESENHO DE SOFTWARE; Disponível em: https://aprender3.unb.br/pluginfile.php/1558828/mod_label/intro/Arquitetura%20e%20Desenho%20de%20software%20-%20Aula%20Projeto-DSW%20-%20Profa.%20Milene.pdf;