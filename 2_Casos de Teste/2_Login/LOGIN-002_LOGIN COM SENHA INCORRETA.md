# Caso de Teste: Login com senha incorreta
**ID:** LOGIN-002 
**Módulo:** Login  
**Prioridade:** Alta, pois o login é requisito essencial para acessar funcionalidades no sistema  
**Tipo de Teste:** Funcional (Negativo)  

---

## Pré-condição
- O navegador deve estar aberto e conectado à internet.    
- A tela de **Login** deve estar carregada corretamente e sem dados preenchidos  
- O usuário deve estar cadastrado no sistema com e-mail e senha válidos

---

## Dados de Entrada
| Campo  | Valor           |
|--------|-----------------|
| E-mail | llorrany@teste.com |
| Senha  | teste@123#      |

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)  
2. Navegar até a tela de **Login** localizado no canto superior direito da página inicial 
3. Preencher corretamente os campos **E-mail** 
4. Preencher o campo **Senha** com uma senha que não foi cadastrada no sistema  
5. Clicar no botão **"CONECTE-SE"**  
6. Validar se o sistema exibe a **mensagem de erro** correspondente.
7. Capturar evidência da tela

---

## Resultado Esperado
- O sistema deve não deve**logar** o usuário    
- O sistema deve ser exibir uma mensagem de erro:  
  > **"Senha incorreta"**  

---

## Evidência
![Erro-Login realizado](/3_Evidências/2_Login/LOGIN-002_Login_com_senha_incorreta.JPG)
