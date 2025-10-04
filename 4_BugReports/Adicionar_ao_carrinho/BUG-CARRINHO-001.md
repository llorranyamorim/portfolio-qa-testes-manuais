# BUG-CARRINHO-001

**Título:** Imagem e preço do produto não correspondem ao esperado ao adicionar ao carrinho

**ID:** BUG-CARRINHO-001  
**Módulo:** Carrinho de Compras  
**Prioridade:** Alta  
**Severidade:** Alta (impede a experiência correta do usuário e causa confusão)  
**Status:** Aberto  
**Reportado por:** Lorrany Amorim de Oliveira  
**Data:** 04/10/2025  

---

## Descrição
Ao adicionar o produto **"Vestido Longo"** ao carrinho, foram observados vários erros:
1. A imagem exibida do produto **"Vestido Longo"** é de um **iPhone 11**, o que gera confusão, pois a imagem não corresponde ao produto.
2. Ao tentar alterar a cor do produto, a foto muda para imagens de produtos totalmente diferentes, como **controle de PlayStation**, **PS4 com dois controles e um jogo "GTA V"**.
3. O valor do subtotal no carrinho permanece em **$0,00**, quando deveria ser atualizado para **$43,00**, que é o preço do **"Vestido Longo"**.

---

## Pré-condições
- Usuário logado no sistema com credenciais válidas.  
- Produto **"Vestido Longo"** disponível no catálogo, com imagens e preço corretos.  

---

## Passos para Reproduzir
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)  
2. Fazer login no sistema.  
3. Localizar o produto **"Vestido Longo"**.  
4. Clicar no botão **Adicionar ao Carrinho**.  
5. Tentar alterar a cor do produto.  
6. Verificar a imagem que aparece ao lado do produto e a atualização do valor no carrinho.  
7. Acessar o carrinho para verificar o subtotal.

---

## Resultado Atual
- A imagem do produto exibida é de um **iPhone 11** (não corresponde ao **Vestido Longo**).  
- Ao alterar a cor do produto, a foto muda para imagens de produtos diferentes, como **controle de PlayStation** e **PS4 com dois controles e um jogo "GTA V"**.  
- O valor do subtotal no carrinho permanece em **$0,00**, quando deveria ser **$43,00**.  

---

## Resultado Esperado
- A imagem exibida no produto **"Vestido Longo"** deve ser correta, mostrando o vestido.  
- Ao alterar a cor do produto, a imagem deve refletir a cor selecionada do **"Vestido Longo"**.  
- O valor do subtotal no carrinho deve ser atualizado corretamente para **$43,00**.

---

## Evidência  
📎 [Vídeo do erro](https://drive.google.com/file/d/1N1YQh7nKJtj_fp-IBnukKJm95jx_PYy5/view?usp=sharing)  
