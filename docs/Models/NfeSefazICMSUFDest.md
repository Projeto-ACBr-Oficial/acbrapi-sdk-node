# NfeSefazICMSUFDest

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **vBCUFDest** | **number** | Valor da Base de Cálculo do ICMS na UF do destinatário. |  |
| **vBCFCPUFDest** | **number** | Valor da Base de Cálculo do FCP na UF do destinatário. | [opcional]  |
| **pFCPUFDest** | **number** | Percentual adicional inserido na alíquota interna da UF de destino, relativo ao Fundo de Combate à Pobreza (FCP) naquela UF. | [opcional]  |
| **pICMSUFDest** | **number** | Alíquota adotada nas operações internas na UF do destinatário para o produto / mercadoria. |  |
| **pICMSInter** | **number** | Alíquota interestadual das UF envolvidas:  * 4%% alíquota interestadual para produtos importados  * 7%% para os Estados de origem do Sul e Sudeste (exceto ES), destinado para os Estados do Norte e Nordeste  ou ES  * 12%% para os demais casos. |  |
| **pICMSInterPart** | **number** | Percentual de partilha para a UF do destinatário:  * 40%% em 2016  * 60%% em 2017  * 80%% em 2018  * 100%% a partir de 2019. |  |
| **vFCPUFDest** | **number** | Valor do ICMS relativo ao Fundo de Combate à Pobreza (FCP) da UF de destino. | [opcional]  |
| **vICMSUFDest** | **number** | Valor do ICMS de partilha para a UF do destinatário. |  |
| **vICMSUFRemet** | **number** | Valor do ICMS de partilha para a UF do remetente. Nota: A partir de 2019, este valor será zero. |  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

