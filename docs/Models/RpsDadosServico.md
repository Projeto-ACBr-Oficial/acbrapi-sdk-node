# RpsDadosServico

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **iss\_retido** | **boolean** | Reter ISSQN. | [opcional]  |
| **responsavel\_retencao** | **number** | Responsável pela retenção:  * 0 - Prestador;  * 1 - Tomador;  * 2 - Intermediário. | [opcional]  |
| **item\_lista\_servico** | **string** | Código do item da lista de serviço, geralmente segue a LC116, podendo variar de acordo com a prefeitura.    Você pode encontrar esse dado no portal da prefeitura, em uma nota emitida ou junto ao contador. |  |
| **codigo\_cnae** | **string** | Código CNAE (Classificação Nacional de Atividades Econômicas). | [opcional]  |
| **codigo\_tributacao\_municipio** | **string** | Código de tributação do município. | [opcional]  |
| **discriminacao** | **string** | Detalhamento do serviço prestado. |  |
| **codigo\_municipio** | **string** | Código IBGE do município de prestação do serviço.  Caso não informado, será considerado o município do prestador. | [opcional]  |
| **codigo\_pais** | **string** | Código do país de prestação do serviço. | [opcional]  |
| **tipo\_tributacao** | **number** | Tipo de Tributação do Serviço:  * 1 - Isento de ISS  * 2 - Imune  * 3 - Não Incidência no Município  * 4 - Não Tributável  * 5 - Retido  * 6 - Tributável Dentro do Município  * 7 - Tributável Fora do Município  * 8 - Tributável Dentro do Município pelo tomador | [opcional]  |
| **exigibilidade\_iss** | **number** | Exigibilidade do ISS:  * 1 - Exigível  * 2 - Não Incidência  * 3 - Isenção  * 4 - Exportação  * 5 - Imunidade  * 6 - Suspenso por Decisão Judicial  * 7 - Suspenso por Processo Administrativo | [opcional]  |
| **codigo\_municipio\_incidencia** | **string** | Código IBGE do município de incidência do ISSQN. | [opcional]  |
| **numero\_processo** | **string** | Número do Processo de Suspensão da Exigibilidade. | [opcional]  |
| **unidade** | **string** | Unidade do serviço prestado. | [opcional]  |
| **quantidade** | **number** | Quantidade dos serviços prestados. | [opcional]  |
| **valores** | [**RpsServicoValores**](RpsServicoValores.md) |  |  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

