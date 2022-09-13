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
Passo 3.1 | Se o usuário não clicar no título do email a aplicação deverá obrigá-lo a clicar exibindo uma mensagem, retornando ao passo 3
Passo 4.1 | Caso o usuário não digite nada, a aplicação deverá obrigá-lo a digitar algo, voltando ao passo 4.
Passo 5.1 | A aplicação deve obrigar o usuário a clicar na caixa de texto do corpo do email, voltando ao passo 5.
Passo 6.1 | Se o usuário não digitar nada, deverá aparecer uma mensagem obrigando-o a digitar algo para que o email possa ser enviado, voltando ao passo 6.
Passo 7.1 | Se o usuário nao clicar no botão de enviar, o corpo do email deve ser minimizado até que o usuário reabra ele ou o feche, cancelando o email.
