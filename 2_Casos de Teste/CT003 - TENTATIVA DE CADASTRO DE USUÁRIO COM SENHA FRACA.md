# Caso de Teste: Tentativa de cadastro de usuário com senha fraca(ex:12345)

**ID:** CAD-CT003 
**Módulo:** Cadastro  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Negativo)  

---

## Pré-condição
- O usuário deve estar na tela de cadastro
- O usuário não deve estar cadastrado previamente no sistema
- O sistema deverá aceitar senha de no mínimo 6 caracteres

---

## Dados de Entrada
| Campo  | Valor               |
|--------|---------------------|
| Nome   | Lorrany Amorim      |
| E-mail | llorrany@teste.com |
| Senha  | 12345

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)
2. Navegar até a tela de **Cadastro**.
3. Preencher o campo **Nome** com um nome válido.
4. Preencher o campo **E-mail** com um e-mail válido.
5. Preencher o campo **Senha** com uma senha menor de 6 digitos
6. Clicar no botão **"Cadastrar"**.
7. Validar se o sistema exibe a **mensagem de erro** corretamente.

---

## Resultado Esperado
- O sistema **não deve criar um novo cadastro**.
- Deve ser exibida a seguinte mensagem de erro:
  > **"O campo senha deve ter pelo menos 6 dígitos"**
- O usuário deve **permanecer na tela de cadastro** para tentar novamente.

---

## Evidência
![Erro - senha fraca](/evidencias/cadastro/erro_email_existente.png)
