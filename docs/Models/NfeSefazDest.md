# NfeSefazDest

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **CNPJ** | **string** | Número do CNPJ. | [opcional]  |
| **CPF** | **string** | Número do CPF. | [opcional]  |
| **idEstrangeiro** | **string** | Identificador do destinatário, em caso de comprador estrangeiro. | [opcional]  |
| **xNome** | **string** | Razão Social ou nome do destinatário. | [opcional]  |
| **enderDest** | [**NfeSefazEndereco**](NfeSefazEndereco.md) |  | [opcional]  |
| **indIEDest** | **number** | Indicador da IE do destinatário:  * 1 - Contribuinte ICMSpagamento à vista  * 2 - Contribuinte isento de inscrição  * 9 - Não Contribuinte |  |
| **IE** | **string** | Inscrição Estadual (obrigatório nas operações com contribuintes do ICMS). | [opcional]  |
| **ISUF** | **string** | Inscrição na SUFRAMA (Obrigatório nas operações com as áreas com benefícios de incentivos fiscais sob controle da SUFRAMA) PL_005d - 11/08/09 - alterado para aceitar 8 ou 9 dígitos. | [opcional]  |
| **IM** | **string** | Inscrição Municipal do tomador do serviço. | [opcional]  |
| **email** | **string** | Informar o e-mail do destinatário. O campo pode ser utilizado para informar o e-mail  de recepção da NF-e indicada pelo destinatário. | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

