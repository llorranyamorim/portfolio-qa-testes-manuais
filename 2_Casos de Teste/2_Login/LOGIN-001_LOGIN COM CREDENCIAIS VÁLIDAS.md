# Caso de Teste: Login com credenciais válidas
**ID:** LOGIN-001 
**Módulo:** Login  
**Prioridade:** Alta, pois o login é requisito essencial para acessar funcionalidades no sistema  
**Tipo de Teste:** Funcional (Caminho Feliz)  

---

## Pré-condição
- O navegador deve estar aberto e conectado à internet.    
- A tela de **Login** deve estar carregada corretamente e sem dados preenchidos  
- O usuário deve já estar cadastrado no sistema com e-mail válido

---

## Dados de Entrada
| Campo  | Valor           |
|--------|-----------------|
| E-mail | llorrany@teste.com |
| Senha  | teste12345      |

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)  
2. Navegar até a tela de **Login** localizado no canto superior direito da página inicial 
3. Preencher corretamente os campos **E-mail** e **Senha**   
4. Clicar no botão **"CONECTE-SE"**  
5. Validar se o sistema redireciona o usuário para página inicial  
6. Capturar evidência da tela confirmando o login

---

## Resultado Esperado
- O sistema deve **logar** o usuário corretamente  
- O usuário deve ser redirecionado para a **Página Inicial**.  
- O sistema deve ser exibir uma mensagem de boas-vindas com o nome do usuário logado:  
  > **"Login realizado! Olá, Lorrany"**  

---

## Evidência
![Erro-Login realizado](/3_Evidências/2_Login/LOGIN-001_Evidencia_Sucesso.JPG)
