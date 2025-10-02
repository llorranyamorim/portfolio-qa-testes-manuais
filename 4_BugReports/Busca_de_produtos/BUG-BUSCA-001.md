# BUG-BUSCA-001

**Título:** Busca por produto existente exibe mensagem de sucesso, mas não redireciona para o produto específico  

**ID:** BUG-BUSCA-001  
**Módulo:** Busca  
**Prioridade:** Alta  
**Severidade:** Média (não impede uso, mas prejudica a experiência do usuário)  
**Status:** Aberto  
**Reportado por:** Lorrany Amorim de Oliveira  
**Data:** 02/10/2025  

---

## Descrição
Ao buscar o produto **"CAMISETA PARA HOMENS"** pelo nome exato, o sistema exibe a mensagem de sucesso **"Sucesso, confira os resultados"**.  
Porém, em vez de redirecionar o usuário diretamente para a página do produto, o sistema redireciona para a listagem de todos os produtos.  

---

## Pré-condições
- Usuário logado no sistema com credenciais válidas.  
- Produto **"CAMISETA PARA HOMENS"** cadastrado no catálogo.  

---

## Passos para Reproduzir
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)  
2. Fazer login no sistema.  
3. Clicar na lupa (campo de busca).  
4. Digitar **"CAMISETA PARA HOMENS"**.  
5. Clicar no botão **Procurar**.  

---

## Resultado Atual
- O sistema exibe a mensagem de sucesso **"Sucesso, confira os resultados"**.  
- Usuário é redirecionado para a **página de todos os produtos**.  

---

## Resultado Esperado
- O sistema deve exibir a mensagem de sucesso **"Sucesso, confira os resultados"**.  
- O sistema deve redirecionar o usuário diretamente para a página do produto exato pesquisado.  

---

## Evidência
📎 [Vídeo do erro](../3_Evidências/3_Busca_de_produtos/BUSCA-001-ERRO_buscar_produto_pelo_nome_existente.mp4)  

