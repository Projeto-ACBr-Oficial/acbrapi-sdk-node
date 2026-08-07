# MdfeApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**baixarPdfCancelamentoMdfe**](MdfeApi.md#baixarPdfCancelamentoMdfe) | **GET** /mdfe/{id}/cancelamento/pdf | Baixar PDF do cancelamento |
| [**baixarPdfEncerramentoMdfe**](MdfeApi.md#baixarPdfEncerramentoMdfe) | **GET** /mdfe/{id}/encerramento/pdf | Baixar PDF do encerramento |
| [**baixarPdfEventoMdfe**](MdfeApi.md#baixarPdfEventoMdfe) | **GET** /mdfe/eventos/{id}/pdf | Baixar PDF do evento |
| [**baixarPdfMdfe**](MdfeApi.md#baixarPdfMdfe) | **GET** /mdfe/{id}/pdf | Baixar PDF do DAMDFE |
| [**baixarXmlCancelamentoMdfe**](MdfeApi.md#baixarXmlCancelamentoMdfe) | **GET** /mdfe/{id}/cancelamento/xml | Baixar XML do cancelamento |
| [**baixarXmlEncerramentoMdfe**](MdfeApi.md#baixarXmlEncerramentoMdfe) | **GET** /mdfe/{id}/encerramento/xml | Baixar XML do encerramento |
| [**baixarXmlEventoMdfe**](MdfeApi.md#baixarXmlEventoMdfe) | **GET** /mdfe/eventos/{id}/xml | Baixar XML do evento |
| [**baixarXmlMdfe**](MdfeApi.md#baixarXmlMdfe) | **GET** /mdfe/{id}/xml | Baixar XML do MDF-e processado |
| [**baixarXmlMdfeManifesto**](MdfeApi.md#baixarXmlMdfeManifesto) | **GET** /mdfe/{id}/xml/manifesto | Baixar XML do MDF-e |
| [**baixarXmlMdfeProtocolo**](MdfeApi.md#baixarXmlMdfeProtocolo) | **GET** /mdfe/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ |
| [**cancelarMdfe**](MdfeApi.md#cancelarMdfe) | **POST** /mdfe/{id}/cancelamento | Cancelar um MDF-e autorizado |
| [**consultarCancelamentoMdfe**](MdfeApi.md#consultarCancelamentoMdfe) | **GET** /mdfe/{id}/cancelamento | Consultar o cancelamento do MDF-e |
| [**consultarEncerramentoMdfe**](MdfeApi.md#consultarEncerramentoMdfe) | **GET** /mdfe/{id}/encerramento | Consultar encerramento do MDF-e |
| [**consultarEventoMdfe**](MdfeApi.md#consultarEventoMdfe) | **GET** /mdfe/eventos/{id} | Consultar evento do MDF-e |
| [**consultarLoteMdfe**](MdfeApi.md#consultarLoteMdfe) | **GET** /mdfe/lotes/{id} | Consultar lote de MDF-e |
| [**consultarMdfe**](MdfeApi.md#consultarMdfe) | **GET** /mdfe/{id} | Consultar manifesto |
| [**consultarMdfeNaoEncerrados**](MdfeApi.md#consultarMdfeNaoEncerrados) | **GET** /mdfe/nao-encerrados | Consulta MDF-e não encerrados |
| [**consultarStatusSefazMdfe**](MdfeApi.md#consultarStatusSefazMdfe) | **GET** /mdfe/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora |
| [**emitirLoteMdfe**](MdfeApi.md#emitirLoteMdfe) | **POST** /mdfe/lotes | Emitir lote de MDF-e |
| [**emitirMdfe**](MdfeApi.md#emitirMdfe) | **POST** /mdfe | Emitir MDF-e |
| [**encerrarMdfe**](MdfeApi.md#encerrarMdfe) | **POST** /mdfe/{id}/encerramento | Encerrar um MDF-e autorizado |
| [**incluirCondutorMdfe**](MdfeApi.md#incluirCondutorMdfe) | **POST** /mdfe/{id}/inclusao-condutor | Incluir um condutor em um MDF-e autorizado |
| [**incluirDfeMdfe**](MdfeApi.md#incluirDfeMdfe) | **POST** /mdfe/{id}/inclusao-dfe | Incluir um DF-e em um MDF-e autorizado |
| [**listarLotesMdfe**](MdfeApi.md#listarLotesMdfe) | **GET** /mdfe/lotes | Listar lotes de MDF-e |
| [**listarMdfe**](MdfeApi.md#listarMdfe) | **GET** /mdfe | Listar MDF-e |
| [**sincronizarMdfe**](MdfeApi.md#sincronizarMdfe) | **POST** /mdfe/{id}/sincronizar | Sincroniza dados no MDF-e a partir da SEFAZ |


<a name="baixarPdfCancelamentoMdfe"></a>
# **baixarPdfCancelamentoMdfe**
> Blob baixarPdfCancelamentoMdfe(id)

Baixar PDF do cancelamento

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do MDF-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPdfEncerramentoMdfe"></a>
# **baixarPdfEncerramentoMdfe**
> Blob baixarPdfEncerramentoMdfe(id)

Baixar PDF do encerramento

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do MDF-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPdfEventoMdfe"></a>
# **baixarPdfEventoMdfe**
> Blob baixarPdfEventoMdfe(id)

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

<a name="baixarPdfMdfe"></a>
# **baixarPdfMdfe**
> Blob baixarPdfMdfe(id, logotipo)

Baixar PDF do DAMDFE

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do MDF-e gerado pela API. | |
| **logotipo** | **boolean**| Imprime o documento com logotipo, desde que esteja cadastrado na empresa. | [opcional] |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCancelamentoMdfe"></a>
# **baixarXmlCancelamentoMdfe**
> Blob baixarXmlCancelamentoMdfe(id)

Baixar XML do cancelamento

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do MDF-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlEncerramentoMdfe"></a>
# **baixarXmlEncerramentoMdfe**
> Blob baixarXmlEncerramentoMdfe(id)

Baixar XML do encerramento

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do MDF-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlEventoMdfe"></a>
# **baixarXmlEventoMdfe**
> Blob baixarXmlEventoMdfe(id)

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

<a name="baixarXmlMdfe"></a>
# **baixarXmlMdfe**
> Blob baixarXmlMdfe(id)

Baixar XML do MDF-e processado

    Utilize esse endpoint para obter o XML do manifesto enviado para a SEFAZ, complementado com a informação do protocolo de autorização ou denegação de uso (TAG raiz &#x60;mdfeProc&#x60;).    O XML só estará disponível nesse endpoint caso o manifesto tenha sido autorizado ou denegado pela SEFAZ. Para obter o XML nos demais casos, utilize o endpoint &#x60;GET /mdfe/{id}/xml/manifesto&#x60;.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do MDF-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlMdfeManifesto"></a>
# **baixarXmlMdfeManifesto**
> Blob baixarXmlMdfeManifesto(id)

Baixar XML do MDF-e

    Utilize esse endpoint para obter o XML do manifesto enviado para a SEFAZ.    O XML estará disponível nesse endpoint mesmo em casos que o manifesto tenha sido rejeitado.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da MDF-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlMdfeProtocolo"></a>
# **baixarXmlMdfeProtocolo**
> Blob baixarXmlMdfeProtocolo(id)

Baixar XML do Protocolo da SEFAZ

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da MDF-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="cancelarMdfe"></a>
# **cancelarMdfe**
> DfeCancelamento cancelarMdfe(id, body)

Cancelar um MDF-e autorizado

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do MDF-e gerado pela API. | |
| **body** | [**MdfePedidoCancelamento**](../Models/MdfePedidoCancelamento.md)| Dados do cancelamento. | [opcional] |

### Tipo do retorno

[**DfeCancelamento**](../Models/DfeCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCancelamentoMdfe"></a>
# **consultarCancelamentoMdfe**
> DfeCancelamento consultarCancelamentoMdfe(id)

Consultar o cancelamento do MDF-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do MDF-e gerado pela API. | |

### Tipo do retorno

[**DfeCancelamento**](../Models/DfeCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarEncerramentoMdfe"></a>
# **consultarEncerramentoMdfe**
> MdfeEncerramento consultarEncerramentoMdfe(id)

Consultar encerramento do MDF-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do MDF-e gerado pela API. | |

### Tipo do retorno

[**MdfeEncerramento**](../Models/MdfeEncerramento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarEventoMdfe"></a>
# **consultarEventoMdfe**
> DfeEvento consultarEventoMdfe(id)

Consultar evento do MDF-e

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

<a name="consultarLoteMdfe"></a>
# **consultarLoteMdfe**
> DfeLote consultarLoteMdfe(id)

Consultar lote de MDF-e

    Consulta os detalhes de um lote já existente. Forneça o ID único obtido de uma requisição de emissão ou de listagem de lotes e a API irá retornar as informações do lote correspondente.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do lote gerado pela API. | |

### Tipo do retorno

[**DfeLote**](../Models/DfeLote.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarMdfe"></a>
# **consultarMdfe**
> Dfe consultarMdfe(id)

Consultar manifesto

    Consulta os detalhes de um manifesto já existente. Forneça o ID único obtido de uma requisição de emissão ou de listagem de manifestos e a API irá retornar as informações do manifesto correspondente.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do MDF-e gerado pela API. | |

### Tipo do retorno

[**Dfe**](../Models/Dfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarMdfeNaoEncerrados"></a>
# **consultarMdfeNaoEncerrados**
> MdfeNaoEncerrados consultarMdfeNaoEncerrados(cpfCnpj)

Consulta MDF-e não encerrados

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| CPF/CNPJ do emitente.  Utilize o valor sem máscara. | |

### Tipo do retorno

[**MdfeNaoEncerrados**](../Models/MdfeNaoEncerrados.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarStatusSefazMdfe"></a>
# **consultarStatusSefazMdfe**
> DfeSefazStatus consultarStatusSefazMdfe(cpfCnpj, autorizador)

Consulta do Status do Serviço na SEFAZ Autorizadora

    Consulta do status do serviço prestado pelo Portal da Secretaria de Fazenda Estadual.    A API mantém a última consulta em cache por 5 minutos, evitando sobrecarregar desnecessariamente os servidores da SEFAZ (conforme orientação do MOC - versão 3.0.0a, item 4.6.3). Dessa forma, você poderá chamar esse endpoint quantas vezes quiser, sem preocupar-se em ter o seu CNPJ bloqueado por consumo indevido (Rejeição 656).

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

<a name="emitirLoteMdfe"></a>
# **emitirLoteMdfe**
> DfeLote emitirLoteMdfe(body)

Emitir lote de MDF-e

    **Informações adicionais**:  - Consumo: 1 unidade por MDF-e.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**MdfePedidoEmissaoLote**](../Models/MdfePedidoEmissaoLote.md)|  | |

### Tipo do retorno

[**DfeLote**](../Models/DfeLote.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="emitirMdfe"></a>
# **emitirMdfe**
> Dfe emitirMdfe(body)

Emitir MDF-e

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**MdfePedidoEmissao**](../Models/MdfePedidoEmissao.md)|  | |

### Tipo do retorno

[**Dfe**](../Models/Dfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="encerrarMdfe"></a>
# **encerrarMdfe**
> MdfeEncerramento encerrarMdfe(id, body)

Encerrar um MDF-e autorizado

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do MDF-e gerado pela API. | |
| **body** | [**MdfePedidoEncerramento**](../Models/MdfePedidoEncerramento.md)|  | |

### Tipo do retorno

[**MdfeEncerramento**](../Models/MdfeEncerramento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="incluirCondutorMdfe"></a>
# **incluirCondutorMdfe**
> MdfeInclusaoCondutor incluirCondutorMdfe(id, body)

Incluir um condutor em um MDF-e autorizado

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do MDF-e gerado pela API. | |
| **body** | [**MdfePedidoInclusaoCondutor**](../Models/MdfePedidoInclusaoCondutor.md)|  | |

### Tipo do retorno

[**MdfeInclusaoCondutor**](../Models/MdfeInclusaoCondutor.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="incluirDfeMdfe"></a>
# **incluirDfeMdfe**
> MdfeInclusaoDfe incluirDfeMdfe(id, body)

Incluir um DF-e em um MDF-e autorizado

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do MDF-e gerado pela API. | |
| **body** | [**MdfePedidoInclusaoDfe**](../Models/MdfePedidoInclusaoDfe.md)|  | |

### Tipo do retorno

[**MdfeInclusaoDfe**](../Models/MdfeInclusaoDfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarLotesMdfe"></a>
# **listarLotesMdfe**
> DfeLoteListagem listarLotesMdfe(cpfCnpj, ambiente, $top, $skip, $inlinecount, referencia)

Listar lotes de MDF-e

    Retorna a lista dos lotes de acordo com os critérios de busca utilizados. Os lotes são retornados ordenados pela data da criação, com os mais recentes aparecendo primeiro.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| Filtrar pelo CPF ou CNPJ do emitente.  Utilize o valor sem máscara. | |
| **ambiente** | **string**| Identificação do Ambiente.    Valores aceitos: homologacao, producao | |
| **$top** | **number**| Limite no número de objetos a serem retornados pela API, entre 1 e 100. | [opcional] |
| **$skip** | **number**| Quantidade de objetos que serão ignorados antes da lista começar a ser retornada. | [opcional] |
| **$inlinecount** | **boolean**| Inclui no JSON de resposta, na propriedade &#x60;@count&#x60;, o número total de registros que o filtro retornaria, independente dos filtros de paginação. | [opcional] |
| **referencia** | **string**|  | [opcional] |

### Tipo do retorno

[**DfeLoteListagem**](../Models/DfeLoteListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarMdfe"></a>
# **listarMdfe**
> DfeListagem listarMdfe(cpfCnpj, ambiente, $top, $skip, $inlinecount, referencia, chave, serie)

Listar MDF-e

    Retorna a lista de manifestos de acordo com os critérios de busca utilizados. Os manifestos são retornados ordenados pela data da criação, com os mais recentes aparecendo primeiro.

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

<a name="sincronizarMdfe"></a>
# **sincronizarMdfe**
> DfeSincronizacao sincronizarMdfe(id)

Sincroniza dados no MDF-e a partir da SEFAZ

    Realiza a sincronização dos dados a partir da consulta da situação atual da MDF-e na Base de Dados do Portal da Secretaria de Fazenda Estadual.    **Cenários de uso**:  * Sincronizar um manifesto que se encontra com o status &#x60;erro&#x60; na API, mas está autorizado na SEFAZ (útil em casos de erros de transmissão com a SEFAZ, como instabilidades e timeouts).  * Sincronizar um manifesto que se encontra com o status &#x60;autorizado&#x60;na API, mas está cancelado ou encerrado na SEFAZ.  * Sincronizar todos os eventos de Cancelamento, Encerramento, Inclusão de condutor e Inclusão de DF-e de um manifesto que porventura não tenham sido feitos a partir da API.    **Informações adicionais**:  - Consumo: 1 unidade por evento sincronizado ou requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do MDF-e gerado pela API. | |

### Tipo do retorno

[**DfeSincronizacao**](../Models/DfeSincronizacao.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

