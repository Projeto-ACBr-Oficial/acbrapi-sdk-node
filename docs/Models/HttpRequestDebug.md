# HttpRequestDebug

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **id** | **string** | Identificador interno da requisição HTTP.    Esse identificador pode ser utilizado no endpoint  &lt;a href&#x3D;\&quot;#tag/Debug/operation/DebugHttpRequestContent\&quot;&gt;Corpo da Requisição HTTP&lt;/a&gt; ou &lt;a href&#x3D;\&quot;#tag/Debug/operation/DebugHttpResponseContent\&quot;&gt;Corpo da Resposta HTTP&lt;/a&gt;  para obter o conteúdo enviado ou recebido na comunicação com o autorizador. | [opcional]  |
| **method** | **string** | Método HTTP utilizado (ex: &#39;POST&#39;). | [opcional]  |
| **uri** | **string** | URI do serviço externo (SEFAZ, prefeitura, etc.). | [opcional]  |
| **headers** | **string** | Cabeçalhos HTTP enviados na requisição, no formato bruto. | [opcional]  |
| **response\_status\_code** | **number** | Código de status HTTP retornado (ex: 200, 403). | [opcional]  |
| **response\_status\_reason** | **string** | Motivo ou descrição do status HTTP retornado. | [opcional]  |
| **response\_headers** | **string** | Cabeçalhos retornados na resposta, no formato bruto. | [opcional]  |
| **response\_time** | **number** | Tempo de resposta do serviço externo, em milissegundos. | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

