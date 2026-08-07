# CteOsSefazInfCteOS

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **versao** | **string** | Versão do leiaute.  Ex: \&quot;4.00\&quot;. |  |
| **Id** | **string** | Identificador da tag a ser assinada.  Informar a chave de acesso do CT-e OS e precedida do literal \&quot;CTe\&quot;.    *Geramos automaticamente quando nenhum valor é informado.* | [opcional]  |
| **ide** | [**CteOsSefazIdeOS**](CteOsSefazIdeOS.md) |  |  |
| **compl** | [**CteOsSefazComplOS**](CteOsSefazComplOS.md) |  | [opcional]  |
| **emit** | [**CteOsSefazEmitOS**](CteOsSefazEmitOS.md) |  |  |
| **toma** | [**CteOsSefazTomaOS**](CteOsSefazTomaOS.md) |  | [opcional]  |
| **vPrest** | [**CteOsSefazVPrestOS**](CteOsSefazVPrestOS.md) |  |  |
| **imp** | [**CteOsSefazInfCte_ImpOS**](CteOsSefazInfCte_ImpOS.md) |  |  |
| **pgtoVinc** | [**CteOsSefazPgtoVincOS**](CteOsSefazPgtoVincOS.md) |  | [opcional]  |
| **infCTeNorm** | [**CteOsSefazInfCTeNormOS**](CteOsSefazInfCTeNormOS.md) |  | [opcional]  |
| **infCteComp** | [**Array**](CteOsSefazInfCteCompOS.md) |  | [opcional]  |
| **autXML** | [**Array**](CteOsSefazAutXMLOS.md) |  | [opcional]  |
| **infRespTec** | [**CteOsSefazRespTecOS**](CteOsSefazRespTecOS.md) |  | [opcional]  |
| **tpPagAnt** | **number** | Tipo Pagamento ou Pagamento Antecipado.  Informar:  * 1 - Pagamento Antecipado  * 3 - Fornecimento com pagamento realizado anteriormente  Este campo é opcional e apenas deve ser informado quando pagamento que ocorre antes da prestação do serviço e na DFe de fornecimento associada a esses pagamentos, demais hipóteses de prestação de serviço sem antecipação não devem preencher. | [opcional]  |
| **gPagAntecipado** | [**CteOsSefazGPagAntecipadoOS**](CteOsSefazGPagAntecipadoOS.md) |  | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

