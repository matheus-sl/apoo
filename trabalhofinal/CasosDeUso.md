## Especificação dos Casos de Uso

### Caso de Uso UC01: CRUD de Usuários

| Campo            | Descrição |
|------------------|-----------|
| **Nome**         | CRUD de Usuários |
| **Ator(es)**     | Administrador, Usuário |
| **Descrição**    | Permite ao administrador cadastrar, atualizar, consultar e deletar informações de usuários. |
| **Pré-condições**| O sistema deve estar no modo Administrador. |
| **Pós-condições**| Não há. |
| **Fluxo Principal** | 1. O administrador insere o nome, login e senha do usuário para cadastro. 2. O sistema confirma o cadastro e limpa os campos. |
| **Fluxos Alternativos** | **Consultar**:  1. O administrador insere o nome ou código do usuário a buscar. 2. O sistema exibe a lista dos usuários encontrados. **Atualizar**: 1. O administrador seleciona um usuário e altera os dados. 2. O sistema confirma a atualização. **Deletar**: 1. O administrador seleciona um usuário para exclusão. 2. O sistema confirma a exclusão. |

![Diagrma1](/case01.png)


### Caso de Uso UC02: CRUD de Notas Fiscais

| Campo            | Descrição |
|------------------|-----------|
| **Nome**         | CRUD de Notas Fiscais |
| **Ator(es)**     | Administrador, Sistema |
| **Descrição**    | Permite ao administrador cadastrar, atualizar, consultar e deletar notas fiscais de aquisição. |
| **Pré-condições**| O sistema deve estar no modo Administrador. |
| **Pós-condições**| Não há. |
| **Fluxo Principal** | 1. O administrador insere informações da nota fiscal para cadastro. 2. O sistema confirma o cadastro e limpa os campos. |
| **Fluxos Alternativos** | **Consultar**: 1. O administrador insere dados para busca da nota fiscal. 2. O sistema exibe as notas fiscais encontradas. **Atualizar**: 1. O administrador altera dados de uma nota. 2. O sistema confirma a atualização. **Deletar**: 1. O administrador exclui uma nota fiscal. 2. O sistema confirma a exclusão. |

![Diagrma2](/case02.png)

### Caso de Uso UC03: CRUD de Mercadorias

| Campo            | Descrição |
|------------------|-----------|
| **Nome**         | CRUD de Mercadorias |
| **Ator(es)**     | Administrador, Sistema |
| **Descrição**    | Permite ao administrador cadastrar, atualizar, consultar e deletar informações de mercadorias. |
| **Pré-condições**| O sistema deve estar no modo Administrador. |
| **Pós-condições**| Não há. |
| **Fluxo Principal** | 1. O administrador insere o nome ou código da mercadoria. 2. O sistema confirma o cadastro e limpa os campos. |
| **Fluxos Alternativos** | **Consultar**: 1. O administrador realiza busca de mercadorias. 2. O sistema exibe as mercadorias encontradas. **Atualizar**: 1. O administrador altera informações de uma mercadoria. 2. O sistema confirma a atualização. **Deletar**: 1. O administrador exclui uma mercadoria. 2. O sistema confirma a exclusão. |

![Diagrma3](/case03.png)

### Caso de Uso UC04: CRUD de Fornecedores

| Campo            | Descrição |
|------------------|-----------|
| **Nome**         | CRUD de Fornecedores |
| **Ator(es)**     | Administrador, Sistema |
| **Descrição**    | Permite ao administrador cadastrar, atualizar, consultar e deletar informações de fornecedores. |
| **Pré-condições**| O sistema deve estar no modo Administrador. |
| **Pós-condições**| Não há. |
| **Fluxo Principal** | 1. O administrador insere informações do fornecedor para cadastro. 2. O sistema confirma o cadastro e limpa os campos. |
| **Fluxos Alternativos** | **Consultar**: 1. O administrador insere dados para busca do fornecedor. 2. O sistema exibe os fornecedores encontrados. **Atualizar**: 1. O administrador altera informações de um fornecedor. 2. O sistema confirma a atualização. **Deletar**: 1. O administrador exclui um fornecedor. 2. O sistema confirma a exclusão. |

