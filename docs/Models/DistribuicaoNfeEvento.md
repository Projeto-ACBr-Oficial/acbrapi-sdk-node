# DistribuicaoNfeEvento

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **id** | **string** | ID único gerado pela API para este evento. | [opcional]  |
| **created\_at** | **Date** | Data/hora em que o evento foi criado na API. Representado no formato &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/ISO_8601\&quot; target&#x3D;\&quot;blank\&quot;&gt;&#x60;ISO 8601&#x60;&lt;/a&gt;. | [opcional]  |
| **ambiente** | **string** | Identificação do ambiente. | [opcional]  |
| **status** | **string** | Status do Evento. | [opcional]  |
| **cpf\_cnpj\_autor** | **string** | CPF/CNPJ do autor do evento. | [opcional]  |
| **chave\_acesso** | **string** | Chave de Acesso do documento vinculado ao evento. | [opcional]  |
| **tipo\_evento** | **string** | Tipo do evento vinculado. | [opcional]  |
| **data\_evento** | **Date** | Data e hora do Evento. | [opcional]  |
| **numero\_sequencial** | **number** | Sequencial do evento para o mesmo tipo de evento. | [opcional]  |
| **justificativa** | **string** | Justificativa para o desconhecimento ou não-realização da operação. | [opcional]  |
| **data\_registro** | **Date** | Data e hora do registro do evento pela SEFAZ. | [opcional]  |
| **codigo\_status** | **number** | Código do status de registro do evento. | [opcional]  |
| **motivo\_status** | **string** | Descrição literal do status do registro do evento. | [opcional]  |
| **numero\_protocolo** | **string** | Número do Protocolo de registro do evento. | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

