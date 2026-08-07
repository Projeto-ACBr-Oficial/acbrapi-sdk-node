# MdfeSefazAquav

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **irin** | **string** | Irin do navio sempre deverá ser informado. |  |
| **tpEmb** | **string** | Código do tipo de embarcação.  Preencher com código da Tabela de Tipo de Embarcação definida no Ministério dos Transportes. |  |
| **cEmbar** | **string** | Código da embarcação. |  |
| **xEmbar** | **string** | Nome da embarcação. |  |
| **nViag** | **string** | Número da Viagem. |  |
| **cPrtEmb** | **string** | Código do Porto de Embarque.  Preencher de acordo com Tabela de Portos definida no Ministério dos Transportes. |  |
| **cPrtDest** | **string** | Código do Porto de Destino.  Preencher de acordo com Tabela de Portos definida no Ministério dos Transportes. |  |
| **prtTrans** | **string** | Porto de Transbordo. | [opcional]  |
| **tpNav** | **number** | Tipo de Navegação.  Preencher com:  * 0 - Interior  * 1 - Cabotagem | [opcional]  |
| **infTermCarreg** | [**Array**](MdfeSefazInfTermCarreg.md) |  | [opcional]  |
| **infTermDescarreg** | [**Array**](MdfeSefazInfTermDescarreg.md) |  | [opcional]  |
| **infEmbComb** | [**Array**](MdfeSefazInfEmbComb.md) |  | [opcional]  |
| **infUnidCargaVazia** | [**Array**](MdfeSefazInfUnidCargaVazia.md) |  | [opcional]  |
| **infUnidTranspVazia** | [**Array**](MdfeSefazInfUnidTranspVazia.md) |  | [opcional]  |
| **MMSI** | **string** | Maritime Mobile Service Identify.  Preencher com o MMSI (Maritime Mobile Service Identify) fornecido pela ANATEL ou autoridade de telecomunicações de origem da embarcação. | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

