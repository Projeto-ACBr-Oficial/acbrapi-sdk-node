# MdfeSefazInfResp

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **respSeg** | **number** | Responsável pelo seguro.  Preencher com:  * 1 - Emitente do MDF-e  * 22 - Responsável pela contratação do serviço de transporte (contratante)  Dados obrigatórios apenas no modal Rodoviário, depois da lei 11.442/07. Para os demais modais esta informação é opcional. |  |
| **CNPJ** | **string** | Número do CNPJ do responsável pelo seguro.  Obrigatório apenas se responsável pelo seguro for (2) responsável pela contratação do transporte - pessoa jurídica. | [opcional]  |
| **CPF** | **string** | Número do CPF do responsável pelo seguro.  Obrigatório apenas se responsável pelo seguro for (2) responsável pela contratação do transporte - pessoa física. | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

