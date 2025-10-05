# BUG-LOGIN-003

**Título:** Login realizado com E-mail não cadastrado  

**ID:** BUG-LOGIN-003  
**Módulo:** Login  
**Prioridade:** Alta  
**Severidade:** Alta (impede uso correto do sistema)  
**Status:** Aberto  
**Reportado por:** Lorrany Amorim de Oliveira  
**Data:** 2025-09-30  

---

## Descrição
O sistema permite o login do usuário com um **E-mail não cadastrado**.  
Esse comportamento compromete a segurança do sistema e viola o requisito de validação correta das credenciais.

---

## Ambiente
- **URL:** https://www.automationpratice.com.br/  
- **Navegador:** Google Chrome 140.0.0.0 (64 bits)  
- **Sistema Operacional:** Windows 10 Pro – 64 bits  
- **Data/Hora do Teste:** 30/09/2025 – 08:14  

---

## Pré-condições
1. Usuário `lorranyamorim@teste.com` (não cadastrado no sistema)  
2. Senha `teste12345` (senha válida de outro usuário cadastrado)  
3. Navegador aberto e conectado à internet  
4. Página de login acessível  

---

## Passos para Reproduzir
1. Acessar a URL: https://www.automationpratice.com.br/  
2. Clicar em **Login**  
3. Informar as credenciais:  
   - **E-mail:** `lorranyamorim@teste.com`  
   - **Senha:** `teste12345`  
4. Clicar no botão **CONECTE-SE**  
5. Observar o comportamento do sistema  

---

## Resultado Atual
- O sistema permite o login e exibe a mensagem:  
  > **Login realizado. Olá, lorranyamorim@teste.com**  

---

## Resultado Esperado
- O sistema **não deve permitir o login** com e-mail não cadastrado  
- O sistema deve exibir uma mensagem clara de erro de autenticação, por exemplo:  
  > **Usuário não encontrado**  

---

## Impacto
- Falha crítica de autenticação: permite que qualquer pessoa acesse o sistema com e-mail inexistente, desde que use uma senha válida.  
- Compromete a **integridade da autenticação** e abre brecha para acessos não autorizados.  

---

## Evidências
![Evidência Login - Bug](/3_Evidências/2_Login/LOGIN-003_E-mail_não_cadastrado.JPG)  

> Arquivo de evidência: `3_Evidências/2_Login/LOGIN-003_E-mail_não_cadastrado.JPG`  

---

## Observações
- Recomendado correção imediata, pois este defeito impacta diretamente a **segurança do sistema**.
