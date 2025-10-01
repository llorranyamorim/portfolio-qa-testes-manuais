# Caso de Teste: Login sem preencher os campos obrigatórios

**ID:** LOGIN-005  
**Módulo:** Login  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Negativo)  

---

## Pré-condições
- O navegador deve estar aberto e conectado à internet.  
- O usuário deve estar na tela de login

## Dados de Entrada
| Campo  | Valor           |
|--------|-----------------|
| E-mail | vazio |
| Senha  | vazio |  

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)  
2. Navegar até a tela de **Login** localizado no canto superior direito da página inicial 
3. Deixar campos **E-mail** e **Senha** em branco
4. Clicar no botão **"CONECTE-SE"**  
5. Validar se o sistema exibe a **mensagem de erro** correspondente.
6. Capturar evidência da tela

---

## Resultado Esperado
- O sistema não deve permitir o **login** do usuário    
- O sistema deve exibir uma mensagem clara informando que os campos obrigatórios não foram preenchidos, por exemplo: 
(**O campo E-mail é obrigatório"**)
(**O campo Senha é obrigatório"**) 
-O usuário deve permanecer na tela de login

---

## Evidência
![Erro! Login sem preencher os campos obrigatórios](/3_Evidências/2_Login/LOGIN-005_Login_sem_prencher_campos_obrigatórios.JPG)
