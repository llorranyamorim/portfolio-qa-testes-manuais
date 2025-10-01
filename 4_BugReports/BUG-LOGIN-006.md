# BUG-LOGIN-006 - Tecla ENTER não executa login

**Módulo:** Login  
**Prioridade:** Alta  
**Severidade:** Média (afeta usabilidade, mas não impede login)  
**Status:** Aberto  
**Reportado por:** Lorrany Amorim de Oliveira  
**Data:** 01/10/2025  

---

## Descrição
- Ao tentar realizar o login pressionando a tecla **ENTER** do teclado, o sistema não autentica o usuário.  
- O login só é realizado quando o usuário clica manualmente no botão **"CONECTE-SE"**.  
- Esse comportamento não está de acordo com boas práticas de usabilidade, já que o ENTER deve funcionar como atalho para enviar o formulário.  

---

## Pré-condições
- Estar na tela de **Login**.  
- Possuir credenciais válidas de acesso.  

---

## Passos para Reproduzir
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/).  
2. Navegar até a tela de **Login**.  
3. Preencher o campo **E-mail** com `llorrany@teste.com`.  
4. Preencher o campo **Senha** com `teste12345`.  
5. Pressionar a tecla **ENTER** do teclado.  

---

## Resultado Esperado
- O sistema deve autenticar o usuário ao pressionar a tecla **ENTER**.  
- O usuário deve ser redirecionado para a **Página Inicial** já logado.  
- Deve ser exibida a mensagem de boas-vindas com o nome do usuário logado.  

---

## Resultado Obtido
- Nada acontece ao pressionar a tecla **ENTER**.  
- O login só é possível clicando manualmente no botão **"CONECTE-SE"**.  

---

## Evidência
![Evidência - ENTER não executa login](/3_Evidências/2_Login/BUG-LOGIN-006_Enter_nao_funciona.JPG)
