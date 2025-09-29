# Cenários de Teste - E-commerce

Este documento contém os cenários de teste para as seguintes funcionalidades:
- **Cadastro**
- **Entrar/Sair (Login e Logout)**
- **Busca de Produtos**
- **Adicionar ao Carrinho**
- **Finalizar Compra**

Cada funcionalidade contém **10 cenários**, contemplando:
- **Caminho Feliz** ✅  
- **Alternativos** 🔄  
- **Negativos** ❌  

---

## **1. Cadastro**

| ID | Cenário | Tipo | Pré-condição | Resultado Esperado |
|----|---------|------|--------------|--------------------|
| CAD-001 | Cadastrar usuário com todos os campos obrigatórios válidos | ✅ Caminho feliz | Usuário acessa a tela de cadastro | Cadastro realizado com sucesso e mensagem de confirmação exibida |
| CAD-002 | Cadastrar usuário com e-mail já existente | ❌ Negativo | Já existe um usuário com o mesmo e-mail no sistema | Mensagem informando que o e-mail já está cadastrado |
| CAD-003 | Tentar cadastrar com senha fraca (ex: "12345") | ❌ Negativo | - | Mensagem de erro informando que a senha não atende aos critérios |
| CAD-004 | Cadastrar usuário sem preencher campos obrigatórios | ❌ Negativo | - | Mensagem destacando os campos obrigatórios não preenchidos |
| CAD-005 | Cadastrar usuário com e-mail inválido (ex: "usuario@") | ❌ Negativo | - | Mensagem de erro solicitando e-mail válido |
| CAD-006 | Cadastrar usuário com caracteres especiais no nome | 🔄 Alternativo | - | Cadastro realizado com sucesso aceitando caracteres como “José D’Ávila” |
| CAD-007 | Cadastrar com CPF inválido (quando aplicável) | ❌ Negativo | - | Sistema deve recusar CPF inválido e exibir mensagem |
| CAD-008 | Cadastrar usuário maior que 18 anos | ✅ Caminho feliz | Usuário informa data de nascimento válida | Cadastro realizado com sucesso |
| CAD-009 | Cadastrar usuário menor de 18 anos (quando não permitido) | ❌ Negativo | - | Mensagem informando que o cadastro não é permitido para menores |
| CAD-010 | Cadastrar usuário com dados opcionais preenchidos | 🔄 Alternativo | - | Cadastro concluído com sucesso, incluindo informações opcionais |

---

## **2. Entrar/Sair (Login e Logout)**

| ID | Cenário | Tipo | Pré-condição | Resultado Esperado |
|----|---------|------|--------------|--------------------|
| LOGIN-001 | Login com credenciais válidas | ✅ Caminho feliz | Usuário já cadastrado | Sistema autentica e redireciona para página inicial |
| LOGIN-002 | Login com senha incorreta | ❌ Negativo | Usuário cadastrado | Mensagem de erro: "Senha incorreta" |
| LOGIN-003 | Login com e-mail não cadastrado | ❌ Negativo | - | Mensagem de erro: "Usuário não encontrado" |
| LOGIN-004 | Logout após login bem-sucedido | ✅ Caminho feliz | Usuário logado | Sistema encerra a sessão e retorna à tela inicial |
| LOGIN-005 | Login sem preencher os campos obrigatórios | ❌ Negativo | - | Sistema bloqueia login e solicita preenchimento dos campos |
| LOGIN-006 | Login com e-mail em letras maiúsculas | 🔄 Alternativo | Usuário cadastrado com e-mail em minúsculas | Login realizado com sucesso (case insensitive) |
| LOGIN-007 | Login usando botão "Enter" do teclado | 🔄 Alternativo | Usuário cadastrado | Sistema deve autenticar normalmente |
| LOGIN-008 | Tentativa de login após 5 falhas consecutivas | ❌ Negativo | Usuário errou senha 5 vezes | Conta temporariamente bloqueada |
| LOGIN-009 | Login em múltiplos dispositivos simultaneamente | 🔄 Alternativo | Usuário já logado em outro dispositivo | Sistema permite ou exibe aviso, conforme política |
| LOGIN-010 | Logout em aba do navegador sem encerrar sessão em outra | 🔄 Alternativo | Usuário logado em várias abas | Sessão permanece ativa nas demais abas |

---

## **3. Busca de Produtos**

