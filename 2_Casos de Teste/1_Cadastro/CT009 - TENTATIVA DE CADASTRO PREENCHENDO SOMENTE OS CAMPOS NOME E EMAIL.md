# Caso de Teste: Tentativa de cadastro preenchendo somente os campos Nome e Email

**ID:** CAD-CT009
**Módulo:** Cadastro  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Negativo)  

---

## Pré-condição
- O navegador deve estar aberto
- A tela de **Cadastro** deve estar carregada corretamente e sem dados preenchidos
- Não deve existir nenhum cadastro prévio associado aos dados que serão utilizados no teste

---

## Dados de Entrada
| Campo  | Valor               |
|--------|---------------------|
| Nome   | Lorrany Amorim |
| E-mail | llorrany@teste.com |
| Senha  | vazio |

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/).
2. Navegar até a tela de **Cadastro**.
3. Preencher corretamente os campos **Nome** e **E-mail**.
4. Deixar o campo **Senha** em branco
5. Clicar no botão **"Cadastrar"**.
6. Validar se o sistema exibe a **mensagem de erro** correspondente.
7. Capturar evidência da tela

---

## Resultado Esperado
- O sistema **não deve criar um novo cadastro**.
- Deve ser exibida a seguinte mensagem de erro abaixo dos campos **Senha** 
  > **"O campo senha deve ter pelo menos 6 dígitos"**
- O usuário deve **permanecer na tela de cadastro** para tentar novamente.

---

## Evidência
![Erro - cadastro preenchendo campos nome e email](/3_Evidências/CT009.tentativa_de_cadastro_preenchendo_campos_nome_e_email.JPG)