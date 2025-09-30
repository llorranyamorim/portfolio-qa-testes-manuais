# Caso de Teste: Login com senha incorreta
**ID:** LOGIN-002 
**Módulo:** Login  
**Prioridade:** Alta, pois o login é requisito essencial para acessar funcionalidades no sistema  
**Tipo de Teste:** Funcional (Negativo)  

---

## Pré-condição
- O navegador deve estar aberto e conectado à internet.    
- A tela de **Login** deve estar carregada corretamente e sem dados preenchidos  
- O usuário de teste **llorrany@teste.com**, deve estar cadastrado no sistema com senha válida **(teste12345)**.

---

## Dados de Entrada
| Campo  | Valor           | Obervação |
|--------|-----------------|-----------|
| E-mail | llorrany@teste.com | Usuário Válido |
| Senha  | teste@123#      | Senha inválida (não cadastrada)

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)  
2. Navegar até a tela de **Login** localizado no canto superior direito da página inicial 
3. Preencher corretamente o campo **E-mail** com llorrany@teste.com 
4. Preencher o campo **Senha** com teste@123# (senha inválida)  
5. Clicar no botão **"CONECTE-SE"**  
6. Validar se o sistema exibe a **mensagem de erro** correspondente.
7. Capturar evidência da tela

---

## Resultado Esperado
- O sistema não deve permitir o **login** do usuário    
- O sistema deve exibir uma mensagem clara informando erro de autenticação 
> **"(ex: Senha incorreta)"**  
 

---

## Evidência
![Erro-Login realizado](/3_Evidências/2_Login/LOGIN-002_Evidencia_Senha_Incorreta.JPG)
