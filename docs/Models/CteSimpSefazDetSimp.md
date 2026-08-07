# CteSimpSefazDetSimp

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **nItem** | **number** | Número identificador do item agrupador da prestação. |  |
| **cMunIni** | **string** | Código do Município de início da prestação.  Utilizar a tabela do IBGE. Informar 9999999 para operações com o exterior. |  |
| **xMunIni** | **string** | Nome do Município do início da prestação.  Informar &#39;EXTERIOR&#39; para operações com o exterior. |  |
| **cMunFim** | **string** | Código do Município de término da prestação.  Utilizar a tabela do IBGE. Informar 9999999 para operações com o exterior. |  |
| **xMunFim** | **string** | Nome do Município do término da prestação.  Informar &#39;EXTERIOR&#39; para operações com o exterior. |  |
| **vPrest** | **number** | Valorl da Prestação do Serviço.  Pode conter zeros quando o CT-e for de complemento de ICMS. |  |
| **vRec** | **number** | Valor a Receber. |  |
| **Comp** | [**Array**](CteSimpSefazCompSimp.md) |  | [opcional]  |
| **infNFe** | [**Array**](CteSimpSefazInfNFeSimp.md) |  | [opcional]  |
| **infDocAnt** | [**Array**](CteSimpSefazInfDocAntSimp.md) |  | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

