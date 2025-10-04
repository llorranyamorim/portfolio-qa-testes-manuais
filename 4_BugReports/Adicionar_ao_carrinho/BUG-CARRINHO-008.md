# BUG-CARRINHO-008

**Título:** Produto adicionado ao carrinho sem estar logado no sistema

**ID:** BUG-CARRINHO-008  
**Módulo:** Carrinho de Compras  
**Prioridade:** Alta  
**Severidade:** Alta (afeta a segurança e fluxo de compra do usuário)  
**Status:** Aberto  
**Reportado por:** Lorrany Amorim de Oliveira  
**Data:** 04/10/2025  

---

## Descrição
O sistema permite que o usuário adicione um produto ao carrinho sem estar logado. Embora a ação de adicionar o produto seja realizada com sucesso, o sistema deveria obrigar o login antes de permitir que o usuário adicione qualquer item ao carrinho.

---

## Pré-condições
- O navegador deve estar aberto e conectado à internet.  
- O usuário **não deve estar logado** no sistema.

---

## Passos para Reproduzir
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)  
2. Não realizar login no sistema.  
3. Localizar um produto desejado (exemplo: **Vestido Longo**).  
4. Tentar adicionar o produto ao carrinho sem fazer login.
5. Verificar se o produto é adicionado ao carrinho com sucesso.

---

## Resultado Atual
- O sistema **permite** que o usuário adicione o produto ao carrinho **sem estar logado**.  
- O produto é adicionado ao carrinho, mas o usuário não é solicitado a fazer login antes de prosseguir com a ação.

---

## Resultado Esperado
- O sistema deve **bloquear** a adição de qualquer produto ao carrinho se o usuário **não estiver logado**.  
- O sistema deve **solicitar** o login do usuário antes de permitir a adição de produtos ao carrinho, redirecionando-o para a página de login.

---

## Evidência  
📎 [Vídeo do erro](https://drive.google.com/file/d/1NhtdPOL2-JKsnib8o75egLPL78bF_D7E/view?usp=sharing)
