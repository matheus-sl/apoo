
# Documento de Requisitos

## Sistema Financeiro - Requisitos do Sistema

### Requisitos Funcionais

#### 1. CRUD de Fornecedores
**Descrição:** Permitir a criação, edição, visualização e exclusão de fornecedores com informações detalhadas, como nome, CNPJ e contato.

**Usuários:** Funcionários do setor financeiro, administradores.

**Informações de Entrada:**
- Nome do fornecedor
- CNPJ
- Telefone
- E-mail

**Informações de Saída:**
- Lista de fornecedores
- Dados atualizados do fornecedor

**Requisitos Não Funcionais:**
- Tempo de resposta rápido para operações de CRUD
- Segurança dos dados com criptografia

---

#### 2. CRUD de Despesas
**Descrição:** Permitir a criação, edição, visualização e exclusão de despesas, incluindo detalhes como data, valor, categoria e fornecedor associado.

**Usuários:** Funcionários do setor financeiro, administradores.

**Informações de Entrada:**
- Data
- Valor
- Categoria
- Fornecedor vinculado

**Informações de Saída:**
- Relatórios de despesas
- Histórico de despesas por fornecedor

**Requisitos Não Funcionais:**
- Confiabilidade dos dados armazenados
- Compatibilidade com relatórios financeiros

---

### Requisitos Suplementares

1. O sistema deve operar via interface Web.
2. Deve garantir tempo de resposta abaixo de 2 segundos para consultas frequentes.
3. Acesso restrito a dados financeiros sensíveis apenas para administradores.
4. O sistema deve estar em conformidade com a LGPD (Lei Geral de Proteção de Dados).

---

