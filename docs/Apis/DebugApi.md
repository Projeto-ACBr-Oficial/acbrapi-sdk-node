# DebugApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**debugDfe**](DebugApi.md#debugDfe) | **GET** /debug/{id} | Debug de DF-e |
| [**debugDfeOriginalPayload**](DebugApi.md#debugDfeOriginalPayload) | **GET** /debug/{id}/original-payload | Payload original recebido |
| [**debugHttpRequestContent**](DebugApi.md#debugHttpRequestContent) | **GET** /debug/http-requests/{id}/request-content | Corpo da requisição HTTP |
| [**debugHttpResponseContent**](DebugApi.md#debugHttpResponseContent) | **GET** /debug/http-requests/{id}/response-content | Corpo da resposta HTTP |


<a name="debugDfe"></a>
# **debugDfe**
> DfeDebug debugDfe(id)

Debug de DF-e

    Este endpoint retorna informações detalhadas de debug sobre o processamento de um documento fiscal eletrônico (DFe),  como NF-e, NFC-e, MDF-e, CT-e, NFS-e, dentre outros. Ele permite inspecionar o conteúdo original enviado à API e analisar  todas as interações realizadas com os serviços autorizadores (SEFAZ ou prefeituras) durante o fluxo de emissão.    **Informações retornadas**:  - JSON original recebido no momento da criação do documento.  - Histórico das etapas de envio e consulta.  - Status e mensagens retornadas pelo autorizador.    **Cenários de uso**:  - Diagnóstico de falhas no processamento do documento.  - Verificação da resposta da SEFAZ ou prefeitura.  - Apoio ao suporte técnico e análise de integração.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do documento fiscal gerado pela API. | |

### Tipo do retorno

[**DfeDebug**](../Models/DfeDebug.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="debugDfeOriginalPayload"></a>
# **debugDfeOriginalPayload**
> Blob debugDfeOriginalPayload(id)

Payload original recebido

    Este endpoint retorna o conteúdo original recebido pela API no momento da criação do documento fiscal.    **Cenários de uso**:  - Inspeção detalhada dos dados enviados à API.  - Verificação de divergências entre o payload fornecido e o processado.  - Encaminhamento do conteúdo original ao suporte da API.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID do documento fiscal gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="debugHttpRequestContent"></a>
# **debugHttpRequestContent**
> Blob debugHttpRequestContent(id)

Corpo da requisição HTTP

    Este endpoint retorna apenas o corpo da requisição HTTP enviada ao autorizador,  preservando o conteúdo exatamente como foi armazenado pela API.    **Informações retornadas**:  - Envelope SOAP da requisição, possivelmente compactado.    **Cenários de uso**:  - Verificação do XML ou SOAP efetivamente enviado.  - Encaminhamento ao suporte da SEFAZ ou prefeitura para análise.  - Diagnóstico técnico do conteúdo de envio.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID da requisição HTTP. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="debugHttpResponseContent"></a>
# **debugHttpResponseContent**
> Blob debugHttpResponseContent(id)

Corpo da resposta HTTP

    Este endpoint retorna apenas o corpo da resposta HTTP recebida do autorizador,  permitindo análise técnica da mensagem retornada pela SEFAZ ou prefeitura.    **Informações retornadas**:  - Envelope SOAP da resposta, ou mensagem de erro (ex: HTML, XML), no formato original.    **Cenários de uso**:  - Inspeção da resposta real retornada pelo autorizador.  - Encaminhamento do conteúdo ao suporte técnico.  - Diagnóstico de rejeições, falhas de processamento ou erros de infraestrutura.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID da requisição HTTP. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

