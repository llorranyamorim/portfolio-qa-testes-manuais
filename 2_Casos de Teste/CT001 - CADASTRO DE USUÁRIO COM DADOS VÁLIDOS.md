# Caso de Teste: Cadastro de Usuário com Dados Válidos

**ID:** CAD-CT001  
**Módulo:** Cadastro  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Positivo)  
**Pré-condição:**  
- Usuário e e-mail não cadastrados previamente no sistema.  
- Usuário deve estar na tela de cadastro.  

## Dados de Entrada
| Campo | Valor |
|-------|-------|
| Nome  | Lorrany Amorim |
| E-mail | llorrany@teste.com |
| Senha  | teste12345|

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)
2. Navegar até a tela de **Cadastro**.
3. Preencher o campo **Nome** com um nome válido.
4. Preencher o campo **E-mail** com um e-mail válido.
5. Preencher o campo **Senha** com uma senha válida.
6. Clicar no botão **"Cadastrar"**.
7. Verificar se o sistema redireciona para a **Página Inicial**.
8. Validar se a mensagem de sucesso é exibida corretamente.

## Resultado Esperado
- O sistema deve redirecionar para a **Página Inicial**.
- Deve ser exibida a mensagem:
  > **"Cadastro realizado! Bem-vindo, Lorrany Amorim"**
- Dados devem ser salvos corretamente na base de dados e associados ao novo usuário.

## Evidência
![Cadastro de Usuário com Sucesso](/3_Evidências/CT001-cadastro_realizado_com_sucesso.png)
