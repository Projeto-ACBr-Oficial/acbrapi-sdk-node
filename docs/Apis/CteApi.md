# CteApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**baixarPdfCancelamentoCte**](CteApi.md#baixarPdfCancelamentoCte) | **GET** /cte/{id}/cancelamento/pdf | Baixar PDF do cancelamento |
| [**baixarPdfCartaCorrecaoCte**](CteApi.md#baixarPdfCartaCorrecaoCte) | **GET** /cte/{id}/carta-correcao/pdf | Baixar PDF da carta de correção |
| [**baixarPdfCte**](CteApi.md#baixarPdfCte) | **GET** /cte/{id}/pdf | Baixar PDF do DACTE |
| [**baixarPdfEventoCte**](CteApi.md#baixarPdfEventoCte) | **GET** /cte/eventos/{id}/pdf | Baixar PDF do evento |
| [**baixarXmlCancelamentoCte**](CteApi.md#baixarXmlCancelamentoCte) | **GET** /cte/{id}/cancelamento/xml | Baixar XML do cancelamento |
| [**baixarXmlCartaCorrecaoCte**](CteApi.md#baixarXmlCartaCorrecaoCte) | **GET** /cte/{id}/carta-correcao/xml | Baixar XML da carta de correção |
| [**baixarXmlCte**](CteApi.md#baixarXmlCte) | **GET** /cte/{id}/xml | Baixar XML do CT-e processado |
| [**baixarXmlCteConhecimento**](CteApi.md#baixarXmlCteConhecimento) | **GET** /cte/{id}/xml/conhecimento | Baixar XML do CT-e |
| [**baixarXmlCteProtocolo**](CteApi.md#baixarXmlCteProtocolo) | **GET** /cte/{id}/xml/protocolo | Baixar XML do Protocolo da SEFAZ |
| [**baixarXmlEventoCte**](CteApi.md#baixarXmlEventoCte) | **GET** /cte/eventos/{id}/xml | Baixar XML do evento |
| [**cancelarCte**](CteApi.md#cancelarCte) | **POST** /cte/{id}/cancelamento | Cancelar um CT-e autorizado |
| [**consultarCancelamentoCte**](CteApi.md#consultarCancelamentoCte) | **GET** /cte/{id}/cancelamento | Consultar o cancelamento do CT-e |
| [**consultarCartaCorrecaoCte**](CteApi.md#consultarCartaCorrecaoCte) | **GET** /cte/{id}/carta-correcao | Consultar a solicitação de correção do CT-e |
| [**consultarCte**](CteApi.md#consultarCte) | **GET** /cte/{id} | Consultar CT-e |
| [**consultarEventoCte**](CteApi.md#consultarEventoCte) | **GET** /cte/eventos/{id} | Consultar evento |
| [**consultarStatusSefazCte**](CteApi.md#consultarStatusSefazCte) | **GET** /cte/sefaz/status | Consulta do Status do Serviço na SEFAZ Autorizadora |
| [**criarCartaCorrecaoCte**](CteApi.md#criarCartaCorrecaoCte) | **POST** /cte/{id}/carta-correcao | Solicitar correção do CT-e |
| [**emitirCte**](CteApi.md#emitirCte) | **POST** /cte | Emitir CT-e |
| [**emitirCteSimp**](CteApi.md#emitirCteSimp) | **POST** /cte/simp | Emitir CT-e Simplificado |
| [**listarCte**](CteApi.md#listarCte) | **GET** /cte | Listar CT-e |
| [**sincronizarCte**](CteApi.md#sincronizarCte) | **POST** /cte/{id}/sincronizar | Sincroniza dados no CT-e a partir da SEFAZ |


<a name="baixarPdfCancelamentoCte"></a>
# **baixarPdfCancelamentoCte**
> Blob baixarPdfCancelamentoCte(id)

Baixar PDF do cancelamento

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPdfCartaCorrecaoCte"></a>
# **baixarPdfCartaCorrecaoCte**
> Blob baixarPdfCartaCorrecaoCte(id)

Baixar PDF da carta de correção

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPdfCte"></a>
# **baixarPdfCte**
> Blob baixarPdfCte(id, logotipo)

Baixar PDF do DACTE

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e gerado pela API. | |
| **logotipo** | **boolean**| Imprime o documento com logotipo, desde que esteja cadastrado na empresa. | [opcional] |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarPdfEventoCte"></a>
# **baixarPdfEventoCte**
> Blob baixarPdfEventoCte(id)

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

<a name="baixarXmlCancelamentoCte"></a>
# **baixarXmlCancelamentoCte**
> Blob baixarXmlCancelamentoCte(id)

Baixar XML do cancelamento

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCartaCorrecaoCte"></a>
# **baixarXmlCartaCorrecaoCte**
> Blob baixarXmlCartaCorrecaoCte(id)

Baixar XML da carta de correção

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCte"></a>
# **baixarXmlCte**
> Blob baixarXmlCte(id)

Baixar XML do CT-e processado

    Utilize esse endpoint para obter o XML do conhecimento enviado para a SEFAZ, complementado com a informação do protocolo de autorização de uso (TAG raiz &#x60;cteProc&#x60;).    O XML só estará disponível nesse endpoint caso o conhecimento tenha sido autorizado pela SEFAZ. Para obter o XML nos demais casos, utilize o endpoint &#x60;GET /cte/{id}/xml/conhecimento&#x60;.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCteConhecimento"></a>
# **baixarXmlCteConhecimento**
> Blob baixarXmlCteConhecimento(id)

Baixar XML do CT-e

    Utilize esse endpoint para obter o XML do conhecimento enviado para a SEFAZ.    O XML estará disponível nesse endpoint mesmo em casos que o conhecimento tenha sido rejeitado.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da CT-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCteProtocolo"></a>
# **baixarXmlCteProtocolo**
> Blob baixarXmlCteProtocolo(id)

Baixar XML do Protocolo da SEFAZ

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da CT-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlEventoCte"></a>
# **baixarXmlEventoCte**
> Blob baixarXmlEventoCte(id)

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

<a name="cancelarCte"></a>
# **cancelarCte**
> DfeCancelamento cancelarCte(id, body)

Cancelar um CT-e autorizado

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e gerado pela API. | |
| **body** | [**CtePedidoCancelamento**](../Models/CtePedidoCancelamento.md)|  | [opcional] |

### Tipo do retorno

[**DfeCancelamento**](../Models/DfeCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCancelamentoCte"></a>
# **consultarCancelamentoCte**
> DfeCancelamento consultarCancelamentoCte(id)

Consultar o cancelamento do CT-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e gerado pela API. | |

### Tipo do retorno

[**DfeCancelamento**](../Models/DfeCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCartaCorrecaoCte"></a>
# **consultarCartaCorrecaoCte**
> CteCartaCorrecao consultarCartaCorrecaoCte(id)

Consultar a solicitação de correção do CT-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e gerado pela API. | |

### Tipo do retorno

[**CteCartaCorrecao**](../Models/CteCartaCorrecao.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCte"></a>
# **consultarCte**
> Dfe consultarCte(id)

Consultar CT-e

    Consulta os detalhes de um CT-e já existente. Forneça o ID único obtido de uma requisição de emissão ou de listagem de CT-e e a API irá retornar as informações do CT-e correspondente.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e gerado pela API. | |

### Tipo do retorno

[**Dfe**](../Models/Dfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarEventoCte"></a>
# **consultarEventoCte**
> DfeEvento consultarEventoCte(id)

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

<a name="consultarStatusSefazCte"></a>
# **consultarStatusSefazCte**
> DfeSefazStatus consultarStatusSefazCte(cpfCnpj, autorizador)

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

<a name="criarCartaCorrecaoCte"></a>
# **criarCartaCorrecaoCte**
> CteCartaCorrecao criarCartaCorrecaoCte(id, body)

Solicitar correção do CT-e

    É possível enviar até 20 correções diferentes, sendo que será válido sempre a última correção enviada.    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e gerado pela API. | |
| **body** | [**CtePedidoCartaCorrecao**](../Models/CtePedidoCartaCorrecao.md)|  | |

### Tipo do retorno

[**CteCartaCorrecao**](../Models/CteCartaCorrecao.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="emitirCte"></a>
# **emitirCte**
> Dfe emitirCte(body)

Emitir CT-e

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**CtePedidoEmissao**](../Models/CtePedidoEmissao.md)|  | |

### Tipo do retorno

[**Dfe**](../Models/Dfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="emitirCteSimp"></a>
# **emitirCteSimp**
> Dfe emitirCteSimp(body)

Emitir CT-e Simplificado

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**CteSimpPedidoEmissao**](../Models/CteSimpPedidoEmissao.md)|  | |

### Tipo do retorno

[**Dfe**](../Models/Dfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarCte"></a>
# **listarCte**
> DfeListagem listarCte(cpfCnpj, ambiente, $top, $skip, $inlinecount, referencia, chave, serie)

Listar CT-e

    Retorna a lista de CT-e de acordo com os critérios de busca utilizados. Os CT-e são retornados ordenados pela data da criação, com os mais recentes aparecendo primeiro.

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

<a name="sincronizarCte"></a>
# **sincronizarCte**
> DfeSincronizacao sincronizarCte(id)

Sincroniza dados no CT-e a partir da SEFAZ

    Realiza a sincronização dos dados a partir da consulta da situação atual da CT-e na Base de Dados do Portal da Secretaria de Fazenda Estadual.    **Cenários de uso**:  * Sincronizar um CT-e que se encontra com o status &#x60;erro&#x60; na API, mas está autorizado na SEFAZ (útil em casos de erros de transmissão com a SEFAZ, como instabilidades e timeouts).  * Sincronizar um CT-e que se encontra com o status &#x60;autorizado&#x60;na API, mas está cancelado na SEFAZ.  * Sincronizar todos os eventos de Cancelamento e Carta de Correção de um CT-e que porventura não tenham sido feitos a partir da API.    **Informações adicionais**:  - Consumo: 1 unidade por evento sincronizado ou requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do CT-e gerado pela API. | |

### Tipo do retorno

[**DfeSincronizacao**](../Models/DfeSincronizacao.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

