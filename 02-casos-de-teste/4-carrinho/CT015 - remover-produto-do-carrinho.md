# Caso de Teste – CT015  
## Remover produto do carrinho

**ID:** CT015  
**Funcionalidade:** Carrinho  
**Cenário Relacionado:** CEN15 – Remover produto do carrinho     
**Tipo:** Positivo  
**Prioridade:** Alta  
**Pré-condição:** Usuário deve estar cadastrado no sistema e deve ter pelo menos um item no carrinho

---

### Objetivo
Validar que o usuário pode remover um item do carrinho com sucesso.

---

### Passos
1. Acessar o carrinho de compras.  
2. Identificar o produto que será removido.  
3. Clicar no botão **"Remover"** ou no ícone correspondente.  

---

### Resultado Esperado
- O item deve ser removido imediatamente.  
- O total do carrinho deve ser recalculado.  
- Caso fosse o único item, o carrinho deve exibir a mensagem de vazio.  

---

### Status
Passou ✅ 

---

### Resultado Encontrado
O mesmo que o esperado
  
---

### Evidências
**CARRINHO ANTES DE REMOVER O PRODUTO**
![EV-CT015](../../03-evidencias/EV-CT015.png)

**CARRINHO DEPOIS DE REMOVER O PRODUTO**
![EV-CT015](../../03-evidencias/EV-CT015(2).png)




