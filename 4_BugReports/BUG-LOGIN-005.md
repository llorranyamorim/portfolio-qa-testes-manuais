# BUG-LOGIN-005

**Título:** Validação ausente do campo "Senha" ao tentar login sem preencher campos obrigatórios  

**ID:** BUG-LOGIN-0035 
**Módulo:** Login  
**Prioridade:** Alta  
**Severidade:** Média (afeta a experiência do usuário, mas não impede login)  
**Status:** Aberto  
**Reportado por:** Lorrany Amorim de Oliveira  
**Data:** 01/10/2025  

---

## Descrição
Ao tentar fazer login sem preencher os campos obrigatórios, o sistema exibe a mensagem de erro apenas para o campo **E-mail**. O campo **Senha** fica em branco sem nenhuma indicação de que é obrigatório.

---

## Ambiente
- **URL:** https://www.automationpratice.com.br/  
- **Navegador:** Google Chrome 140.0.0.0 (64 bits)  
- **Sistema Operacional:** Windows 10 Pro – 64 bits  
- **Data/Hora do Teste:** 01/10/2025 – 17:20  

---

## Pré-condições
1. Estar na tela de login 

---

## Passos para Reproduzir
1. Acessar a URL: https://www.automationpratice.com.br/  
2. Navegar até a tela de **Login**  
3. Deixar os campos *E-mail* e *Senha* em branco
4. Clicar no botão **CONECTE-SE**   

---

## Resultado Atual
- O sistema exibe apenas a mensagem **E-mail inválido**
- O campo **Senha** não apresenha nenhuma mensagem de erro  

---

## Resultado Esperado
- o sistema deve exibir mensagens claras de erro abaixo de **cada campo obrigatório**, por exemplo:
**"O campo E-mail é obrigatório"**
**"O campo Senha é obrigatório"**


---

## Impacto
- Experiência do usuário (UX), pois usuário não recebe feedback adequado sobre o erro no campo **Senha**, podendo até ficar sem entender porque não conseguiu fazer login.
- O sistema trata o campo **E-mail** como obrigatório (exibindo a mensagem de erro), mas não aplica a mesma regra de forma clara para o campo **Senha**.

---

## Evidências
![Evidência Login - Bug](/3_Evidências/2_Login/LOGIN-005_Login_sem_prencher_campos_obrigatórios)  

> Arquivo de evidência: `3_Evidências/2_Login/LOGIN-005_Login_sem_prencher_campos_obrigatórios`  

