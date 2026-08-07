# NfeSefazDetPag

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **indPag** | **number** | Indicador da Forma de Pagamento:0-Pagamento à Vista  * 1 - Pagamento à Prazo | [opcional]  |
| **tPag** | **string** | Forma de Pagamento:. |  |
| **xPag** | **string** | Descrição do Meio de Pagamento. | [opcional]  |
| **vPag** | **number** | Valor do Pagamento. Esta tag poderá ser omitida quando a tag tPag&#x3D;90 (Sem Pagamento), caso contrário deverá ser preenchida. |  |
| **dPag** | **Date** | Data do Pagamento. | [opcional]  |
| **CNPJPag** | **string** | CNPJ transacional do pagamento - Preencher informando o CNPJ do estabelecimento onde o pagamento foi processado/transacionado/recebido quando a emissão do documento fiscal ocorrer em estabelecimento distinto. | [opcional]  |
| **UFPag** | **string** | UF do CNPJ do estabelecimento onde o pagamento foi processado/transacionado/recebido. | [opcional]  |
| **card** | [**NfeSefazCard**](NfeSefazCard.md) |  | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

