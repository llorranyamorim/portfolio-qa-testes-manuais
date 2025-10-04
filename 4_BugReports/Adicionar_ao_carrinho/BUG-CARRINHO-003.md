# BUG-CARRINHO-003

**Título:** Adicionar o mesmo produto várias vezes não atualiza a quantidade nem o valor no carrinho

**ID:** BUG-CARRINHO-003
**Módulo:** Carrinho de Compras  
**Prioridade:** Alta  
**Severidade:** Alta (impacta diretamente a funcionalidade do carrinho e pode gerar confusão na finalização da compra)  
**Status:** Aberto  
**Reportado por:** Lorrany Amorim de Oliveira  
**Data:** 04/10/2025  

---

## Descrição
Ao adicionar o mesmo produto **"Vestido Longo"** várias vezes ao carrinho, o sistema **não atualiza a quantidade nem o valor** no carrinho. Apesar de o usuário adicionar o produto mais de uma vez, a quantidade permanece em **1** e o valor **não é somado**. O carrinho de compras não reflete corretamente a quantidade de unidades ou o total a ser pago.

---

## Pré-condições
- Usuário logado no sistema com credenciais válidas.  
- Produto **"Vestido Longo"** disponível no catálogo.  

---

## Passos para Reproduzir
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)  
2. Fazer login no sistema com e-mail e senha válidos.  
3. Localizar o produto **"Vestido Longo"**.  
4. Adicionar o produto **"Vestido Longo"** ao carrinho uma vez.  
5. Adicionar o mesmo produto ao carrinho novamente (pelo menos 2 vezes).  
6. Acessar o carrinho de compras.

---

## Resultado Atual
- O produto **"Vestido Longo"** é adicionado ao carrinho várias vezes, mas a **quantidade** e o **valor** não são atualizados.  
- O carrinho exibe apenas uma unidade do produto, e o valor do subtotal não reflete as unidades adicionadas.

---

## Resultado Esperado
- O carrinho deve **atualizar automaticamente** a quantidade de unidades do produto e somar o valor correspondente, refletindo corretamente o total de produtos e o subtotal.  
- O carrinho deve exibir a **quantidade correta** de unidades e o **valor total correto** para o produto adicionado várias vezes.

---

## Evidência  
📎 [Vídeo do erro](.https://drive.google.com/file/d/1emEaph4ES5UAjkGGgOsJOmzwRloJiULf/view?usp=sharing)  
