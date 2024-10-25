### Caso de Uso: Gerenciar Fornecedores

**Ator Principal:** Funcionário do Setor Financeiro, Administrador

**Pré-condições:**
- O ator principal deve estar autenticado no sistema.
- O sistema deve estar acessível por meio de uma interface web.

**Fluxo Principal:**
1. [IN] O usuário acessa o módulo de gerenciamento de fornecedores.
2. [OUT] O sistema exibe a lista de fornecedores existentes.
3. [IN] O usuário seleciona a opção de criar, editar, visualizar ou excluir um fornecedor.
   - **3a. Criar fornecedor:** O usuário insere as informações necessárias (nome, CNPJ, telefone, e-mail) e confirma.
   - **3b. Editar fornecedor:** O usuário seleciona um fornecedor da lista, faz as alterações necessárias e confirma.
   - **3c. Visualizar fornecedor:** O usuário escolhe um fornecedor para ver os detalhes completos.
   - **3d. Excluir fornecedor:** O usuário escolhe um fornecedor para remoção e confirma a exclusão.
4. [OUT] O sistema salva as alterações e exibe uma mensagem de sucesso.

**Pós-condições:**
- O sistema atualiza os dados dos fornecedores de acordo com a operação realizada (inclusão, edição ou exclusão).

**Exceções:**
- **Exceção 3a.1 - Dados obrigatórios incompletos:**
  - [OUT] O sistema informa que campos obrigatórios não foram preenchidos.
  - [IN] O usuário preenche os campos obrigatórios.
  - Volta ao passo 4.
- **Exceção 3b.1 - CNPJ inválido ou duplicado:**
  - [OUT] O sistema informa que o CNPJ é inválido ou já existe no sistema.
  - [IN] O usuário insere um CNPJ válido e não cadastrado.
  - Volta ao passo 4.
- **Exceção 3d.1 - Exclusão de fornecedor com vínculos ativos:**
  - [OUT] O sistema informa que o fornecedor possui vínculos e não pode ser excluído.
  - [IN] O usuário opta por cancelar a operação ou desvincular o fornecedor.
  - Volta ao passo 4, caso desvincule o fornecedor. 