# Caso de Teste: Tentativa de cadastro preenchendo somente o campo "E-mail"

**ID:** CAD-CT007
**Módulo:** Cadastro  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Negativo)  

---

## Pré-condição
- O navegador deve estar aberto e o site carregado corretamente
- O usuário deve estar na tela de cadastro
- O usuário deverá tentar se cadastrar preenchendo somente o campo "E-mail"

---

## Dados de Entrada
| Campo  | Valor               |
|--------|---------------------|
| Nome   | vazio |
| E-mail | llorranya@teste.com |
| Senha  | vazio |

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/).
2. Navegar até a tela de **Cadastro**.
3. Preencher corretamente o campo **E-mail**.
4. Deixar os campos **Nome** e **Senha** em branco**
5. Clicar no botão **"Cadastrar"**.
6. Validar se o sistema exibe a **mensagem de erro** correspondente.
7. Capturar evidência da tela

---

## Resultado Esperado
- O sistema **não deve criar um novo cadastro**.
- Deve ser exibida a seguinte mensagem de erro abaixo dos campos **Nome** e **Senha"**
  > **"O campo Nome deve ser preenchido"**
  > **O campo senha deve ter pelo menos 6 dígitos"**
- O usuário deve **permanecer na tela de cadastro** para tentar novamente.

---

## Evidência
![Erro - cadastro sem preencher campos obrigatórios](/3_Evidências/CT007.JPG)