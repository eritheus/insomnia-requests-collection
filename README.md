# insomnia-requests-collection

Coleção de requisições do [Insomnia](https://insomnia.rest/) usadas para testar as APIs do projeto Eritheus.

## Conteúdo

| Arquivo | Workspace | Descrição |
|---|---|---|
| `customer-registration-api.yaml` | Customer-Registration-API | Requisições para a API de cadastro de clientes (listar, consultar health, criar cliente) |
| `product-registration-api.yaml` | Product-Registration-API | Workspace para a API de cadastro de produtos (ainda sem requisições cadastradas) |

Cada arquivo é um export no formato `collection.insomnia.rest/5.0` (schema `5.1`), contendo um workspace completo: requisições, cookie jar e environment base.

## Como importar no Insomnia

1. Abra o Insomnia.
2. Vá em **Application Menu → Preferences → Data → Import Data** (ou `Ctrl+O` / `Cmd+O`).
3. Escolha **From File** e selecione o arquivo `.yaml` desejado.
4. O workspace correspondente será criado com as requisições, environment e cookie jar já configurados.

Cada `.yaml` é um workspace independente — importe os arquivos separadamente para manter os workspaces distintos no Insomnia.

## Convenções

- Um arquivo por API/workspace, nomeado em kebab-case: `<nome-da-api>.yaml`.
- As requisições usam o ambiente de desenvolvimento (`https://dev.lowbit.com.br`) como base.
- Ao adicionar novas requisições, exporte o workspace completo do Insomnia (Export → Current Workspace → formato YAML) e substitua o arquivo correspondente.

## Como exportar alterações

1. No Insomnia, clique com o botão direito no workspace desejado.
2. Selecione **Export** → escolha o formato **Insomnia v5 (YAML)**.
3. Salve sobrescrevendo o arquivo correspondente neste repositório.
4. Faça commit da alteração.
