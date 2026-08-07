# RTCListaDoc

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **dFeNacional** | [**RTCListaDocDFe**](RTCListaDocDFe.md) |  | [opcional]  |
| **docFiscalOutro** | [**RTCListaDocFiscalOutro**](RTCListaDocFiscalOutro.md) |  | [opcional]  |
| **docOutro** | [**RTCListaDocOutro**](RTCListaDocOutro.md) |  | [opcional]  |
| **fornec** | [**RTCListaDocFornec**](RTCListaDocFornec.md) |  | [opcional]  |
| **dtEmiDoc** | **Date** | Data da emissão do documento dedutível  Ano, mês e dia (AAAA-MM-DD). |  |
| **dtCompDoc** | **Date** | Data da competência do documento dedutível  Ano, mês e dia (AAAA-MM-DD). |  |
| **tpReeRepRes** | **string** | Tipo de valor incluído neste documento, recebido por motivo de estarem relacionadas a operações de terceiros,  objeto de reembolso, repasse ou ressarcimento pelo recebedor, já tributados e aqui referenciados. |  |
| **xTpReeRepRes** | **string** | Descrição do reembolso ou ressarcimento quando a opção é  \&quot;99 - Outros reembolsos ou ressarcimentos recebidos por valores pagos relativos a operações por conta e ordem de terceiro\&quot;. | [opcional]  |
| **vlrReeRepRes** | **number** | Valor monetário (total ou parcial, conforme documento informado) utilizado para não inclusão na base de cálculo  do ISS e do IBS e da CBS da NFS-e que está sendo emitida (R$). |  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

