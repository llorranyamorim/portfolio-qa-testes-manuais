# BUG-CARRINHO-009

**Título:** Produto adicionado ao carrinho sem selecionar tamanho/cor obrigatórios

**ID:** BUG-CARRINHO-009  
**Módulo:** Carrinho de Compras  
**Prioridade:** Alta  
**Severidade:** Alta (impede a experiência correta do usuário e pode levar a erros no processamento do pedido)  
**Status:** Aberto  
**Reportado por:** Lorrany Amorim de Oliveira  
**Data:** 04/10/2025  

---

## Descrição
O sistema permitiu que o produto **"Vestido Longo"** fosse adicionado ao carrinho sem que o usuário selecionasse as opções obrigatórias de **tamanho** e **cor**. Essas opções são essenciais para a compra do produto e, apesar de serem obrigatórias, o sistema não bloqueou a ação de adicionar o produto ao carrinho.  

---

## Pré-condições
- Usuário logado no sistema com credenciais válidas.  
- Produto **"Vestido Longo"** disponível no catálogo, com opções de tamanho e cor obrigatórias.

---

## Passos para Reproduzir
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)  
2. Fazer login no sistema com e-mail e senha válidos.  
3. Localizar o produto **"Vestido Longo"** com opções de **tamanho** e **cor** obrigatórias.  
4. Tentar adicionar o produto ao carrinho sem selecionar o tamanho e a cor.  
5. Clicar no botão **Adicionar ao Carrinho**.

---

## Resultado Atual
- O sistema permite que o produto seja adicionado ao carrinho **sem selecionar o tamanho ou a cor obrigatória**.  
- Não há mensagem de erro ou bloqueio da ação, e o produto é adicionado ao carrinho sem essas informações obrigatórias.

---

## Resultado Esperado
- O sistema deve **bloquear** a adição do produto ao carrinho **até que as opções de tamanho e cor obrigatórias sejam selecionadas**.  
- O sistema deve exibir uma mensagem clara informando ao usuário que a seleção dessas opções é necessária para prosseguir.

---

## Evidência  
📎 [Vídeo do erro](https://drive.google.com/file/d/1_7ltVIC7xPwXbx9s-rG0FIYIG7QSLVhB/view?usp=sharing)  
