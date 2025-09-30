# Caso de Teste: Cadastro de Usuário com E-mail Existente

**ID:** CAD-CT002  
**Módulo:** Cadastro  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Negativo)  

---

## Pré-condição
- Deve existir previamente um usuário cadastrado no sistema com o e-mail **llorrany@teste.com**.
- Usuário deve estar na tela de **Cadastro**.

---

## Dados de Entrada
| Campo  | Valor               |
|--------|---------------------|
| Nome   | Lorrany Amorim      |
| E-mail | llorrany@teste.com |
| Senha  | teste12345

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)
2. Navegar até a tela de **Cadastro**.
3. Preencher o campo **Nome** com um nome válido.
4. Preencher o campo **E-mail** com um e-mail já existente no sistema.
5. Preencher o campo **Senha** com uma senha válida.
6. Clicar no botão **"Cadastrar"**.
7. Validar se o sistema exibe a **mensagem de erro** corretamente.

---

## Resultado Esperado
- O sistema **não deve criar um novo cadastro**.
- Deve ser exibida a seguinte mensagem de erro:
  > **"E-mail já cadastrado no sistema"**
- Nenhum dado novo deve ser gravado no banco de dados.
- O usuário deve **permanecer na tela de cadastro** para tentar novamente.

---

## Evidência
![Erro - E-mail já cadastrado](/evidencias/cadastro/erro_email_existente.png)
