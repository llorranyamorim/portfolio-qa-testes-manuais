# BUG-LOGIN-001

**Título:** Mensagem de boas-vindas exibe e-mail em vez do nome do usuário cadastrado

**ID:** BUG-LOGIN-001  
**Módulo:** Login  
**Prioridade:** Média  
**Severidade:** Baixa (não impede uso do sistema, mas afeta a experiência)  
**Status:** Aberto  
**Reportado por:** Lorrany Amorim de Oliveira  
**Data:** 2025-09-30

---

## Descrição
Após realizar login com credenciais válidas, o sistema exibe mensagem de boas-vindas utilizando o **e-mail do usuário** em vez do **nome cadastrado**. Isso prejudica a experiência do usuário e está em desacordo com o requisito de exibir o nome.

---

## Ambiente
- **URL:** https://www.automationpratice.com.br/  
- **Navegador:** Google Chrome 140.0.0.0 (64 bits)  
- **Sistema Operacional:** Windows 10 Pro – 64 bits  
- **Data/Hora do Teste:** 30/09/2025 – 08:14  

---

## Pré-condições
- Usuário `llorrany@teste.com` previamente cadastrado no sistema.  
- Navegador aberto e conectado à internet.  
- Página de login acessível.

---

## Passos para Reproduzir
1. Acessar a URL: https://www.automationpratice.com.br/  
2. Clicar em **Login**.  
3. Informar as credenciais válidas:  
   - **E-mail:** `llorrany@teste.com`  
   - **Senha:** `teste12345`  
4. Clicar no botão **CONECTE-SE**.  
5. Observar a mensagem de boas-vindas exibida.

---

## Resultado Atual
- Mensagem apresentada:  
  > **Login realizado. Olá, llorrany@teste.com**

---

## Resultado Esperado
- Mensagem de boas-vindas deve exibir o **nome do usuário cadastrado**, por exemplo:  
  > **Login realizado. Olá, Lorrany**

---

## Impacto
- Experiência do usuário (UX) comprometida: usuários esperam ser saudados pelo nome.  
- Baixo impacto funcional (login funciona normalmente), mas afeta percepção de profissionalismo e personalização.

---

## Evidências
![Evidência Login - Bug](/3_Evidencias/LOGIN-001_Login_realizado.JPG)

> Arquivo de evidência: `3_Evidencias/LOGIN-001_Login_realizado.JPG`

---

## Observações / Comentários do Testador
- Verificar se o cadastro do usuário possui campo "Nome" preenchido no perfil.  
- Caso o campo exista e esteja preenchido, investigar a rotina que popula o texto da mensagem (possível uso de `user.email` em vez de `user.name`).  
- Se a exibição do e-mail for uma decisão de produto, alinhar com PO/PM e ajustar o caso de teste.

---

## Proposta de Correção (sugestão)
- Ajustar a função que renderiza a mensagem de boas-vindas para priorizar `user.name` (quando presente), e só exibir `user.email` como fallback caso `user.name` esteja vazio ou nulo.

---


