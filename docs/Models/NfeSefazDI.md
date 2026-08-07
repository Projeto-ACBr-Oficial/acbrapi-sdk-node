# NfeSefazDI

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **nDI** | **string** | Número do Documento de Importação (DI, DSI, DIRE, DUImp) (NT2011/004). |  |
| **dDI** | **Date** | Data de registro da DI/DSI/DA (AAAA-MM-DD). |  |
| **xLocDesemb** | **string** | Local do desembaraço aduaneiro. |  |
| **UFDesemb** | **string** | UF onde ocorreu o desembaraço aduaneiro. |  |
| **dDesemb** | **Date** | Data do desembaraço aduaneiro (AAAA-MM-DD). |  |
| **tpViaTransp** | **number** | Via de transporte internacional informada na DI ou na Declaração Única de Importação (DUImp):  * 1 - Maritima  * 2 - Fluvial  * 3 - Lacustre  * 4 - Aerea  * 5 - Postal  * 6 - Ferroviaria  * 7 - Rodoviaria  * 8 - Conduto  * 9 - Meios Proprios  * 10 - Entrada/Saida Ficta  * 11 - Courier  * 12 - Em maos  * 13 - Por reboque |  |
| **vAFRMM** | **number** | Valor Adicional ao frete para renovação de marinha mercante. | [opcional]  |
| **tpIntermedio** | **number** | Forma de Importação quanto a intermediação  * 1 - por conta propria  * 2 - por conta e ordem  * 3 - encomenda |  |
| **CNPJ** | **string** | CNPJ do adquirente ou do encomendante. | [opcional]  |
| **CPF** | **string** | CPF do adquirente ou do encomendante. | [opcional]  |
| **UFTerceiro** | **string** | Sigla da UF do adquirente ou do encomendante. | [opcional]  |
| **cExportador** | **string** | Código do exportador (usado nos sistemas internos de informação do emitente da NF-e). |  |
| **adi** | [**Array**](NfeSefazAdi.md) |  |  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

