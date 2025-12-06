# Caso de Teste – CT002  
## Cadastro com e-mail já existente

**ID:** CT002  
**Funcionalidade:** Cadastro de Usuário  
**Cenário Relacionado:** CEN02 – Cadastro com e-mail já existente  
**Tipo:** Negativo  
**Prioridade:** Alta  
**Pré-condição:** O e-mail informado já deve estar cadastrado no sistema  

---

### Objetivo
Validar que o sistema impeça a criação de um novo usuário utilizando um e-mail já existente.

---

### Passos

1. Acessar a página de cadastro.
2. Preencher o campo "Nome".
3. Preencher o campo "E-mail" com um e-mail já cadastrado.
4. Preencher o campo "Senha" com uma senha válida (mínimo de 6 caracteres).
5. Clicar no botão **"Cadastrar"**.

---

### Resultado Esperado
- O sistema deve impedir o cadastro.  
- Deve exibir a mensagem: **"E-mail já cadastrado"**.  
- O usuário deve permanecer na página de cadastro.  

---

### Status
- Falhou ❌  

---

### Resultado Encontrado
- Sistema está permitindo realizar cadastro, mesmo para um email que já foi cadastrado anteriormente.
  
---

### Evidências
![EV-CT002](../../03-evidencias/EV-CT002.png)




