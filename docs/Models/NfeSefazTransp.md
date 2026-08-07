# NfeSefazTransp

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **modFrete** | **number** | Modalidade do frete  * 0 - Contratação do Frete por conta do Remetente (CIF)  * 1 - Contratação do Frete por conta do destinatário/remetente (FOB)  * 2 - Contratação do Frete por conta de terceiros  * 3 - Transporte próprio por conta do remetente  * 4 - Transporte próprio por conta do destinatário  * 9 - Sem Ocorrência de transporte |  |
| **transporta** | [**NfeSefazTransporta**](NfeSefazTransporta.md) |  | [opcional]  |
| **retTransp** | [**NfeSefazRetTransp**](NfeSefazRetTransp.md) |  | [opcional]  |
| **veicTransp** | [**NfeSefazVeiculo**](NfeSefazVeiculo.md) |  | [opcional]  |
| **reboque** | [**Array**](NfeSefazVeiculo.md) |  | [opcional]  |
| **vagao** | **string** | Identificação do vagão (v2.0). | [opcional]  |
| **balsa** | **string** | Identificação da balsa (v2.0). | [opcional]  |
| **vol** | [**Array**](NfeSefazVol.md) |  | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

