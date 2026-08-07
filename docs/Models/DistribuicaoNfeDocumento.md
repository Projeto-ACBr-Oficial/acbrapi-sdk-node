# DistribuicaoNfeDocumento

## Propriedades

| Nome | Tipo | Descrição | Comentários |
|------------ | ------------- | ------------- | -------------|
| **id** | **string** | ID único gerado pela API para identificar o documento. |  |
| **created\_at** | **Date** | Data/hora em que o documento foi criado na API. Representado no formato &lt;a href&#x3D;\&quot;https://en.wikipedia.org/wiki/ISO_8601\&quot; target&#x3D;\&quot;blank\&quot;&gt;&#x60;ISO 8601&#x60;&lt;/a&gt;. | [opcional]  |
| **nsu** | **number** | NSU do documento fiscal. | [opcional]  |
| **schema** | **string** | Identificação do Schema XML que será utilizado para validar o XML existente no conteúdo da tag docZip. Vai identificar o tipo do documento e sua versão. Exemplos: resNFe_v1.00.xsd, procNFe_v3.10.xsd, resEvento_1.00.xsd, procEventoNFe_v1.00.xsd. |  |
| **tipo\_documento** | **string** | Tipo do documento de interesse da pessoa ou empresa. | [opcional]  |
| **chave\_acesso** | **string** | Chave de Acesso da NF-e. | [opcional]  |
| **resumo** | **boolean** | Indica se o documento distribuído está em sua forma resumida. | [opcional]  |
| **tipo\_evento** | **string** | Tipo do evento. | [opcional]  |
| **numero\_sequencial** | **number** | Número sequencial do evento para o mesmo tipo de evento. | [opcional]  |
| **data\_evento** | **Date** | Data e hora do evento. | [opcional]  |
| **data\_recebimento** | **Date** | Data e hora de autorização do evento. | [opcional]  |
| **numero\_protocolo** | **string** | Número do protocolo de autorização. | [opcional]  |
| **tipo\_nfe** | **number** | Tipo da NF-e (0 - entrada; 1 - saída). | [opcional]  |
| **valor\_nfe** | **number** | Valor total da NF-e. | [opcional]  |
| **digest\_value** | **string** | Digest Value da NF-e processada. Utilizado para conferir a integridade da NF-e original. | [opcional]  |
| **emitente\_cpf\_cnpj** | **string** | CPF/CNPJ do emitente. | [opcional]  |
| **emitente\_nome\_razao\_social** | **string** | Nome ou Razão Social do emitente. | [opcional]  |
| **emitente\_inscricao\_estadual** | **string** | Inscrição Estadual do emitente. | [opcional]  |

[[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar ao README]](../README.md)