| ID | Cenário | Tipo | Pré-condição | Resultado Esperado |
|----|---------|------|--------------|--------------------|
| BUSCA-001 | Buscar produto existente pelo nome exato | ✅ Caminho feliz | Produto cadastrado no sistema | Produto é exibido na lista de resultados |
| BUSCA-002 | Buscar produto por parte do nome | 🔄 Alternativo | Produto cadastrado no sistema | Lista com resultados aproximados |
| BUSCA-003 | Buscar produto inexistente | ❌ Negativo | Produto não cadastrado | Mensagem: "Nenhum produto encontrado" |
| BUSCA-004 | Buscar usando categoria | ✅ Caminho feliz | Categorias cadastradas | Produtos relacionados à categoria exibidos |
| BUSCA-005 | Buscar utilizando filtro de preço | 🔄 Alternativo | Produtos cadastrados | Apenas produtos dentro do intervalo aparecem |
| BUSCA-006 | Buscar com caracteres especiais (ex: "Tênis nº 42") | 🔄 Alternativo | Produto cadastrado | Sistema reconhece e retorna resultados corretos |
| BUSCA-007 | Buscar sem preencher campo de pesquisa | ❌ Negativo | - | Mensagem: "Digite algo para buscar" |
| BUSCA-008 | Buscar produto com conexão lenta | 🔄 Alternativo | Internet instável | Sistema exibe mensagem de carregamento até concluir |
| BUSCA-009 | Buscar com termos genéricos (ex: "camisa") | 🔄 Alternativo | Diversos produtos cadastrados | Sistema retorna lista extensa com paginação |
| BUSCA-010 | Buscar e aplicar múltiplos filtros (preço + categoria) | ✅ Caminho feliz | Produtos cadastrados | Sistema retorna resultados conforme critérios combinados |

---

## **4. Adicionar ao Carrinho**

| ID | Cenário | Tipo | Pré-condição | Resultado Esperado |
|----|---------|------|--------------|--------------------|
| CARR-001 | Adicionar produto disponível ao carrinho | ✅ Caminho feliz | Produto em estoque | Produto adicionado com sucesso |
| CARR-002 | Adicionar produto sem selecionar tamanho/cor obrigatório | ❌ Negativo | Produto com variação | Sistema exibe mensagem solicitando seleção |
| CARR-003 | Adicionar produto fora de estoque | ❌ Negativo | Produto sem estoque | Sistema bloqueia ação e exibe aviso |
| CARR-004 | Adicionar múltiplas unidades do mesmo produto | ✅ Caminho feliz | Produto em estoque | Quantidade atualizada corretamente no carrinho |
| CARR-005 | Adicionar produto e continuar navegando | 🔄 Alternativo | - | Produto permanece salvo no carrinho |
| CARR-006 | Adicionar produto com valor promocional | 🔄 Alternativo | Promoção ativa | Valor atualizado corretamente |
| CARR-007 | Adicionar produtos diferentes ao carrinho | ✅ Caminho feliz | Produtos em estoque | Carrinho exibe todos os itens corretamente |
| CARR-008 | Remover produto do carrinho | ✅ Caminho feliz | Produto já no carrinho | Produto removido corretamente |
| CARR-009 | Carrinho esvaziado automaticamente após logout | 🔄 Alternativo | Usuário desloga após adicionar produtos | Carrinho vazio ao relogar, se regra definida |
| CARR-010 | Adicionar produto ao carrinho sem estar logado | 🔄 Alternativo | Usuário visitante | Sistema salva em sessão temporária ou solicita login |

---

## **5. Finalizar Compra**

| ID | Cenário | Tipo | Pré-condição | Resultado Esperado |
|----|---------|------|--------------|--------------------|
| CHECK-001 | Finalizar compra com dados válidos (cartão de crédito) | ✅ Caminho feliz | Produtos no carrinho | Compra finalizada e pedido confirmado |
| CHECK-002 | Finalizar compra via PIX | ✅ Caminho feliz | Produtos no carrinho | QR Code gerado e pedido aguardando pagamento |
| CHECK-003 | Tentar finalizar compra sem produtos no carrinho | ❌ Negativo | Carrinho vazio | Sistema bloqueia ação e exibe aviso |
| CHECK-004 | Finalizar compra sem endereço cadastrado | ❌ Negativo | - | Sistema solicita cadastro de endereço |
| CHECK-005 | Finalizar compra com cartão inválido | ❌ Negativo | Cartão inválido | Mensagem: "Pagamento não autorizado" |
| CHECK-006 | Finalizar compra com frete grátis aplicado | 🔄 Alternativo | Regra ativa | Frete exibido como "Grátis" |
| CHECK-007 | Finalizar compra utilizando cupom de desconto válido | ✅ Caminho feliz | Cupom ativo | Valor do pedido atualizado corretamente |
| CHECK-008 | Tentar finalizar compra com cupom expirado | ❌ Negativo | Cupom inválido | Mensagem: "Cupom inválido ou expirado" |
| CHECK-009 | Finalizar compra com conexão instável | 🔄 Alternativo | Internet instável | Sistema salva estado e permite retomar |
| CHECK-010 | Finalizar compra e receber e-mail de confirmação | ✅ Caminho feliz | E-mail válido cadastrado | Confirmação enviada para o e-mail informado |

---

## **Legenda**
- ✅ **Caminho Feliz:** Cenário padrão que representa a funcionalidade funcionando como esperado.  
- 🔄 **Alternativo:** Fluxos diferentes que também devem ser validados.  
- ❌ **Negativo:** Cenários que testam falhas ou erros no sistema.  
