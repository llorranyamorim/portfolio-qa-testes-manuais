# Caso de Teste: Cadastrar usuário com caracteres especiais no campo Nome

**ID:** CAD-CT012  
**Módulo:** Cadastro  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Alternativo)  

---

## Pré-condição
- O navegador deve estar aberto e conectado à internet.  
- O ambiente de testes deve estar ativo e acessível.  
- A tela de **Cadastro** deve estar carregada corretamente e sem dados preenchidos.  
- Não deve existir nenhum cadastro prévio associado aos dados que serão utilizados no teste.

---

## Dados de Entrada
| Campo  | Valor           |
|--------|-----------------|
| Nome   | José D'Ávila    |
| E-mail | llorrany@teste.com |
| Senha  | teste12345      |

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/).  
2. Navegar até a tela de **Cadastro**.  
3. Preencher corretamente os campos **E-mail** e **Senha**.  
4. Preencher o campo **Nome** utilizando caracteres especiais: `José D'Ávila`.  
5. Clicar no botão **"Cadastrar"**.  
6. Validar se o sistema cadastra o usuário com sucesso.  
7. Capturar evidência da tela confirmando o cadastro.

---

## Resultado Esperado
- O sistema deve **criar o cadastro** do usuário corretamente.  
- O usuário deve ser redirecionado para a **Página Inicial**.  
- Deve ser exibida a mensagem de sucesso:  
  > **"Cadastro realizado! Bem-vindo, José D'Ávila"**  
- Os dados devem ser salvos corretamente na base de dados e vinculados ao novo usuário.

---

## Evidência
![Cadastro com caracteres especiais no nome realizado com sucesso](/3_Evidências/CT012.cadastro_com_caracteres_especiais_no_nome.JPG)
