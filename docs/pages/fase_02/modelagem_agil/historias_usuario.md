# Histórias de usuário

## Versionamento

| Versão | Data       | Modificação          | Autor                        |Revisor|
| ------ | :--------: | :------------------: | :--------------------------: | :---: |
| 1.0    | 15/02/2022 | Criação do Documento |  Dafne Moretti Moreira |       |

## Introdução

Histórias de usuário são maneiras simplificadas, apresentadas em linguagem natural de representação de requisitos e que beneficiam a comunicação verbal e contém os testes de aceitação especificados pelos clientes. As histórias de usuário devem ser independentes, sucintas, estimáveis, negociáveis, testáveis e devem agregar valor para o negócio. 

## Metodologia

Para a criação das histórias de usuário do Chapa Quente, a PO assumiu a posição de representante do cliente para o time dos desenvolvedores, descrevendo os principais papéis do sistema como "Cozinheiro", "Chapa Quente", "Usuário" (que atua como cliente ou interessado no serviço oferecido) e por fim, "Entregador". 

As histórias foram separadas por ID para facilitar a rastreabilidade. Contém a descrição, que é a própria história em si no seguinte formato: "Como [papel do usuário], eu gostaria de [realizar determinada ação] a fim de/para [objetivo final do usuário]". Possuem ainda os critérios de aceitação, que foram definidos considerando que o requisito descrito na história só será considerado concluído pelo cliente caso os testes de aceitação estejam de acordo com os estabelecidos.

## Descrição de história de usuário

### - *EP01*

#### US01

**ID:** US01

**Descrição:** Como usuário, eu gostaria de poder me cadastrar na plataforma para ter acesso as funcionalidades desta.

**Critérios de aceitação**:
* Eu quero poder cadastrar meu nome completo, nome de usuário cpf, email, senha, número de celular, endereço e cep
* Eu quero poder cadastrar meu cartão de crédito usando o numero do cartão, numero de segurança, nome do responsável pelo cartão, nome que consta no cartão, cpf do responsável e bandeira do cartão 
* Eu quero poder escolher se sou "cliente", "funcionário", "entregador" ou "cozinheiro"

#### US02

**ID:** US02

**Descrição:** Como usuário, eu gostaria de poder me identificar na plataforma para acessar a minha conta.

**Critérios de aceitação**:
- Eu quero poder entrar na minha conta do aplicativo com email ou nome de usuário e senha cadastrada
- Eu quero poder fazer pedidos após fazer o login do aplicativo
- Eu quero poder clicar em acessar assim que entrar e ir direto para o cardápio
- Eu quero poder encerrar minha sessão no aplicativo utilizando um botão "Sair"

#### US03

**ID:** US03

**Descrição:** Como usuário, eu gostaria de poder editar minha senha para poder voltar a ter acesso a plataforma em caso de esquecimento.

**Critérios de aceitação**:
- Eu quero poder acessar um botão "Esqueci minha senha" e recuperar uma senha
- Eu quero poder pedir para me enviar uma nova senha para qualquer meio cadastrado no aplicativo (email ou celular)
- Eu quero poder acessar o sistema com a senha que recebi por email, ir em configurações e editar minha senha antiga


#### US04

**ID:** US04

**Descrição:** Como usuário, eu gostaria de poder atualizar meus dados pessoais para manter as minhas informações atualizadas na plataforma.

**Critérios de aceitação**:
- Eu quero poder acessar as informaçãoes do meu perfil, encontrar um ícone de lápis e trocar cada dado que estiver desatualizado

#### US05

**ID:** US05

**Descrição:** Como usuário eu gostaria de excluir minha conta caso não queira mais utilizar a aplicação.

**Critérios de aceitação**:
- Eu quero poder ir no meu perfil e encontrar um botão excluir conta para não utilizá-la mais
- Eu quero ser avisado de que eu estou excluindo a minha conta para não excluir por engano

#### US06

**ID:** US06

**Descrição:** Como Chapa Quente, eu gostaria de excluir o usuário caso ele descumpra as diretrizes da aplicação.

**Critérios de aceitação**:
- Eu quero ser notificado de que um usuário descumpriu as diretrizes 
- Eu quero poder visualizar uma lista de usuários e selecionar o que desejo excluir para que ele não tenha mais acesso à aplicação

