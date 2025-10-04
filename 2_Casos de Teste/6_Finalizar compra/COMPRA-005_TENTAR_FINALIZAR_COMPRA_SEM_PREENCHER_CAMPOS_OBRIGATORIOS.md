# Caso de Teste: Tentar finalizar compra sem preencher campos obrigatórios

**ID:** COMPRA-008  
**Módulo:** Finalização de Compra  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Negativo)

---

## Pré-condições
- Usuário logado no sistema com credenciais válidas.  
- O carrinho deve conter pelo menos um produto adicionado.  
- O sistema deve exigir preenchimento de campos obrigatórios (por exemplo: dados de pagamento, endereço de entrega, etc).

---

## Passos para Reproduzir
1. Acessar a URL: [Loja Online](https://www.automationpratice.com.br/)  
2. Fazer login no sistema com e-mail e senha válidos.  
3. Adicionar um produto ao carrinho.  
4. Acessar a página de **Finalização de Compra**.  
5. Tentar prosseguir para a finalização da compra **sem preencher os campos obrigatórios** (como endereço de entrega, dados de pagamento, etc).
6. Clicar no botão **Finalizar Compra**.

---

## Resultado Atual
- O sistema deve exibir mensagens de erro indicando que os **campos obrigatórios** não foram preenchidos.  
- O usuário deve ser impedido de continuar a compra até que todos os campos obrigatórios sejam preenchidos corretamente.  
- O sistema não deve permitir que a compra seja finalizada sem esses dados.

---

## Resultado Esperado
- O sistema deve **bloquear** a finalização da compra até que todos os campos obrigatórios sejam preenchidos corretamente.  
- O sistema deve exibir **mensagens de erro claras** sobre quais campos precisam ser preenchidos.

---

## Evidência  
📎 [Evidência da execução do teste](./3_Evidências/3_Finalizacao_de_Compra/COMPRA-008-CAMPO_OBRIGATORIO_FALTANDO.mp4)
