# MdfeInclusaoDfe

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **codigo\_municipio\_carrega** | **string** | Código do Município de carregamento. | [opcional]  |
| **municipio\_carrega** | **string** | Nome do Município de carregamento. | [opcional]  |
| **documentos** | [**Array**](MdfeDocumentoVinculado.md) | Informações dos documentos fiscais vinculados ao manifesto. | [opcional]  |
| **id** | **string** | ID único gerado pela API para este evento. | [opcional]  |
| **ambiente** | **string** | Identificação do ambiente. | [opcional]  |
| **status** | **string** | Status do Evento. | [opcional]  |
| **autor** | [**DfeAutorEvento**](DfeAutorEvento.md) |  | [opcional]  |
| **chave\_acesso** | **string** | Chave de Acesso do documento vinculado ao evento. | [opcional]  |
| **data\_evento** | **Date** | Data e hora do Evento. | [opcional]  |
| **numero\_sequencial** | **number** | Sequencial do evento para o mesmo tipo de evento. | [opcional]  |
| **data\_recebimento** | **Date** | Data e hora do recebimento do Evento pela SEFAZ. | [opcional]  |
| **codigo\_status** | **number** | Código do status de registro do Evento. | [opcional]  |
| **motivo\_status** | **string** | Descrição literal do status do registro do Evento. | [opcional]  |
| **numero\_protocolo** | **string** | Número do Protocolo de registro do Evento. | [opcional]  |
| **codigo\_mensagem** | **number** | Código da Mensagem. | [opcional]  |
| **mensagem** | **string** | Mensagem da SEFAZ para o emissor. | [opcional]  |
| **tipo\_evento** | **string** |  | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

