# Caso de Teste: Finalizar compra com dados válidos (cartão de crédito)

**ID:** COMPRA-001  
**Módulo:** Finalização de Compra  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Positivo)

---

## Pré-condições
- Usuário logado no sistema com credenciais válidas.  
- O carrinho deve conter pelo menos um produto adicionado.  
- O sistema deve aceitar pagamento via cartão de crédito.

---

## Passos para Reproduzir
1. Acessar a URL: [Loja Online](https://www.automationpratice.com.br/)  
2. Fazer login no sistema com e-mail e senha válidos.  
3. Adicionar pelo menos um produto ao carrinho.  
4. Acessar a página de **Finalização de Compra**.  
5. Inserir os dados de pagamento válidos (cartão de crédito).  
6. Confirmar o endereço de entrega.  
7. Clicar no botão **Finalizar Compra**.

---

## Resultado Esperado
- O sistema deve processar o pagamento com os dados válidos do cartão de crédito.  
- O sistema deve exibir uma mensagem de sucesso indicando que a compra foi concluída com êxito.  
- O pedido deve ser registrado no sistema.

---

## Evidência  
📎 [Evidência da execução do teste](./3_Evidências/3_Finalizacao_de_Compra/COMPRA-001-DADOS_VALIDOS.mp4)
