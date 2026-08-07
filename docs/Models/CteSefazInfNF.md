# CteSefazInfNF

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **nRoma** | **string** | Número do Romaneio da NF. | [opcional]  |
| **nPed** | **string** | Número do Pedido da NF. | [opcional]  |
| **mod** | **string** | Modelo da Nota Fiscal.  Preencher com:  * 01 - NF Modelo 01/1A e Avulsa  * 04 - NF de Produtor |  |
| **serie** | **string** | Série. |  |
| **nDoc** | **string** | Número. |  |
| **dEmi** | **Date** | Data de Emissão.  Formato AAAA-MM-DD. |  |
| **vBC** | **number** | Valor da Base de Cálculo do ICMS. |  |
| **vICMS** | **number** | Valor Total do ICMS. |  |
| **vBCST** | **number** | Valor da Base de Cálculo do ICMS ST. |  |
| **vST** | **number** | Valor Total do ICMS ST. |  |
| **vProd** | **number** | Valor Total dos Produtos. |  |
| **vNF** | **number** | Valor Total da NF. |  |
| **nCFOP** | **string** | CFOP Predominante.  CFOP da NF ou, na existência de mais de um, predominância pelo critério de valor econômico. |  |
| **nPeso** | **number** | Peso total em Kg. | [opcional]  |
| **PIN** | **string** | PIN SUFRAMA.  PIN atribuído pela SUFRAMA para a operação. | [opcional]  |
| **dPrev** | **Date** | Data prevista de entrega.  Formato AAAA-MM-DD. | [opcional]  |
| **infUnidCarga** | [**Array**](CteSefazUnidCarga.md) |  | [opcional]  |
| **infUnidTransp** | [**Array**](CteSefazUnidadeTransp.md) |  | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