![Diagrma4](/case04.png)

### Caso de Uso UC05: Abertura do Caixa

| Campo            | Descrição |
|------------------|-----------|
| **Nome**         | Abertura do Caixa |
| **Ator(es)**     | Usuário, Sistema |
| **Descrição**    | Permite ao usuário abrir o caixa com saldo inicial do dia. |
| **Pré-condições**| O sistema deve estar no modo Administrador ou Usuário. |
| **Pós-condições**| Não há. |
| **Fluxo Principal** | 1. O usuário insere o saldo inicial e abre o caixa. <br> 2. O sistema confirma a operação. |

![Diagrma5](/case05.png)

### Caso de Uso UC06: Controle de Vendas e Caixa

| Campo            | Descrição |
|------------------|-----------|
| **Nome**         | Controle de Vendas e Caixa |
| **Ator(es)**     | Usuário, Sistema |
| **Descrição**    | Permite ao usuário realizar vendas e controlar o caixa. |
| **Pré-condições**| O sistema deve estar no modo Administrador ou Usuário. |
| **Pós-condições**| Não há. |
| **Fluxo Principal** | 1. O usuário insere produtos e quantidade para a venda. 2. O sistema soma o valor total e confirma a venda. 3. O estoque é atualizado. |

![Diagrma6](/case06.png)

### Caso de Uso UC07: Fechamento do Caixa

| Campo            | Descrição |
|------------------|-----------|
| **Nome**         | Fechamento do Caixa |
| **Ator(es)**     | Usuário, Sistema |
| **Descrição**    | Permite o fechamento do caixa com saldo final do dia. |
| **Pré-condições**| O sistema deve estar no modo Administrador ou Usuário. |
| **Pós-condições**| Não há. |
| **Fluxo Principal** | 1. O sistema exibe o saldo final. 2. O usuário confirma o fechamento do caixa. |

![Diagrma7](/case07.png)

### Caso de Uso UC08: Relatório de Estoque

| Campo            | Descrição |
|------------------|-----------|
| **Nome**         | Relatório de Estoque |
| **Ator(es)**     | Administrador, Sistema |
| **Descrição**    | Gera relatório de estoque com status de cada produto. |
| **Pré-condições**| Cadastro de Mercadorias |
| **Pós-condições**| Não há. |
| **Fluxo Principal** | 1. O administrador seleciona a filtragem e emite o relatório. 2. O sistema realiza a impressão. |

![Diagrma8](/case08.png)

### Caso de Uso UC09: Relatório de Vendas

| Campo            | Descrição |
|------------------|-----------|
| **Nome**         | Relatório de Vendas |
| **Ator(es)**     | Administrador, Sistema |
| **Descrição**    | Gera relatório de vendas de acordo com o período selecionado. |
| **Pré-condições**| Cadastro de Mercadorias |
| **Pós-condições**| Não há. |
| **Fluxo Principal** | 1. O administrador escolhe a filtragem. 2. O sistema exibe e imprime o relatório. |

![Diagrma9](/case09.png)

### Caso de Uso UC10: Relatório Financeiro

| Campo            | Descrição |
|------------------|-----------|
| **Nome**         | Relatório Financeiro |
| **Ator(es)**     | Administrador, Sistema |
| **Descrição**    | Gera relatório financeiro contendo entradas, saídas e balanço final. |
| **Pré-condições**| Realização de vendas, controle de estoque, cadastro de notas fiscais. |
| **Pós-condições**| Não há. |
| **Fluxo Principal** | 1. O administrador escolhe a filtragem e confirma a emissão. 2. O sistema exibe e imprime o relatório financeiro. |

![Diagrma10](/case10.png)
