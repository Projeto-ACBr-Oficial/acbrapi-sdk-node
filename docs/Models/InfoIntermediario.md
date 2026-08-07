# InfoIntermediario

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **CNPJ** | **string** | Número do CNPJ. | [opcional]  |
| **CPF** | **string** | Número do CPF. | [opcional]  |
| **NIF** | **string** | Número de Identificação Fiscal fornecido por órgão de administração tributária no exterior. | [opcional]  |
| **cNaoNIF** | **number** | Motivo para não informação do NIF:  * 0 - Não informado na nota de origem  * 1 - Dispensado do NIF  * 2 - Não exigência do NIF | [opcional]  |
| **CAEPF** | **string** | Número do Cadastro de Atividade Econômica da Pessoa Física (CAEPF). | [opcional]  |
| **IM** | **string** | Número da inscrição municipal. | [opcional]  |
| **IE** | **string** | Número da inscrição estadual.    **Atenção**: Para emissões pelo Sistema Nacional NFS-e, esse campo é ignorado. | [opcional]  |
| **xNome** | **string** | Nome/Nome Empresarial. |  |
| **end** | [**Endereco**](Endereco.md) |  | [opcional]  |
| **fone** | **string** | Número do telefone do prestador:  Preencher com o Código DDD + número do telefone.  Nas operações com exterior é permitido informar o código do país + código da localidade + número do telefone). | [opcional]  |
| **email** | **string** | * E-mail | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

