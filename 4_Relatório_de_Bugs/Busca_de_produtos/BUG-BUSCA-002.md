# BUG-BUSCA-002

**Título:** Busca por parte do nome exibe mensagem de sucesso, mas não redireciona para o produto específico  

**ID:** BUG-BUSCA-002  
**Módulo:** Busca  
**Prioridade:** Alta  
**Severidade:** Média (não impede uso, mas prejudica a experiência do usuário)  
**Status:** Aberto  
**Reportado por:** Lorrany Amorim de Oliveira  
**Data:** 2025-10-02  

---

## Descrição
Ao buscar o produto **"CAMISETA PARA HOMENS"** utilizando apenas parte do nome (**"CAMISETA"**), o sistema exibe a mensagem de sucesso **"Sucesso, confira os resultados"**.  
Porém, em vez de mostrar os produtos filtrados ou direcionar para o item correspondente, o sistema redireciona o usuário para a listagem de **todos os produtos**.  

---

## Pré-condições
- Usuário logado no sistema com credenciais válidas.  
- Produto **"CAMISETA PARA HOMENS"** cadastrado no catálogo.  

---

## Passos para Reproduzir
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)  
2. Fazer login no sistema.  
3. Clicar na lupa (campo de busca).  
4. Digitar **"CAMISETA"** (parte do nome do produto).  
5. Clicar no botão **Procurar**.  

---

## Resultado Atual
- O sistema exibe a mensagem de sucesso **"Sucesso, confira os resultados"**.  
- Usuário é redirecionado para a **página de todos os produtos**, sem destaque para o item pesquisado.  

---

## Resultado Esperado
- O sistema deve exibir a mensagem de sucesso **"Sucesso, confira os resultados"**.  
- O sistema deve retornar somente os produtos que contenham o termo pesquisado no nome (**"CAMISETA"**).  
- O produto **"CAMISETA PARA HOMENS"** deve estar listado nos resultados.  

---

## Evidência
📎 [Vídeo do erro](/3_Evidências/3_Busca_de_produtos/BUSCA-002-ERRO_buscar_produto_por_parte_do_nome.mp4)  
