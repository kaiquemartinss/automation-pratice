# Cenários de Teste – Automation Pratice 

## 1. Cadastro

| ID     | Cenário                                               | Tipo        | Pré-condição                       | Resultado Esperado                                      |
|--------|--------------------------------------------------------|-------------|-------------------------------------|----------------------------------------------------------|
| CEN01  | Cadastro com dados válidos                             | Positivo    | Usuário não cadastrado              | Conta criada com sucesso                                 |
| CEN02  | Cadastro com e-mail já existente                       | Negativo    | E-mail já registrado                | Exibir mensagem de e-mail já cadastrado                      |
| CEN03  | Campos obrigatórios vazios                             | Negativo    | Nenhuma                              | Exibir alerta indicando campos obrigatórios               |
| CEN04  | Senha menor que 6 caracteres                           | Negativo    | Nenhuma                              | Exibir mensagem de senha inválida                         |
| CEN05  | E-mail em formato inválido                             | Negativo    | Nenhuma                              | Exibir mensagem de e-mail inválido                       |

---

## 2. Login

| ID     | Cenário                                               | Tipo        | Pré-condição                       | Resultado Esperado                                      |
|--------|--------------------------------------------------------|-------------|-------------------------------------|----------------------------------------------------------|
| CEN06  | Login com credenciais corretas                         | Positivo    | Usuário cadastrado                  | Login realizado com sucesso                              |
| CEN07  | Login com senha incorreta                              | Negativo    | Conta existente                     | Mensagem de senha incorreta                              |
| CEN08  | Login com e-mail não cadastrado                        | Negativo    | Nenhuma                              | Mensagem de usuário não encontrado                       |
| CEN09  | Tentar logar com campo Senha vazio                         | Negativo    | Nenhuma                              | Exibir mensagem de senha inválida                |
| CEN10  | Tentar logar com campo Email vazio                              | Negativo    | Nenhuma                              | Exibir mensagem de e-mail inválido                       |

---

## 3. Busca de Produtos

| ID     | Cenário                                               | Tipo        | Pré-condição                       | Resultado Esperado                                      |
|--------|--------------------------------------------------------|-------------|-------------------------------------|----------------------------------------------------------|
| CEN11  | Busca por produto existente                            | Positivo    | Produto listado no sistema          | Exibição dos produtos encontrados                        |
| CEN12  | Busca por produto inexistente                          | Negativo    | Nenhuma                              | Mensagem “Nenhum produto encontrado”                    |
| CEN13  | Busca com campo vazio                                  | Negativo    | Nenhuma                              | Solicitar preenchimento do campo                         |

---

## 4. Carrinho

| ID     | Cenário                                               | Tipo        | Pré-condição                       | Resultado Esperado                                      |
|--------|--------------------------------------------------------|-------------|-------------------------------------|----------------------------------------------------------|
| CEN14  | Adicionar produto ao carrinho                          | Positivo    | Produto disponível                  | Item adicionado ao carrinho                              |
| CEN15  | Remover produto do carrinho                            | Positivo    | Carrinho com itens                  | Item removido com sucesso                                |
| CEN16  | Atualizar quantidade de itens                          | Positivo    | Item no carrinho                    | Quantidade alterada e total atualizado                   |
| CEN17  | Validar cálculo total do carrinho                      | Positivo    | Carrinho com itens                  | Total exibido corretamente                               |
| CEN18  | Carrinho vazio após remover todos os itens             | Positivo    | Carrinho previamente preenchido     | Carrinho exibe mensagem de vazio                         |

---

## 5. Checkout

| ID     | Cenário                                               | Tipo        | Pré-condição                       | Resultado Esperado                                      |
|--------|--------------------------------------------------------|-------------|-------------------------------------|----------------------------------------------------------|
| CEN19  | Finalizar compra com dados válidos                     | Positivo    | Carrinho com itens                  | Pedido finalizado com sucesso                            |
| CEN20  | Tentar finalizar compra com dados inválidos            | Negativo    | Carrinho com itens                  | Exibir mensagens de erro                                 |
| CEN21  | Selecionar forma de pagamento                          | Positivo    | Fluxo de checkout iniciado          | Pagamento selecionado corretamente                       |
| CEN22  | Validar cálculo final do pedido                        | Positivo    | Checkout iniciado                   | Total calculado corretamente                             |
| CEN23  | Exibir confirmação do pedido                           | Positivo    | Compra finalizada                   | Tela/confirmação de pedido exibida                       |

---


