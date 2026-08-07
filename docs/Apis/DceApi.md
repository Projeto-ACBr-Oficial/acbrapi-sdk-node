# DceApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**baixarPdfDce**](DceApi.md#baixarPdfDce) | **GET** /dce/{id}/pdf | Baixar PDF do DACE |
| [**baixarXmlCancelamentoDce**](DceApi.md#baixarXmlCancelamentoDce) | **GET** /dce/{id}/cancelamento/xml | Baixar XML do cancelamento |
| [**baixarXmlDce**](DceApi.md#baixarXmlDce) | **GET** /dce/{id}/xml | Baixar XML da DC-e processada |
| [**baixarXmlDceDeclaracao**](DceApi.md#baixarXmlDceDeclaracao) | **GET** /dce/{id}/xml/declaracao | Baixar XML da DC-e |
| [**baixarXmlDceProtocolo**](DceApi.md#baixarXmlDceProtocolo) | **GET** /dce/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ |
| [**cancelarDce**](DceApi.md#cancelarDce) | **POST** /dce/{id}/cancelamento | Cancelar uma DC-e autorizada |
| [**consultarCancelamentoDce**](DceApi.md#consultarCancelamentoDce) | **GET** /dce/{id}/cancelamento | Consultar o cancelamento da DC-e |
| [**consultarDce**](DceApi.md#consultarDce) | **GET** /dce/{id} | Consultar DC-e |
| [**consultarStatusSefazDce**](DceApi.md#consultarStatusSefazDce) | **GET** /dce/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora |
| [**emitirDce**](DceApi.md#emitirDce) | **POST** /dce | Emitir DC-e |
| [**listarDce**](DceApi.md#listarDce) | **GET** /dce | Listar DC-e |


<a name="baixarPdfDce"></a>
# **baixarPdfDce**
> Blob baixarPdfDce(id)

Baixar PDF do DACE

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da DC-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCancelamentoDce"></a>
# **baixarXmlCancelamentoDce**
> Blob baixarXmlCancelamentoDce(id)

Baixar XML do cancelamento

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da DC-e gerada pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlDce"></a>
# **baixarXmlDce**
> Blob baixarXmlDce(id)

Baixar XML da DC-e processada

    Utilize esse endpoint para obter o XML da DC-e enviada para a SEFAZ, complementado com a informação do protocolo de autorização de uso (TAG raiz &#x60;dceProc&#x60;).    O XML só estará disponível nesse endpoint caso a DC-e tenha sido autorizada pela SEFAZ. Para obter o XML nos demais casos, utilize o endpoint &#x60;GET /dce/{id}/xml/declaracao&#x60;.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da DC-e gerada pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlDceDeclaracao"></a>
# **baixarXmlDceDeclaracao**
> Blob baixarXmlDceDeclaracao(id)

Baixar XML da DC-e

    Utilize esse endpoint para obter o XML da DC-e enviada para a SEFAZ.    O XML estará disponível nesse endpoint mesmo em casos que a declaração tenha sido rejeitada.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da DC-e gerada pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlDceProtocolo"></a>
# **baixarXmlDceProtocolo**
> Blob baixarXmlDceProtocolo(id)

Baixar XML do Protocolo da SEFAZ

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da DC-e gerada pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="cancelarDce"></a>
# **cancelarDce**
> DfeCancelamento cancelarDce(id, body)

Cancelar uma DC-e autorizada

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da DC-e gerada pela API. | |
| **body** | [**DcePedidoCancelamento**](../Models/DcePedidoCancelamento.md)|  | [opcional] |

### Tipo do retorno

[**DfeCancelamento**](../Models/DfeCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCancelamentoDce"></a>
# **consultarCancelamentoDce**
> DfeCancelamento consultarCancelamentoDce(id)

Consultar o cancelamento da DC-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da DC-e gerada pela API. | |

### Tipo do retorno

[**DfeCancelamento**](../Models/DfeCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarDce"></a>
# **consultarDce**
> Dfe consultarDce(id)

Consultar DC-e

    Consulta os detalhes de uma DC-e já existente. Forneça o ID único obtido de uma requisição de emissão ou de listagem de DC-e e a API irá retornar as informações da DC-e correspondente.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da DC-e gerada pela API. | |

### Tipo do retorno

[**Dfe**](../Models/Dfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarStatusSefazDce"></a>
# **consultarStatusSefazDce**
> DfeSefazStatus consultarStatusSefazDce(cpfCnpj, autorizador)

Consulta do Status do Serviço na SEFAZ Autorizadora

    Consulta do status do serviço prestado pelo Portal da Secretaria de Fazenda Estadual.    A API mantém a última consulta em cache por 5 minutos, evitando sobrecarregar desnecessariamente os servidores da SEFAZ.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF/CNPJ do emitente.  Utilize o valor sem máscara. | |
| **autorizador** | **string**| Ambiente Autorizador.    Autorizadores disponíveis: &#x60;AN&#x60;.    *Caso não seja informado, será utilizado o ambiente autorizador da UF do emitente.* | [opcional] |

### Tipo do retorno

[**DfeSefazStatus**](../Models/DfeSefazStatus.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="emitirDce"></a>
# **emitirDce**
> Dfe emitirDce(body)

Emitir DC-e

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DcePedidoEmissao**](../Models/DcePedidoEmissao.md)|  | |

### Tipo do retorno

[**Dfe**](../Models/Dfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarDce"></a>
# **listarDce**
> DfeListagem listarDce(cpfCnpj, ambiente, $top, $skip, $inlinecount, referencia, chave, serie)

Listar DC-e

    Retorna a lista de DC-e de acordo com os critérios de busca utilizados. As DC-e são retornadas ordenadas pela data da criação, com as mais recentes aparecendo primeiro.

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

