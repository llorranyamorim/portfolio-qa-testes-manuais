# Caso de Teste: Fazer login com o botão "ENTER" do teclado

**ID:** LOGIN-006  
**Módulo:** Login  
**Prioridade:** Média  
**Tipo de Teste:** Funcional (Alternativo)  

---

## Pré-condições
- O navegador deve estar aberto e conectado à internet.  
- O usuário deve estar na tela de login
- O usuário deve preencher os campos **E-mail** e **Senha** com credenciais válidas

## Dados de Entrada
| Campo  | Valor           |
|--------|-----------------|
| E-mail | llorrany@teste.com |
| Senha  | teste12345 |

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)  
2. Navegar até a tela de **Login** localizado no canto superior direito da página inicial 
3. Preencher o campo **E-mail** com o e-mail "llorrany@teste.com"
4. Preencher o campo **Senha** com a senha "teste12345"
5. Pressionar o botão **ENTER** do teclado  
6. Validar se o sistema redireciona o usuário para página inicial
7. Capturar evidência da tela

---

## Resultado Esperado
- O sistema deve **logar** o usuário corretamente  
- O usuário deve ser redirecionado para a **Página Inicial**.  
- O sistema deve ser exibir uma mensagem de boas-vindas com o nome do usuário logado:  
  > **"Login realizado! Olá, Lorrany"** 

---

## Evidência
![Erro! login usando o botão enter](/3_Evidências/2_Login/LOGIN-006_Fazer_login_usando_o_botão_enter.JPG)
