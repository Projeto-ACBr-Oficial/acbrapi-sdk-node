# DfeContribuinteInfCad

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **ie** | **string** | Número da Inscrição Estadual do contribuinte. |  |
| **cnpj** | **string** | Número do CNPJ  do contribuinte. | [opcional]  |
| **cpf** | **string** | Número do CPF do contribuinte. | [opcional]  |
| **uf** | **string** | Sigla da UF de localização do contribuinte. Em algumas situações, a UF de localização pode ser diferente da UF consultada. Ex. IE de Substituto Tributário. |  |
| **situacao\_cadastral** | **number** | Situação cadastral do contribuinte:  * 0 - não habilitado  * 1 - habilitado |  |
| **indicador\_nfe** | **number** | Indicador de contribuinte credenciado a emitir NF-e.  * 0 - Não credenciado para emissão da NF-e  * 1 - Credenciado  * 2 - Credenciado com obrigatoriedade para todas operações  * 3 - Credenciado com obrigatoriedade parcial  * 4 - a SEFAZ não fornece a informação  Este indicador significa apenas que o contribuinte é credenciado para emitir NF-e na SEFAZ consultada. |  |
| **indicador\_cte** | **number** | Indicador de contribuinte credenciado a emitir CT-e.  * 0 - Não credenciado para emissão da CT-e  * 1 - Credenciado  * 2 - Credenciado com obrigatoriedade para todas operações  * 3 - Credenciado com obrigatoriedade parcial  * 4 - a SEFAZ não fornece a informação  Este indicador significa apenas que o contribuinte é credenciado para emitir CT-e na SEFAZ consultada. |  |
| **nome\_razao\_social** | **string** | Razão Social ou nome do contribuinte. |  |
| **nome\_fantasia** | **string** | Razão Social ou nome do contribuinte. | [opcional]  |
| **regime\_apuracao\_icms** | **string** | Regime de Apuração do ICMS. | [opcional]  |
| **cnae** | **string** | CNAE Fiscal do contribuinte. | [opcional]  |
| **data\_inicio\_atividade** | **Date** | Data de início de atividades do contribuinte. | [opcional]  |
| **data\_situacao\_cadastral** | **Date** | Data da última modificação da situação cadastral do contribuinte. | [opcional]  |
| **data\_fim\_atividade** | **Date** | Data de ocorrência da baixa do contribuinte. | [opcional]  |
| **ie\_unica** | **string** | Inscrição Estadual Única. | [opcional]  |
| **ie\_atual** | **string** | Inscrição Estadual atual. | [opcional]  |
| **endereco** | [**DfeContribuinteEndereco**](DfeContribuinteEndereco.md) |  | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

