# BUG-BUSCA-003

**Título:** Busca por produto inexistente exibe mensagem de sucesso e redireciona para todos os produtos  

**ID:** BUG-BUSCA-003  
**Módulo:** Busca  
**Prioridade:** Alta  
**Severidade:** Alta (gera informação incorreta para o usuário)  
**Status:** Aberto  
**Reportado por:** Lorrany Amorim de Oliveira  
**Data:** 2025-10-02  

---

## Descrição
Ao buscar por um produto **inexistente**, o sistema exibe a mensagem de sucesso **"Sucesso, confira os resultados"**.  
Porém, em vez de informar que não existem produtos correspondentes, o sistema redireciona o usuário para a **página de todos os produtos**.  

Esse bug é semelhante ao já identificado em:  
- **BUG-BUSCA-001** (Busca por nome exato)  
- **BUG-BUSCA-002** (Busca por parte do nome)  

---

## Pré-condições
- Usuário logado no sistema com credenciais válidas.  

---

## Passos para Reproduzir
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)  
2. Fazer login no sistema.  
3. Clicar na lupa (campo de busca).  
4. Digitar um nome inexistente, por exemplo: **"ARROZ"**.  
5. Clicar no botão **Procurar**.  

---

## Resultado Atual
- O sistema exibe a mensagem de sucesso **"Sucesso, confira os resultados"**.  
- Usuário é redirecionado para a **página de todos os produtos**, mesmo não havendo correspondência.  

---

## Resultado Esperado
- O sistema deve exibir a mensagem de erro ou alerta: **"Nenhum produto encontrado para o termo pesquisado"**.  
- Nenhum produto deve ser exibido na lista de resultados.  
- O usuário **não deve ser redirecionado** para a página de todos os produtos.  

---

## Evidência
📎 [Vídeo do erro](/3_Evidências/3_Busca_de_produtos/BUSCA-003-ERRO_burcar_produto_inexistente.mp4)  
