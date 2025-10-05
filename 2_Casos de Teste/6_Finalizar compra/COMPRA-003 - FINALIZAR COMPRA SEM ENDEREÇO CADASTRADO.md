# Caso de Teste: Finalizar compra sem endereço cadastrado

**ID:** COMPRA-003  
**Módulo:** Finalização de Compra  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Negativo)

---

## Pré-condições
- Usuário logado no sistema com credenciais válidas.  
- O carrinho deve conter pelo menos um produto adicionado.  
- O endereço do usuário não está cadastrado.

---

## Passos para Reproduzir
1. Acessar a URL: [Loja Online](https://www.automationpratice.com.br/)  
2. Fazer login no sistema com e-mail e senha válidos.  
3. Adicionar um produto ao carrinho.  
4. Acessar a página de **Finalização de Compra**.  
5. Tentar prosseguir para a finalização sem um endereço cadastrado.

---

## Resultado Esperado
- O sistema deve solicitar que o usuário adicione ou cadastre um endereço de entrega antes de finalizar a compra.  
- O usuário não deve conseguir concluir a compra sem fornecer um endereço válido.

---

## Evidência  
📎 [Evidência da execução do teste](./3_Evidências/3_Finalizacao_de_Compra/COMPRA-003-SEM_ENDERECO.mp4)
