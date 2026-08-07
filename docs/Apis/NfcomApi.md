# NfcomApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**baixarPdfNfcom**](NfcomApi.md#baixarPdfNfcom) | **GET** /nfcom/{id}/pdf | Baixar PDF do DANFE-COM |
| [**baixarXmlCancelamentoNfcom**](NfcomApi.md#baixarXmlCancelamentoNfcom) | **GET** /nfcom/{id}/cancelamento/xml | Baixar XML do cancelamento |
| [**baixarXmlNfcom**](NfcomApi.md#baixarXmlNfcom) | **GET** /nfcom/{id}/xml | Baixar XML da NFCom processada |
| [**baixarXmlNfcomNota**](NfcomApi.md#baixarXmlNfcomNota) | **GET** /nfcom/{id}/xml/nota | Baixar XML da NFCom |
| [**baixarXmlNfcomProtocolo**](NfcomApi.md#baixarXmlNfcomProtocolo) | **GET** /nfcom/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ |
| [**cancelarNfcom**](NfcomApi.md#cancelarNfcom) | **POST** /nfcom/{id}/cancelamento | Cancelar uma NFCom autorizada |
| [**consultarCancelamentoNfcom**](NfcomApi.md#consultarCancelamentoNfcom) | **GET** /nfcom/{id}/cancelamento | Consultar o cancelamento da NFCom |
| [**consultarNfcom**](NfcomApi.md#consultarNfcom) | **GET** /nfcom/{id} | Consultar NFCom |
| [**consultarStatusSefazNfcom**](NfcomApi.md#consultarStatusSefazNfcom) | **GET** /nfcom/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora |
| [**emitirNfcom**](NfcomApi.md#emitirNfcom) | **POST** /nfcom | Emitir NFCom |
| [**listarNfcom**](NfcomApi.md#listarNfcom) | **GET** /nfcom | Listar NFCom |


<a name="baixarPdfNfcom"></a>
# **baixarPdfNfcom**
> Blob baixarPdfNfcom(id, logotipo)

Baixar PDF do DANFE-COM

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFCom gerado pela API. | |
| **logotipo** | **boolean**| Imprime o documento com logotipo, desde que esteja cadastrado na empresa. | [opcional] |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCancelamentoNfcom"></a>
# **baixarXmlCancelamentoNfcom**
> Blob baixarXmlCancelamentoNfcom(id)

Baixar XML do cancelamento

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFCom gerada pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlNfcom"></a>
# **baixarXmlNfcom**
> Blob baixarXmlNfcom(id)

Baixar XML da NFCom processada

    Utilize esse endpoint para obter o XML da nota enviada para a SEFAZ, complementado com a informação do protocolo de autorização de uso (TAG raiz &#x60;nfcomProc&#x60;).    O XML só estará disponível nesse endpoint caso a nota tenha sido autorizada pela SEFAZ. Para obter o XML nos demais casos, utilize o endpoint &#x60;GET /nfcom/{id}/xml/nota&#x60;.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFCom gerada pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlNfcomNota"></a>
# **baixarXmlNfcomNota**
> Blob baixarXmlNfcomNota(id)

Baixar XML da NFCom

    Utilize esse endpoint para obter o XML da nota enviada para a SEFAZ.    O XML estará disponível nesse endpoint mesmo em casos que a nota tenha sido rejeitada.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFCom gerada pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlNfcomProtocolo"></a>
# **baixarXmlNfcomProtocolo**
> Blob baixarXmlNfcomProtocolo(id)

Baixar XML do Protocolo da SEFAZ

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFCom gerada pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="cancelarNfcom"></a>
# **cancelarNfcom**
> DfeCancelamento cancelarNfcom(id, body)

Cancelar uma NFCom autorizada

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFCom gerada pela API. | |
| **body** | [**NfcomPedidoCancelamento**](../Models/NfcomPedidoCancelamento.md)|  | [opcional] |

### Tipo do retorno

[**DfeCancelamento**](../Models/DfeCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCancelamentoNfcom"></a>
# **consultarCancelamentoNfcom**
> DfeCancelamento consultarCancelamentoNfcom(id)

Consultar o cancelamento da NFCom

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFCom gerada pela API. | |

### Tipo do retorno

[**DfeCancelamento**](../Models/DfeCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarNfcom"></a>
# **consultarNfcom**
> Dfe consultarNfcom(id)

Consultar NFCom

    Consulta os detalhes de uma NFCom já existente. Forneça o ID único obtido de uma requisição de emissão ou de listagem de NFCom e a API irá retornar as informações da NFCom correspondente.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFCom gerada pela API. | |

### Tipo do retorno

[**Dfe**](../Models/Dfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarStatusSefazNfcom"></a>
# **consultarStatusSefazNfcom**
> DfeSefazStatus consultarStatusSefazNfcom(cpfCnpj, autorizador)

Consulta do Status do Serviço na SEFAZ Autorizadora

    Consulta do status do serviço prestado pelo Portal da Secretaria de Fazenda Estadual.    A API mantém a última consulta em cache por 5 minutos, evitando sobrecarregar desnecessariamente os servidores da SEFAZ.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF/CNPJ do emitente.  Utilize o valor sem máscara. | |
| **autorizador** | **string**| Ambiente Autorizador.    Autorizadores disponíveis: &#x60;SVRS&#x60;.    *Caso não seja informado, será utilizado o ambiente autorizador da UF do emitente.* | [opcional] |

### Tipo do retorno

[**DfeSefazStatus**](../Models/DfeSefazStatus.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="emitirNfcom"></a>
# **emitirNfcom**
> Dfe emitirNfcom(body)

Emitir NFCom

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**NfcomPedidoEmissao**](../Models/NfcomPedidoEmissao.md)|  | |

### Tipo do retorno

[**Dfe**](../Models/Dfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarNfcom"></a>
# **listarNfcom**
> DfeListagem listarNfcom(cpfCnpj, ambiente, $top, $skip, $inlinecount, referencia, chave, serie)

Listar NFCom

    Retorna a lista de NFCom de acordo com os critérios de busca utilizados. As NFCom são retornadas ordenadas pela data da criação, com as mais recentes aparecendo primeiro.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| Filtrar pelo CPF ou CNPJ do emitente.    Utilize o valor sem máscara. | |
| **ambiente** | **string**| Identificação do Ambiente.    Valores aceitos: homologacao, producao | |
| **$top** | **number**| Limite no número de objetos a serem retornados pela API, entre 1 e 100. | [opcional] |
| **$skip** | **number**| Quantidade de objetos que serão ignorados antes da lista começar a ser retornada. | [opcional] |
| **$inlinecount** | **boolean**| Inclui no JSON de resposta, na propriedade &#x60;@count&#x60;, o número total de registros que o filtro retornaria, independente dos filtros de paginação. | [opcional] |
| **referencia** | **string**| Seu identificador único para o documento. | [opcional] |
| **chave** | **string**| Chave de acesso do DF-e. | [opcional] |
| **serie** | **string**| Série do DF-e. | [opcional] |

### Tipo do retorno

[**DfeListagem**](../Models/DfeListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