#### US07

**ID:** US07

**Descrição:** Como usuário, eu gostaria de visualizar meus dados a fim 
de saber se eles estão atualizados.

**Critérios de aceitação**:
- Eu quero acessar uma tela a partir de um botão "Meu perfil" para saber quais são os dados que estão cadastrados na plataforma

----------------------------------------
 
### - *EP02*

#### US08

**ID:** US08

**Descrição:** Como usuário, eu gostaria de ser capaz de ter acesso aos horários de funcionamento da loja para saber quando posso realizar um pedido.
**Critérios de aceitação**:

- Eu quero poder ver quais dias da semana e horários de funcionamento da lanchonete para saber se posso pedir o meu lanche
- Eu quero que a aplicação esteja cinza e com a informação de que está fechada para que não haja erro
- Eu quero que a aplicação não aceite pedidos quando está fechada e me informe que não está aceitando pedidos

#### US09

**ID:** US09

**Descrição:** Como usuário, eu gostaria de ser capaz de saber onde a lanchonete está localizada a fim de saber de quais locaisposso realizar um pedido.

**Critérios de aceitação**:
- Eu quero visualizar em qual cidade, estado e país a lanchonete está localizada
- Eu quero ver em um mapa na aplicação o local onde a lanchonete está localizada

#### US10

**ID:** US10

**Descrição:** Como usuário, eu gostaria de ter um meio de contato com a loja a fim de resolver eventuais problemas com a loja

**Critérios de aceitação**:
- Eu quero poder acessar um ícone de chat e entrar em contato automaticamente com a lanchonete


----------------------------------------
 
### - *EP03*

#### US11

**ID:** US11

**Descrição:** Como usuário, eu gostaria de ter acesso ao cardapio para saber a lista de refeições disponíveis.
**Critérios de aceitação**:

- Eu quero poder ver o cardápio organizado por categorias
- Eu quero poder acessar o cardápio apertando um botão a partir de qualquer ponto da aplicação

#### US12

**ID:** US12

**Descrição:** Como usuário, eu desejo ter acesso a alimentos para pessoas que possuem restrições alimentares a fim de poder escolher o lanche que mais se adequa nas minhas restrições 

**Critérios de aceitação**:
- Eu quero poder acessar um menu específico para pessoas com restrições alimentares
- O menu específico deve mostrar categorias para as diferentes restrições alimentares e os produtos disponíveis na lanchonete para cada uma delas

#### US13

**ID:** US13

**Descrição:** Como usuário, eu desejo pesquisar o lanche por característica para ir diretamente para os lanches que desejo

**Critérios de aceitação**:
- A aplicação deve ter um campo de filtro para pesquisa do lanche pelo nome atualizando a cada letra escrita os produtos disponíveis
 
#### US14

**ID:** US14

**Descrição:** Como funcionário do Chapa Quente, eu desejo conseguir cadastrar lanches do cardápio a fim de garantir que o sistema sempre estará atualizado de acordo com os produtos disponíveis na lanchonete Chapa Quente.

**Critérios de aceitação**:
- Eu quero poder ver uma tela com os campos nome, categoria, restrição, tamanho e acompanhamentos possíveis na hora de cadastrar um nome produto

#### US15

**ID:** US15

**Descrição:** Como funcionário do Chapa Quente, eu desejo conseguir editar lanches do cardápio a fim de garantir que caso sejam cadastrados com algum erro, não seja necessário apagar todos os produtos

**Critérios de aceitação**:
- Eu quero poder clicar em um ícone para editar o produto e conseguir acessar uma tela que permite essa edição
- Eu quero poder ver uma tela com os campos nome, categoria, restrição, tamanho e acompanhamentos possíveis na hora de editar um produto

#### US16

**ID:** US16

**Descrição:** Como funcionário do Chapa Quente, eu desejo conseguir remover lanches do cardápio a fim de garantir que o sistema sempre estará atualizado de acordo com os produtos disponíveis na lanchonete Chapa Quente.

