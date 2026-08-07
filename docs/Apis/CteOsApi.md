# CteOsApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**baixarPdfCancelamentoCteOs**](CteOsApi.md#baixarPdfCancelamentoCteOs) | **GET** /cteos/{id}/cancelamento/pdf | Baixar PDF do cancelamento |
| [**baixarPdfCartaCorrecaoCteOs**](CteOsApi.md#baixarPdfCartaCorrecaoCteOs) | **GET** /cteos/{id}/carta-correcao/pdf | Baixar PDF da carta de correção |
| [**baixarPdfCteOs**](CteOsApi.md#baixarPdfCteOs) | **GET** /cteos/{id}/pdf | Baixar PDF do DACTE |
| [**baixarPdfEventoCteOs**](CteOsApi.md#baixarPdfEventoCteOs) | **GET** /cteos/eventos/{id}/pdf | Baixar PDF do evento |
| [**baixarXmlCancelamentoCteOs**](CteOsApi.md#baixarXmlCancelamentoCteOs) | **GET** /cteos/{id}/cancelamento/xml | Baixar XML do cancelamento |
| [**baixarXmlCartaCorrecaoCteOs**](CteOsApi.md#baixarXmlCartaCorrecaoCteOs) | **GET** /cteos/{id}/carta-correcao/xml | Baixar XML da carta de correção |
| [**baixarXmlCteOs**](CteOsApi.md#baixarXmlCteOs) | **GET** /cteos/{id}/xml | Baixar XML do CT-e OS processado |
| [**baixarXmlCteOsConhecimento**](CteOsApi.md#baixarXmlCteOsConhecimento) | **GET** /cteos/{id}/xml/conhecimento | Baixar XML do CT-e OS |
| [**baixarXmlCteOsProtocolo**](CteOsApi.md#baixarXmlCteOsProtocolo) | **GET** /cteos/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ |
| [**baixarXmlEventoCteOs**](CteOsApi.md#baixarXmlEventoCteOs) | **GET** /cteos/eventos/{id}/xml | Baixar XML do evento |
| [**cancelarCteOs**](CteOsApi.md#cancelarCteOs) | **POST** /cteos/{id}/cancelamento | Cancelar um CT-e OS autorizado |
| [**consultarCancelamentoCteOs**](CteOsApi.md#consultarCancelamentoCteOs) | **GET** /cteos/{id}/cancelamento | Consultar o cancelamento do CT-e OS |
| [**consultarCartaCorrecaoCteOs**](CteOsApi.md#consultarCartaCorrecaoCteOs) | **GET** /cteos/{id}/carta-correcao | Consultar a solicitação de correção do CT-e OS |
| [**consultarCteOs**](CteOsApi.md#consultarCteOs) | **GET** /cteos/{id} | Consultar CT-e OS |
| [**consultarEventoCteOs**](CteOsApi.md#consultarEventoCteOs) | **GET** /cteos/eventos/{id} | Consultar evento |
| [**consultarStatusSefazCteOs**](CteOsApi.md#consultarStatusSefazCteOs) | **GET** /cteos/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora |
| [**criarCartaCorrecaoCteOs**](CteOsApi.md#criarCartaCorrecaoCteOs) | **POST** /cteos/{id}/carta-correcao | Solicitar correção do CT-e OS |
| [**emitirCteOs**](CteOsApi.md#emitirCteOs) | **POST** /cteos | Emitir CT-e OS |
| [**listarCteOs**](CteOsApi.md#listarCteOs) | **GET** /cteos | Listar CT-e OS |
| [**sincronizarCteOs**](CteOsApi.md#sincronizarCteOs) | **POST** /cteos/{id}/sincronizar | Sincroniza dados no CT-e OS a partir da SEFAZ |


<a name="baixarPdfCancelamentoCteOs"></a>
# **baixarPdfCancelamentoCteOs**
> Blob baixarPdfCancelamentoCteOs(id)

Baixar PDF do cancelamento

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e OS gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPdfCartaCorrecaoCteOs"></a>
# **baixarPdfCartaCorrecaoCteOs**
> Blob baixarPdfCartaCorrecaoCteOs(id)

Baixar PDF da carta de correção

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e OS gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPdfCteOs"></a>
# **baixarPdfCteOs**
> Blob baixarPdfCteOs(id, logotipo)

Baixar PDF do DACTE

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e OS gerado pela API. | |
| **logotipo** | **boolean**| Imprime o documento com logotipo, desde que esteja cadastrado na empresa. | [opcional] |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPdfEventoCteOs"></a>
# **baixarPdfEventoCteOs**
> Blob baixarPdfEventoCteOs(id)

Baixar PDF do evento

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do evento gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCancelamentoCteOs"></a>
# **baixarXmlCancelamentoCteOs**
> Blob baixarXmlCancelamentoCteOs(id)

Baixar XML do cancelamento

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e OS gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCartaCorrecaoCteOs"></a>
# **baixarXmlCartaCorrecaoCteOs**
> Blob baixarXmlCartaCorrecaoCteOs(id)

Baixar XML da carta de correção

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e OS gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCteOs"></a>
# **baixarXmlCteOs**
> Blob baixarXmlCteOs(id)

Baixar XML do CT-e OS processado

    Utilize esse endpoint para obter o XML do conhecimento enviado para a SEFAZ, complementado com a informação do protocolo de autorização de uso (TAG raiz &#x60;cteProc&#x60;).    O XML só estará disponível nesse endpoint caso o conhecimento tenha sido autorizado pela SEFAZ. Para obter o XML nos demais casos, utilize o endpoint &#x60;GET /cteos/{id}/xml/conhecimento&#x60;.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e OS gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCteOsConhecimento"></a>
# **baixarXmlCteOsConhecimento**
> Blob baixarXmlCteOsConhecimento(id)

Baixar XML do CT-e OS

    Utilize esse endpoint para obter o XML do conhecimento enviado para a SEFAZ.    O XML estará disponível nesse endpoint mesmo em casos que o conhecimento tenha sido rejeitado.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da CT-e OS gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCteOsProtocolo"></a>
# **baixarXmlCteOsProtocolo**
> Blob baixarXmlCteOsProtocolo(id)

Baixar XML do Protocolo da SEFAZ

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da CT-e OS gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlEventoCteOs"></a>
# **baixarXmlEventoCteOs**
> Blob baixarXmlEventoCteOs(id)

Baixar XML do evento

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do evento gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="cancelarCteOs"></a>
# **cancelarCteOs**
> DfeCancelamento cancelarCteOs(id, body)

Cancelar um CT-e OS autorizado

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e OS gerado pela API. | |
| **body** | [**CteOsPedidoCancelamento**](../Models/CteOsPedidoCancelamento.md)|  | [opcional] |

### Tipo do retorno

[**DfeCancelamento**](../Models/DfeCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCancelamentoCteOs"></a>
# **consultarCancelamentoCteOs**
> DfeCancelamento consultarCancelamentoCteOs(id)

Consultar o cancelamento do CT-e OS

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e OS gerado pela API. | |

### Tipo do retorno

[**DfeCancelamento**](../Models/DfeCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCartaCorrecaoCteOs"></a>
# **consultarCartaCorrecaoCteOs**
> CteOsCartaCorrecao consultarCartaCorrecaoCteOs(id)

Consultar a solicitação de correção do CT-e OS

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e OS gerado pela API. | |

### Tipo do retorno

[**CteOsCartaCorrecao**](../Models/CteOsCartaCorrecao.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCteOs"></a>
# **consultarCteOs**
> Dfe consultarCteOs(id)

Consultar CT-e OS

    Consulta os detalhes de um CT-e OS já existente. Forneça o ID único obtido de uma requisição de emissão ou de listagem de CT-e OS e a API irá retornar as informações do CT-e OS correspondente.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e OS gerado pela API. | |

### Tipo do retorno

[**Dfe**](../Models/Dfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarEventoCteOs"></a>
# **consultarEventoCteOs**
> DfeEvento consultarEventoCteOs(id)

Consultar evento

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do evento gerado pela API. | |

### Tipo do retorno

[**DfeEvento**](../Models/DfeEvento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarStatusSefazCteOs"></a>
# **consultarStatusSefazCteOs**
> DfeSefazStatus consultarStatusSefazCteOs(cpfCnpj, autorizador)

Consulta do Status do Serviço na SEFAZ Autorizadora

    Consulta do status do serviço prestado pelo Portal da Secretaria de Fazenda Estadual.    A API mantém a última consulta em cache por 5 minutos, evitando sobrecarregar desnecessariamente os servidores da SEFAZ (conforme orientação do MOC - versão 3.0.0a, item 4.6.3). Dessa forma, você poderá chamar esse endpoint quantas vezes quiser, sem preocupar-se em ter o seu CNPJ bloqueado por consumo indevido (Rejeição 656).

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF/CNPJ do emitente.  Utilize o valor sem máscara. | |
| **autorizador** | **string**| Ambiente Autorizador.    Autorizadores disponíveis: &#x60;MT&#x60;, &#x60;MS&#x60;, &#x60;MG&#x60;, &#x60;PR&#x60;, &#x60;RS&#x60;, &#x60;SP&#x60;, &#x60;SVRS&#x60;, &#x60;SVSP&#x60;, &#x60;AN&#x60;.    *Caso não seja informado, será utilizado o ambiente autorizador da UF do emitente.* | [opcional] |

### Tipo do retorno

[**DfeSefazStatus**](../Models/DfeSefazStatus.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="criarCartaCorrecaoCteOs"></a>
# **criarCartaCorrecaoCteOs**
> CteOsCartaCorrecao criarCartaCorrecaoCteOs(id, body)

Solicitar correção do CT-e OS

    É possível enviar até 20 correções diferentes, sendo que será válido sempre a última correção enviada.    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e OS gerado pela API. | |
| **body** | [**CteOsPedidoCartaCorrecao**](../Models/CteOsPedidoCartaCorrecao.md)|  | |

### Tipo do retorno

[**CteOsCartaCorrecao**](../Models/CteOsCartaCorrecao.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="emitirCteOs"></a>
# **emitirCteOs**
> Dfe emitirCteOs(body)

Emitir CT-e OS

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**CteOsPedidoEmissao**](../Models/CteOsPedidoEmissao.md)|  | |

### Tipo do retorno

[**Dfe**](../Models/Dfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarCteOs"></a>
# **listarCteOs**
> DfeListagem listarCteOs(cpfCnpj, ambiente, $top, $skip, $inlinecount, referencia, chave, serie)

Listar CT-e OS

    Retorna a lista de CT-e OS de acordo com os critérios de busca utilizados. Os CT-e OS são retornados ordenados pela data da criação, com os mais recentes aparecendo primeiro.

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

<a name="sincronizarCteOs"></a>
# **sincronizarCteOs**
> DfeSincronizacao sincronizarCteOs(id)

Sincroniza dados no CT-e OS a partir da SEFAZ

    Realiza a sincronização dos dados a partir da consulta da situação atual do CT-e OS na Base de Dados do Portal da Secretaria de Fazenda Estadual.    **Cenários de uso**:  * Sincronizar um CT-e OS que se encontra com o status &#x60;erro&#x60; na API, mas está autorizado na SEFAZ (útil em casos de erros de transmissão com a SEFAZ, como instabilidades e timeouts).  * Sincronizar um CT-e OS que se encontra com o status &#x60;autorizado&#x60;na API, mas está cancelado na SEFAZ.  * Sincronizar todos os eventos de Cancelamento e Carta de Correção de um CT-e OS que porventura não tenham sido feitos a partir da API.    **Informações adicionais**:  - Consumo: 1 unidade por evento sincronizado ou requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e OS gerado pela API. | |

### Tipo do retorno

[**DfeSincronizacao**](../Models/DfeSincronizacao.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

