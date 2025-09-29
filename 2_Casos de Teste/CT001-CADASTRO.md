# Caso de Teste: CADASTRO DE USUÁRIO COM DADOS VÁLIDOS

**ID:** CT001  
**Módulo:** Cadastro  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Positivo)
**Pré-condição:** Usuário e E-mail não cadastrados previamente no sistema.

## Dados de Teste (Massa de Teste)
| Campo | Valor |
| :--- | :--- |
| **Nome** | Lorrany Amorim |
| **E-mail** | lorranyamorim@teste.com |
| **Senha** | senha123 |

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)
2. Clicar no botão **"Cadastro"**.
3. Preencher os campos do formulário com os **Dados de Teste** acima.
4. Clicar no botão **"Cadastrar"**.
5. Verificar o redirecionamento e a mensagem de sucesso na tela.

## Resultado Esperado
- O usuário deve ser **redirecionado** para a **Página Inicial**.
- O sistema deve exibir, na tela, uma mensagem de sucesso, contendo o nome fornecido no cadastro:
  > **"Cadastro realizado! Bem-vindo, Lorrany Amorim"**

## Evidência
![CADASTRO DE USUÁRIO](/3_Evidências/cadastro_realizado_com_sucesso.png)













