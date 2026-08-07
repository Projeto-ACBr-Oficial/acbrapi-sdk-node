# DistribuicaoNfe

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **id** | **string** | ID único gerado pela API para o pedido de distribuição. |  |
| **created\_at** | **Date** | Data/hora em que o pedido foi criado na API. Representado no formato &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/ISO_8601\&quot; target&#x3D;\&quot;blank\&quot;&gt;&#x60;ISO 8601&#x60;&lt;/a&gt;. | [opcional]  |
| **status** | **string** | Indica o status da distribuição. |  |
| **ambiente** | **string** | Identificação do Ambiente. |  |
| **uf\_autor** | **string** | Sigla da UF do autor. | [opcional]  |
| **tipo\_consulta** | **string** |  |  |
| **dist\_nsu** | **number** | Distribuição de conjunto de DF-e a partir do NSU informado.    *Obrigatório quando &#x60;tipo_consulta&#x60; for &#x60;distNSU&#x60;.* | [opcional]  |
| **cons\_nsu** | **number** | Consulta DF-e vinculado ao NSU informado.    *Obrigatório quando &#x60;tipo_consulta&#x60; for &#x60;consNSU&#x60;.* | [opcional]  |
| **cons\_chave** | **string** | Consulta de NF-e por chave de acesso informada.    *Obrigatório quando &#x60;tipo_consulta&#x60; for &#x60;consChNFe&#x60;.* | [opcional]  |
| **codigo\_status** | **number** | Código do status de processamento da requisição. |  |
| **motivo\_status** | **string** | Descrição do status de processamento da requisição. | [opcional]  |
| **data\_hora\_resposta** | **Date** | Data e Hora de processamento da requisição. |  |
| **ultimo\_nsu** | **number** | Último NSU pesquisado no Ambiente Nacional. Se for o caso, o solicitante pode continuar a consulta a partir deste NSU para obter novos resultados. |  |
| **max\_nsu** | **number** | Maior NSU existente no Ambiente Nacional para o CNPJ/CPF informado. |  |
| **documentos** | [**Array**](DistribuicaoNfeDocumento.md) | Conjunto de informações resumidas e documentos fiscais eletrônicos de interesse da pessoa ou empresa. | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