**Critérios de aceitação**:
- Eu quero poder ver um botão para excluir um lanche próximo ao produto no cardápio
- A aplicação deve me perguntar se eu tenho certeza que desejo excluir para evitar erros

----------------------------------------
 
### - *EP04*

#### US17

**ID:** US17

**Descrição:** Como usuário, eu gostaria de realizar meu pedido para prosseguir para o pagamento.

**Critérios de aceitação**:
- Eu quero poder escolher os itens que desejo e adicionar em um carrinho
- Eu quero poder apertar em um botão de "Prosseguir para pagamento" para acessar a parte de pagamento do sistema
- O sistema deve permitir que eu volte e escolha mais itens, exclua itens ou modifique os que já estão no carrinho

#### US18

**ID:** US18

**Descrição:** Como usuário, eu desejo efetuar o pagamento a fim de 
comprar o lanche que desejo

**Critérios de aceitação**:
- O sistema deve permitir que eu escolha diferentes formas de pagamento
- Eu quero poder pagar através do aplicativo utilizando o cartão de crédito

#### US19

**ID:** US19

**Descrição:** Como usuário, eu gostaria de receber cupons para diminuir meus custos.

**Critérios de aceitação**:
- Eu quero poder ver os cupons que tenho disponíveis para utilizar
- Eu quero receber um alerta com frases legais quando possuir cupons novos para utilizar
- Eu quero aplicar um cupom na tela de pagamento 
- Eu quero visualizar de quanto é o meu cupom
- A aplicação deve me mostrar quanto fica o pedido quando o cupom for aplicado

#### US20

**ID:** US20

**Descrição:** Como Chapa Quente, eu desejo disponibilizar cupons  de desconto a fim de fidelizar os usuários

**Critérios de aceitação**:
- Eu quero que a aplicação envie emails para os usuários cadastrados, avisando dos novos cupons
- Eu quero que a aplicação dê desconto para usuários que estão seguindo a quarentena, por isso quero que a aplicação conte os usuários com mais pedidos por entrega e envie cupons para essas pessoas


----------------------------------------
 
### - *EP05*

#### US21

**ID:** US21

**Descrição:** Como usuário, eu desejo acompanhar o rastreamento do pedido a fim de saber em qual etapa o meu pedido está

**Critérios de aceitação**:
- Eu quero poder acessar um campo na aplicação e ver se o meu pedido está "em fila de preparação", "sendo preparado", "finalizando a preparação", "pronto", "esperando o entregador", "em rota de entrega", "no portão", "entregue"
- Eu quero acessar a localização do entregador para que eu saiba se está muito longe da minha casa

#### US22

**ID:** US22

**Descrição:** Como cozinheiro, eu gostaria de ter a lista de pedidos feitos para facilitar aminha propria organização encontrando-os com maior facilidade para cozinhá-los ou prepará-los

**Critérios de aceitação**:
- A aplicação deve permitir o meu cadastro como cozinheiro 
- A aplicação deve permitir que eu acesse a lista de pedidos feitos
- A aplicação deve permitir que eu visualize as informações sobre cada pedido feito

#### US23

**ID:** US19

**Descrição:** Como cozinheiro, eu gostaria de ser capaz de avisar sobre o estado de preparo de um pedido para facilitar a organização interna.

**Critérios de aceitação**:
- A aplicação deve permitir que eu veja e clique em um botão para avisar se o pedido está "sendo preparado", finalizando a preparação" ou "pronto"
- Eu quero que o usuário saiba em qual etapa de preparação está o pedido e seja notificado sobre isso


#### US24

**ID:** US24 

**Descrição:** Como entregador, eu desejo conseguir visualizar as informações sobre os pedidos a fim de saber quando devo ir buscá-lo e quanto tempo falta para que o pedido fique pronto

**Critérios de aceitação**:
- Eu quero poder ver a lista de pedidos feitos e o endereço de entrega de cada pedido
- Eu quero poder ver o estado de preparação de cada pedido

#### US25

**ID:** US25

**Descrição:** Como entregador, eu desejo compartilhar minha localização com o cliente para que ele esteja preparado para receber o pedido quando eu chegar na residência

