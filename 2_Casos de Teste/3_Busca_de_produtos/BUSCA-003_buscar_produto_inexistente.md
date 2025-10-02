# Caso de Teste: Buscar produto inexistente

**ID:** BUSCA-003  
**Módulo:** Busca  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Negativo)  

---

## Pré-condições
- O navegador deve estar aberto e conectado à internet.  
- O usuário deve estar logado no sistema com credenciais válidas.  

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)  
2. Fazer login usando e-mail e senha válidos.  
3. Localizar o campo de busca (ícone da lupa).  
4. Digitar um nome de produto inexistente, por exemplo: **"ARROZ"**.  
5. Clicar no botão **Procurar**.  

---

## Resultado Esperado
- O sistema deve exibir uma mensagem informando que **nenhum produto foi encontrado** para o termo pesquisado.  
- A lista de resultados deve estar **vazia**.  
- O usuário não deve ser redirecionado para a página de todos os produtos.  

---

## Evidência
📎 [Evidência da execução do teste](/3_Evidências/3_Busca_de_produtos/BUSCA-003-ERRO_burcar_produto_inexistente.mp4)  
