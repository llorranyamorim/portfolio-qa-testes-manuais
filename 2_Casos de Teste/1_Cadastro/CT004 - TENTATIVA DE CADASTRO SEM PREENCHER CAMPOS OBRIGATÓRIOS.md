# Caso de Teste: Tentativa de cadastro sem preencher campos obrigatórios

**ID:** CAD-CT004
**Módulo:** Cadastro  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Negativo)  

---

## Pré-condição
- O usuário deve estar na tela de cadastro
- O usuário deverá tentar se cadastrar sem preencher os campos obrigatórios: "nome, e-mail e senha"

---

## Dados de Entrada
| Campo  | Valor               |
|--------|---------------------|
| Nome   | vazio |
| E-mail | vazio |
| Senha  | vazio |

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/)
2. Navegar até a tela de **Cadastro**.
3. Sem preencher nenhum campo obrigatório, Clicar no botão **"Cadastrar"**.
4. Validar se o sistema exibe as **mensagens de erro** correspondentes.

---

## Resultado Esperado
- O sistema **não deve criar um novo cadastro**.
- Deve ser exibida a seguinte mensagem de erro abaixo do campo "nome":
  > **"O campo nome deve ser prenchido"**
  > **"O campo e-mail deve ser preenchido"**
  > **"O campo senha deve ser preenchido"**
- O usuário deve **permanecer na tela de cadastro** para tentar novamente.

---

## Evidência
![Erro - cadastro sem preencher campos obrigatórios](/3_Evidências/CT004-tentativa_de_cadastro_sem_preencher_campos_obrigatorio.JPG)