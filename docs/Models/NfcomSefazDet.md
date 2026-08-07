# NfcomSefazDet

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **nItem** | **number** | Número do item da NFCom. |  |
| **chNFComAnt** | **string** | Chave de Acesso da NFCom anterior.  Informar chave de acesso de referencia anterior  TAG OPCIONAL, DEVE SER INFORMADA APENAS NOS CASOS PREVISTOS DE NOTA ANTERIOR REFERENCIADA. | [opcional]  |
| **nItemAnt** | **string** | Número do item da NFCom anterior.  Informar nro do item da chave de acesso de referencia anterior  TAG OPCIONAL, DEVE SER INFORMADA APENAS NOS CASOS PREVISTOS DE NOTA ANTERIOR REFERENCIADA. | [opcional]  |
| **indNFComAntPapelFatCentral** | **number** | Indicador de Nota anterior em papel no faturamento centralizado.  Informa que a NFCom Anterior de Faturamento centralizado não é eletrônica. | [opcional]  |
| **prod** | [**NfcomSefazProd**](NfcomSefazProd.md) |  |  |
| **imposto** | [**NfcomSefazImposto**](NfcomSefazImposto.md) |  |  |
| **gProcRef** | [**NfcomSefazGProcRef**](NfcomSefazGProcRef.md) |  | [opcional]  |
| **gRessarc** | [**NfcomSefazGRessarc**](NfcomSefazGRessarc.md) |  | [opcional]  |
| **infAdProd** | **string** | Informações adicionais do produto (norma referenciada, informações complementares, etc). | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

