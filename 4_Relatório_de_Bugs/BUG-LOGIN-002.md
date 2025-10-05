# BUG-LOGIN-002

**Título:** Login realizado com senha incorreta

**ID:** BUG-LOGIN-002 
**Módulo:** Login  
**Prioridade:** Alta 
**Severidade:** Alta (impede uso do sistema)  
**Status:** Aberto  
**Reportado por:** Lorrany Amorim de Oliveira  
**Data:** 2025-09-30

---

## Descrição
O sistema permite o login do usuário com a credencial incorreta. Esse comportamento compromete a segurança do sistema e está em desacordo com o requisito de validar corretamente as credenciais.

---

## Ambiente
- **URL:** https://www.automationpratice.com.br/  
- **Navegador:** Google Chrome 140.0.0.0 (64 bits)  
- **Sistema Operacional:** Windows 10 Pro – 64 bits  
- **Data/Hora do Teste:** 30/09/2025 – 08:14  

---

## Pré-condições
1. Usuário `llorrany@teste.com` E-mail (cadastrado no sistema)
2. Senha `teste@123#` Senha inválida (não cadastrada no sistema)
3. Navegador aberto e conectado à internet.  
4. Página de login acessível.

---

## Passos para Reproduzir
1. Acessar a URL: https://www.automationpratice.com.br/  
2. Clicar em **Login**.  
3. Informar as credenciais:  
   - **E-mail:** `llorrany@teste.com`  
   - **Senha:** `teste@123#`  
4. Clicar no botão **CONECTE-SE**  
5. Observar o comportamento do sistema

---

## Resultado Atual
- Mensagem apresentada:  
  > **Login realizado. Olá, llorrany@teste.com**

---

## Resultado Esperado
- O sistema não deve permitir o login e deve exibir uma mensagem clara de erro de autenticação 
(ex: Senha incorreta)

---

## Impacto 
- Bug crítico de segurança: permite login com senha incorreta, comprometendo a integridade da autenticação e expondo o sistema a acessos não autorizados.

---

## Evidências
![Evidência Login - Bug](/3_Evidências/2_Login/LOGIN-002_Evidencia_Senha_Incorreta.JPG)

> Arquivo de evidência: `3_Evidências/2_Login/LOGIN-002_Evidencia_Senha_Incorreta.JPG`

---

## Observações 
- Recomenda-se correção imediata, pois este defeito impacta diretamente a **segurança do sistema**.



