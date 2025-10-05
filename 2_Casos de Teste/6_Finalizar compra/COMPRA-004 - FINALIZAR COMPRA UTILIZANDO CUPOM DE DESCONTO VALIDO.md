# Caso de Teste: Finalizar compra e receber e-mail de confirmação

**ID:** COMPRA-007  
**Módulo:** Finalização de Compra  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Positivo)

---

## Pré-condições
- Usuário logado no sistema com credenciais válidas.  
- O carrinho deve conter pelo menos um produto adicionado.  
- O sistema deve ser configurado para enviar e-mails de confirmação.

---

## Passos para Reproduzir
1. Acessar a URL: [Loja Online](https://www.automationpratice.com.br/)  
2. Fazer login no sistema com e-mail e senha válidos.  
3. Adicionar um produto ao carrinho.  
4. Acessar a página de **Finalização de Compra**.  
5. Finalizar a compra com os dados válidos.  
6. Verificar a caixa de entrada do e-mail associado à conta.

---

## Resultado Esperado
- O sistema deve enviar um **e-mail de confirmação** de compra para o usuário, com detalhes da compra, incluindo o número do pedido e os produtos comprados.

---

## Evidência  
📎 [Evidência da execução do teste](./3_Evidências/3_Finalizacao_de_Compra/COMPRA-007-EMAIL_CONFIRMACAO.mp4)
