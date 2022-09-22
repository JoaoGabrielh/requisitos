# Caso de uso
**RF04**

Item           | Descrição
---------------|----------
Caso de uso    | Visualizar produto.
Resumo           | É esperado que ao ver um produto no catálogo caso o usuário clique seja aberta a página do produto em específico, mostrando preço, descrição do produto, botão de compra, de adicionar ao carrinho, de adicionar à lista de desejos, foto do produto, título do produto, avaliação dele, se ainda tem estoque e comentários sobre ele.
Ator principal | Usuário utilizador da plataforma.
Ator secundário| Não possui.
Pré-condição   | É necessário que o usuário esteja utilizando a plataforma, conectado-á internet.
Pós-condição   | É necessário que para adicionar o produto ao carrinho, à lista de desejos, avaliar ou comprar o produto o usuário esteja na sua própria conta.

#### Fluxo principal

Passos  | Descrição
--------|----------
Passo 1 | Clicar em cima da imagem do produto.
Passo 2 | Esperar a página do produto carregar.

#### Campos da aba de visualizar produtos

Campo                                | Obrigatório | Editável | Formato
-------------------------------------|-------------|----------|--------
Avaliar produto                      | Não         | Não      | Texto

#### Opções de usuário

Opção                                | Descrição   | Atalho
-------------------------------------|-------------|-------
Acessar o produto                    | Ao clicar no produto ele deve ser redirecionado para a aba do produto | 
Comprar o produto                    | Ao clicar no botão de compra ele deve ser redirecionado para a aba de efetuar a compra do produto                        |
Adicionar ao carrinho                | Ao clicar no botão de adicionar ao carrinho o item deve ser adicionado à ele |
Adicionar à lista de desejos         | Ao clicar no botão de adicionar à lista de desejos o item deve ser adicionado a essa lista |

#### Relatório de usuário

Campo | Descrição | Formato
------|-----------|--------

#### Fluxo alternativo

Passos      | Descrição
------------|----------
Passo 1.1   | Caso o usuário não clique, deve-se ter a opção de selecionar os produtos utilizando as setas do teclado e poder visualizar ele com a tecla de enter para confirmar.
Passo 2.1.1 | Caso ocorra erro ao carregar a página, ela deve se auto recarregar a cada 25 segundos para tentar visualizar o produto.
Passo 2.1.2 | Caso o produto não exista mais porque o vendedor o removeu, o usuário deve ser redirecionado para o catálogo de itens anterior.

# User story

Agora iremos escrever uma história de usuário para uma persona.

**Persona um, usuário comum.**

Epic                                |User Story| Critério de aceitação
-----------------------|----------|----------------------
Eu enquanto "usuário comum" quero "visualizar produtos específicos" para "saber mais coisas sobre ele". | Enquanto "usuário comum" eu preciso ser capaz de visualizar um produto em específico para saber mais informações sobre ele | Certifique-se que o usuário é capaz de **fazer login na própria conta, buscar uma série de produtos e visualizar um produto em específico.**
