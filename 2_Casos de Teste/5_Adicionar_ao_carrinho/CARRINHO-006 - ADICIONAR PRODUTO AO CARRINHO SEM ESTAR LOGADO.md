# Caso de Teste: Adicionar produto ao carrinho sem estar logado

**ID:** CARRINHO-008  
**Módulo:** Carrinho de Compras  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Negativo)

---

## Pré-condições
- O navegador deve estar aberto e conectado à internet.  
- O usuário **não deve estar logado** no sistema.

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)  
2. Localizar um produto disponível na loja (exemplo: **Tênis Nike Air Max**).  
3. Clicar no botão **Adicionar ao Carrinho** para adicionar o produto ao carrinho.  
4. Tentar proceder para o carrinho de compras.

---

## Resultado Esperado
- O sistema deve solicitar que o usuário faça login antes de prosseguir com a adição do produto ao carrinho.  
- O carrinho não deve permitir a finalização da compra ou qualquer ação relacionada ao produto enquanto o usuário não estiver logado.  
- O usuário deve ser redirecionado para a página de login ou ser exibida uma mensagem solicitando o login.

---

## Evidência  
📎 [Evidência da execução do teste](./3_Evidências/3_Carrinho_de_Compras/CARRINHO-008-SEM)