**Critérios de aceitação**:
- A aplicação deve permitir que eu compartilhe minha localização com o cliente para que ele saiba a qual distância estou dele
- Eu quero que o sistema calcule aproximadamente a distância que estou do cliente e informe para ele
- Eu quero apertar em um botão para avisar ao cliente que o lanche Chapa Quente chegou

#### US26

**ID:** US26

**Descrição:** Como usuário, eu desejo ver a localização do entregador a fim de saber quanto tempo falta para o meu pedido chegar e para ficar no portão/portaria para recebê-lo

**Critérios de aceitação**:
- A aplicação deve me mostrar em um mapa onde está o entregador
- A aplicação deve me mostrar como um relógio quanto tempo falta para o entregador chegar
- Eu quero que o sistema atualize esse relógio automaticamente de segundo em segundo
- Eu quero que a aplicação me notifique quando o pedido chegar

#### US27

**ID:** US27

**Descrição:** Como entregador, eu gostaria de ter um meio de contato com o usuário, para faciltar eventuais problemas na entrega

**Critérios de aceitação**:
- Eu quero acessar um ícone de chat que me manda para um chat com usuário
- Eu quero poder ver as informações de contato do usuário para me comunicar com ele

#### US28

**ID:** US28

**Descrição:** Como usuário, desejo receber o código de confirmação do pedido a fim de garantir que ninguém receberá o pedido no meu lugar

**Critérios de aceitação**:
- Eu quero ver no sistema um código de confirmação do pedido
- Eu quero receber esse código por email e SMS
- Eu quero ser notificado que o código chegou

#### US29

**ID:** US29

**Descrição:** Como entregador, desejo receber o código de confirmação do pedido a fim de garantir que não estou entregando o pedido no lugar errado

**Critérios de aceitação**:
- Eu quero ver no sistema um código de confirmação do pedido
- Eu quero receber esse código por email e SMS
- Eu quero ser notificado que o código chegou

#### US30

**ID:** US30

**Descrição:** Como Chapa Quente, desejo receber o código de confirmação do pedido a fim de garantir que o pedido está sendo entregue para a pessoa correta

**Critérios de aceitação**:

- Eu quero ver no sistema um código de confirmação do pedido
- Eu quero receber esse código por email e SMS com o nome da pessoa que realizou o pedido, a descrição do pedido e o nome do entregador responsável
- Eu quero ser notificado que o código chegou

#### US31

**ID:** US31

**Descrição:** Como usuário, eu gostaria de poder retirar o pedido no próprio local para reduzir meus custos.

**Critérios de aceitação**:
- Eu quero ver uma opção quando finalizar o pedido para selecionar "Retirar pedido no local"
- Eu quero ser redirecionado para o mapa que mostra onde a lanchonete fica após clicar na opção para retirar no local

----------------------------------------
 
### - *EP06*

#### US32

**ID:** US32

**Descrição:** Como usuário, eu gostaria de poder avaliar um pedido 
a fim de expressar o meu grau de satisfação com o serviço.

**Critérios de aceitação**:
- Eu quero poder ver emojis de triste, mediano e feliz para classificar se o serviço for bom
- Eu quero que o sistema me pergunte porque foi ruim caso eu escolha a carinha triste

#### US33

**ID:** US33

**Descrição:** Como lanchonete Chapa Quente, desejo permitir que o usuário avalie o pedido a fim de melhorar a qualidade do serviço

**Critérios de aceitação**:
- Eu quero que o usuário possa ver emojis de triste, mediano e feliz para classificar se o serviço for bom
- Eu quero que o sistema pergunte o feedback caso o usuário selecione uma carinha triste

## Conclusão

A utilização de histórias de usuário foi discutida e bem aceita pelo grupo, que concluiu que estas facilitam a visualização do sistema por meio do olhar do usuário e agregam bastante valor para o projeto.

## Bibliografia

USER Stories e Critérios de Aceitação. [S. l.], 15 maio 2018. Disponível em: [https://medium.com/@karladiasn/user-stories-e-crit%C3%A9rios-de-aceita%C3%A7%C3%A3o-317c48403fcd](https://medium.com/@karladiasn/user-stories-e-crit%C3%A9rios-de-aceita%C3%A7%C3%A3o-317c48403fcd). Acesso em: 15 fev. 2022.