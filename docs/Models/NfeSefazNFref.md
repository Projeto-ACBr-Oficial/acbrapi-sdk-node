# NfeSefazNFref

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **refNFe** | **string** | Chave de acesso das NF-e referenciadas. Chave de acesso compostas por Código da UF (tabela do IBGE) + AAMM da emissão + CNPJ do Emitente + modelo, série e número da NF-e Referenciada + Código Numérico + DV. | [opcional]  |
| **refNFeSig** | **string** | Referencia uma NF-e (modelo 55) emitida anteriormente pela sua Chave de Acesso com código numérico zerado, permitindo manter o sigilo da NF-e referenciada. | [opcional]  |
| **refNF** | [**NfeSefazRefNF**](NfeSefazRefNF.md) |  | [opcional]  |
| **refNFP** | [**NfeSefazRefNFP**](NfeSefazRefNFP.md) |  | [opcional]  |
| **refCTe** | **string** | Utilizar esta TAG para referenciar um CT-e emitido anteriormente, vinculada a NF-e atual. | [opcional]  |
| **refECF** | [**NfeSefazRefECF**](NfeSefazRefECF.md) |  | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

