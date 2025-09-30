# Caso de Teste: Cadastro de usuário com e-mail inválido (formato incorreto)

**ID:** CAD-CT005
**Módulo:** Cadastro  
**Prioridade:** Alta  
**Tipo de Teste:** Funcional (Negativo)  

---

## Pré-condição
- O usuário deve estar na tela de cadastro
- O usuário preencherá o campo com e-mail inválido (formato incorreto)

---

## Dados de Entrada
| Campo  | Valor               |
|--------|---------------------|
| Nome   | Lorrany Amorim |
| E-mail | llorrany@ |
| Senha  | teste12345 |

---

## Passos
1. Acessar a URL: [Automation Practice](https://www.automationpratice.com.br/).
2. Navegar até a tela de **Cadastro**.
3. Preencher corretamente o campo **nome**.
4. Preencher o campo **e-mail** com um e-mail inválido.
5. Preencher o campo **senha** corretamente.
6. Clicar no botão **"Cadastrar"**.
7. Validar se o sistema exibe a **mensagem de erro** correspondente.

---

## Resultado Esperado
- O sistema **não deve criar um novo cadastro**.
- Deve ser exibida a seguinte mensagem de erro abaixo do campo **E-mail"**
  > **"O campo e-mail deve ser preenchido corretamente"**
- O usuário deve **permanecer na tela de cadastro** para tentar novamente.

---

## Evidência
![Erro - cadastro sem preencher campos obrigatórios](/3_Evidências/CT005.JPG)