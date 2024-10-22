### Caso de Uso RF1: CRUD de Fornecedores

| Campo            | Descrição |
|------------------|-----------|
| **Nome**         | CRUD de Fornecedores |
| **Ator(es)**     | Funcionários do setor financeiro, Administradores |
| **Descrição**    | Permite a criação, edição, visualização e exclusão de fornecedores, com informações como nome, CNPJ e contato. |
| **Pré-condições**| O usuário deve estar autenticado e autorizado a acessar a seção de fornecedores. |
| **Pós-condições**| O sistema deve refletir as mudanças feitas (cadastro, atualização ou exclusão de fornecedores). |

### Fluxo Principal

1. O usuário acessa a seção de gerenciamento de fornecedores.
2. O usuário seleciona a opção de criar um novo fornecedor.
3. O usuário insere as informações do fornecedor (nome, CNPJ, telefone, e-mail).
4. O sistema valida os dados inseridos:
   - Se os dados estiverem corretos, o sistema confirma o cadastro e limpa os campos.
   - Se os dados estiverem incorretos, o sistema exibe uma mensagem de erro e solicita correção.

### Fluxos Alternativos

**Consultar Fornecedor**:
1. O usuário acessa a lista de fornecedores.
2. O sistema exibe a lista de fornecedores cadastrados.
3. O usuário pode selecionar um fornecedor para visualizar detalhes.

**Atualizar Fornecedor**:
1. O usuário seleciona um fornecedor da lista.
2. O sistema exibe os dados do fornecedor.
3. O usuário altera os dados necessários.
4. O sistema valida os dados atualizados:
   - Se os dados estiverem corretos, o sistema confirma a atualização.
   - Se os dados estiverem incorretos, o sistema exibe uma mensagem de erro e solicita correção.

**Deletar Fornecedor**:
1. O usuário seleciona um fornecedor da lista para exclusão.
2. O sistema solicita confirmação da exclusão.
3. O usuário confirma a exclusão.
4. O sistema remove o fornecedor e exibe uma mensagem de sucesso.

### Fluxos de Exceção

- **Cadastro Inválido**:
  - Se o usuário tentar cadastrar um fornecedor com um CNPJ já existente, o sistema exibe uma mensagem informando que o CNPJ já está em uso.
  
- **Erro na Consulta**:
  - Se não houver fornecedores cadastrados, o sistema exibe uma mensagem informando que não há fornecedores disponíveis.

- **Erro na Atualização**:
  - Se o usuário tentar atualizar um fornecedor com dados inválidos (como um formato de e-mail incorreto), o sistema exibe uma mensagem de erro e solicita correção.

- **Erro na Exclusão**:
  - Se o fornecedor a ser deletado não puder ser removido (por exemplo, se tiver transações pendentes), o sistema exibe uma mensagem de erro informando que a exclusão não pode ser realizada.

### Notas Adicionais

- **Segurança**: Os dados devem ser protegidos por criptografia, e o sistema deve registrar todas as operações para auditoria.
- **Validação**: O sistema deve garantir que apenas dados válidos e consistentes sejam cadastrados ou atualizados.
- **Interface do Usuário**: O sistema deve ter uma interface intuitiva, facilitando o acesso às funções de CRUD.

### Diagrama de Casos de Uso

![Diagrma1](/case01.png)