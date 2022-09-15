# Requisitos de um correio eletrônico (email)

Para a execução dessa atividade foi escolhido um sistema de correio eletrônico, e dele serão extraídos os dois **requisitos** funcionais pedidos.
Classifica-se como requisito funcional uma ação que o sistema deve ser capaz de executar para que cumpra com seu propósito, e neste caso serão escolhidos os seguintes requisitos : 

#### Requisitos funcionais
> - enviar email
> - receber email

***

# Casos de uso

Item           | Descrição    
---------------|--------------
Caso de uso    | Enviar email.
Resumo         | É esperado que ao clicar no botão para escrever um email seja exibida para o usuário uma tela onde ele possa informar o destinarário, o título e o conteúdo do email, e é esperado que o destinatário o receba e possa visualizá-lo.
Ator principal | Usuário utilizador do email.
Ator secundário| Não possui.
Pré-condição   | É necessário que primeiramente o usuário tenha efetuado o login com sucesso em sua conta.
Pós-condição   | É necessário que após ter redigido o email, o usuário esteja conectado numa rede de internet para que o email possa ser enviado.

#### Fluxo principal

Passos  | Descrição
--------|-----------
Passo 1 | Clicar no botão de escrever email.
Passo 2 | Digitar um email válido (a aplicação clicará sozinha na caixa de texto do email do destinatário após o passo 1).
Passo 3 | Clicar na caixa de texto do título do email.
Passo 4 | Digitar um título.
Passo 5 | Clicar na caixa de texto do corpo do email.
Passo 6 | Digitar algo no corpo do email.
Passo 7 | Clicar no botão de enviar.
Passo 8 | Aviso de mensagem enviada para o destino.

#### Campos da aba de escrever email

Campo                | Obrigatório | Editável | Formato
---------------------|-------------|----------|--------
Email do destinatário| Sim         | Sim      | Alfa numérico
Título do email      | Sim         | Sim      | Alfa numérico
Corpo do email       | Sim         | Sim      | Alfa numérico

#### Opções de usuários

Opção        | Descrição                                | Atalho
-------------|------------------------------------------|-------
Digitar email|Abre a aba de escrever email              | ctrl + e
Enviar email |Envia o email digitado para o destinatário| ctrl + s

#### Relatório do usuário

Campo| Descrição| Formato
-----|----------|--------

#### Fluxo alternativo

Passos    | Descrição
----------|----------
Passo 2.1 | A aplicação deve informar que um email com domínio válido deve ser digitado se o usuário errar e deverá retornar ao passo 2.
Passo 2.2 | Se um email com domínio válido for inserido mas ele não existir, o usuário deve ser alertado futuramente que o email não foi enviado.
Passo 3.1 | Se o usuário não clicar no título do email a aplicação deverá obrigá-lo a clicar exibindo uma mensagem, retornando ao passo 3
Passo 4.1 | Caso o usuário não digite nada, a aplicação deverá obrigá-lo a digitar algo, voltando ao passo 4.
Passo 5.1 | A aplicação deve obrigar o usuário a clicar na caixa de texto do corpo do email, voltando ao passo 5.
Passo 6.1 | Se o usuário não digitar nada, deverá aparecer uma mensagem obrigando-o a digitar algo para que o email possa ser enviado, voltando ao passo 6.
Passo 7.1 | Se o usuário nao clicar no botão de enviar, o corpo do email deve ser minimizado até que o usuário reabra ele ou o feche, cancelando o email.


Item           | Descrição    
---------------|--------------
Caso de uso    | Receber email.
Resumo         | É esperado que quando um email for enviado com sucesso ao destinatário, este possa visualizá-lo na sua caixa de entrada e lê-lo.
Ator principal | Usuário utilizador do email.
Ator secundário| Não possui.
Pré-condição   | É necessário que primeiramente o usuário tenha efetuado o login com sucesso em sua conta.
Pós-condição   | É necessário que o usuário esteja conectado na internet para que o email possa ser recebido.

#### Fluxo principal

Passos  | Descrição
--------|-----------
Passo 1 | O email deve aparecer na caixa de entrada (caso contrário o remetente será avisado no caso de uso anterior).
Passo 2 | Clicar em cima do email.
Passo 3 | Ter acesso ao conteúdo do email recebido.
Passo 4 | Ao sair da aba de leitura do email, deve aparecer um pequeno símbolo de ok mostrando que ele foi visualizado.

#### Campos da aba de ler email

Campo                | Obrigatório | Editável | Formato
---------------------|-------------|----------|--------

#### Opções de usuários

Opção                                     | Descrição                                | Atalho
------------------------------------------|------------------------------------------|-------
Abrir o email clicando nele               | Abre a aba de ler email                  |
Botão para voltar para a caixa de entrada | Volta para a caixa de entrada inicial    |

#### Relatório do usuário

Campo| Descrição| Formato
-----|----------|--------

#### Fluxo alternativo

Passos    | Descrição
----------|----------
Passo 3.1 | Se o usuário não conseguir ter acesso ao conteúdo do email, deverá clicar num botão com símbolo de bug e será aberto a aba de escrever email para que possa ser redigido um email para o remetente solicitando um reenvio. O campo de email do destinatário deve ser o email do remetente. O campo do título deve ser "falha ao visualizar "nome original do título do email"" e a apliacação deve clicar no corpo do email para que algo possa ser escrito.

# User story

Agora iremos escrever histórias de usuários para cada caso de uso, com uma persona.

#### Persona um, vendedor por web marketing

Epic                                                                                                                        |User story| Critério de aceitação
----------------------------------------------------------------------------------------------------------------------------|----------|----------------------
Eu "vendedor", quero "enviar emails para pessoas interessadas nos serviços de minha empresa, e também receber os emails dos interessados" para "divulgar nossa empresa". |Como "vendedor" eu preciso ser capaz de enviar um email para múltiplos usuário ao mesmo tempo para que eles saibam dos nossos serviços.| Certifique-se que os destinatários serão capazes de **login na sua conta**, **ler o email recebido**, **ver quem enviou ele** e **possam responder ele**.
.                                                                                                                           | Como "vendedor" eu preciso ser capaz de ler os emails respondidos pelos destinatários.                                                                                         | Certifique-se que o vendedor seja capaz de **fazer login na conta com domínio da empresa**, **ler os emails enviados para ele** respondidos e **possa novamente interagir com o remetente** .
.                                                                                                                           | Como "vendedor" eu preciso ser capaz de selecionar como prioritários emails de possíveis interessados.                                                                         | Certifique-se que o vendedor seja capaz de **fazer login na conta com domínio da empresa**, **visualizar os emails destinados a ele** e **clicar numa estrela próxima ao nome do email**
.                                                                                                                           | Como "vendedor" eu preciso ser capaz de excluir os emails de pessoas que negaram a proposta do serviço para que os futuros emails não sejam enviados para ela.                 | Certifique-se que o vendedor seja capaz de **fazer login na conta com domínio da empresa** e **clicar num símbolo de menos ao lado da estrela para que o email do remetente seja adicionado na blacklist**

# Protótipos das telas dos casos de uso

! [telas](telas.png)
