# Caso de Teste: Tentativa de cadastro preenchendo somente o campo "nome"

**ID:** CAD-CT006
**Módulo:** Cadastro  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Negativo)  

---

## Pré-condição
- O navegador deve estar aberto e o site carregado corretamente
- O usuário deve estar na tela de cadastro
- O usuário deverá tentar se cadastrar preenchendo somente o campo "nome"

---

## Dados de Entrada
| Campo  | Valor               |
|--------|---------------------|
| Nome   | Lorrany Amorim |
| E-mail | vazio |
| Senha  | vazio |

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/).
2. Navegar até a tela de **Cadastro**.
3. Preencher corretamente o campo **nome**.
4. Deixar os campos **E-mail** e **Senha** em branco**
5. Clicar no botão **"Cadastrar"**.
6. Validar se o sistema exibe a **mensagem de erro** correspondente.
7. Capturar evidência da tela

---

## Resultado Esperado
- O sistema **não deve criar um novo cadastro**.
- Deve ser exibida a seguinte mensagem de erro abaixo dos campos **E-mail e Senha"**
  > **"O campo e-mail deve ser preenchido corretamente"**
  > **O campo senha deve ter pelo menos 6 dígitos"**
- O usuário deve **permanecer na tela de cadastro** para tentar novamente.

---

## Evidência
![Erro - cadastro sem preencher campos obrigatórios](/3_Evidências/CT006.tentativa_de_cadastro_preenchendo_somente_campo_nome.JPG)