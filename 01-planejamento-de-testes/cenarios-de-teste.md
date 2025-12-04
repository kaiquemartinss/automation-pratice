# Cenários de Teste – Automation Pratice 

## 1. Cadastro

| ID     | Cenário                                               | Tipo        | Pré-condição                       | Resultado Esperado                                      |
|--------|--------------------------------------------------------|-------------|-------------------------------------|----------------------------------------------------------|
| CEN01  | Cadastro com dados válidos                             | Positivo    | Usuário não cadastrado              | Conta criada com sucesso                                 |
| CEN02  | Cadastro com e-mail já existente                       | Negativo    | E-mail já registrado                | Exibir mensagem de e-mail duplicado                      |
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
| CEN09  | Tentar logar com campos vazios                         | Negativo    | Nenhuma                              | Sistema solicita preenchimento dos campos                |
| CEN10  | Login com e-mail inválido                              | Negativo    | Nenhuma                              | Exibir mensagem de e-mail inválido                       |

---

## 3. Busca de Produtos

| ID     | Cenário                                               | Tipo        | Pré-condição                       | Resultado Esperado                                      |
|--------|--------------------------------------------------------|-------------|-------------------------------------|----------------------------------------------------------|
| CEN11  | Busca por produto existente                            | Positivo    | Produto listado no sistema          | Exibição dos produtos encontrados                        |
| CEN12  | Busca por produto inexistente                          | Negativo    | Nenhuma                              | Mensagem “Nenhum produto encontrado”                    |
| CEN13  | Busca com campo vazio                                  | Negativo    | Nenhuma                              | Solicitar preenchimento do campo                         |
| CEN14  | Busca exibindo resultados relacionados (se houver)     | Positivo    | Nenhuma                              | Exibir produtos relacionados ao termo buscado            |

---

## 4. Visualização de Produtos

| ID     | Cenário                                               | Tipo        | Pré-condição                       | Resultado Esperado                                      |
|--------|--------------------------------------------------------|-------------|-------------------------------------|----------------------------------------------------------|
| CEN15  | Visualizar detalhes de um produto                      | Positivo    | Produto existente                   | Exibir nome, descrição, imagem e preço                   |
| CEN16  | Navegar pelas imagens do produto                       | Positivo    | Produto com galeria de imagens      | Imagem principal deve ser atualizada                     |
| CEN17  | Visualizar preço e descrição                           | Positivo    | Produto existente                   | Dados corretos devem ser exibidos                        |
| CEN18  | Exibir produtos relacionados                           | Positivo    | Produtos relacionados cadastrados   | Lista de produtos relacionados deve aparecer             |

---

## 5. Carrinho

| ID     | Cenário                                               | Tipo        | Pré-condição                       | Resultado Esperado                                      |
|--------|--------------------------------------------------------|-------------|-------------------------------------|----------------------------------------------------------|
| CEN19  | Adicionar produto ao carrinho                          | Positivo    | Produto disponível                  | Item adicionado ao carrinho                              |
| CEN20  | Remover produto do carrinho                            | Positivo    | Carrinho com itens                  | Item removido com sucesso                                |
| CEN21  | Atualizar quantidade de itens                          | Positivo    | Item no carrinho                    | Quantidade alterada e total atualizado                   |
| CEN22  | Validar cálculo total do carrinho                      | Positivo    | Carrinho com itens                  | Total exibido corretamente                               |
| CEN23  | Carrinho vazio após remover todos os itens             | Positivo    | Carrinho previamente preenchido     | Carrinho exibe mensagem de vazio                         |

---

## 6. Checkout

| ID     | Cenário                                               | Tipo        | Pré-condição                       | Resultado Esperado                                      |
|--------|--------------------------------------------------------|-------------|-------------------------------------|----------------------------------------------------------|
| CEN24  | Finalizar compra com dados válidos                     | Positivo    | Carrinho com itens                  | Pedido finalizado com sucesso                            |
| CEN25  | Tentar finalizar compra com dados inválidos            | Negativo    | Carrinho com itens                  | Exibir mensagens de erro                                 |
| CEN26  | Selecionar forma de pagamento                          | Positivo    | Fluxo de checkout iniciado          | Pagamento selecionado corretamente                       |
| CEN27  | Validar cálculo final do pedido                        | Positivo    | Checkout iniciado                   | Total calculado corretamente                             |
| CEN28  | Exibir confirmação do pedido                           | Positivo    | Compra finalizada                   | Tela/confirmação de pedido exibida                       |

---

## 7. Contato

| ID     | Cenário                                               | Tipo        | Pré-condição                       | Resultado Esperado                                      |
|--------|--------------------------------------------------------|-------------|-------------------------------------|----------------------------------------------------------|
| CEN29  | Enviar mensagem com dados válidos                      | Positivo    | Nenhuma                              | Mensagem enviada com sucesso                             |
| CEN30  | Enviar formulário com campos vazios                    | Negativo    | Nenhuma                              | Exibir mensagens de campos obrigatórios                  |
| CEN31  | Enviar com e-mail inválido                             | Negativo    | Nenhuma                              | Exibir mensagem de e-mail inválido                       |
| CEN32  | Enviar mensagem muito longa (testar limites)           | Negativo    | Campo com limite definido           | Exibir aviso ou bloquear envio                           |

---
