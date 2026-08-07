# NfseApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**baixarPdfNfse**](NfseApi.md#baixarPdfNfse) | **GET** /nfse/{id}/pdf | Baixar PDF do DANFSE |
| [**baixarXmlCancelamentoNfse**](NfseApi.md#baixarXmlCancelamentoNfse) | **GET** /nfse/{Id}/cancelamento/xml | Baixar XML do evento de cancelamento |
| [**baixarXmlDps**](NfseApi.md#baixarXmlDps) | **GET** /nfse/{id}/xml/dps | Baixar XML da DPS |
| [**baixarXmlNfse**](NfseApi.md#baixarXmlNfse) | **GET** /nfse/{id}/xml | Baixar XML da NFS-e processada |
| [**cancelarNfse**](NfseApi.md#cancelarNfse) | **POST** /nfse/{id}/cancelamento | Cancelar uma NFS-e autorizada |
| [**cidadesAtendidas**](NfseApi.md#cidadesAtendidas) | **GET** /nfse/cidades | Cidades atendidas |
| [**consultarCancelamentoNfse**](NfseApi.md#consultarCancelamentoNfse) | **GET** /nfse/{id}/cancelamento | Consultar o cancelamento da NFS-e |
| [**consultarLoteNfse**](NfseApi.md#consultarLoteNfse) | **GET** /nfse/lotes/{id} | Consultar lote de NFS-e |
| [**consultarMetadados**](NfseApi.md#consultarMetadados) | **GET** /nfse/cidades/{codigo_ibge} | Consultar metadados |
| [**consultarNfse**](NfseApi.md#consultarNfse) | **GET** /nfse/{id} | Consultar NFS-e |
| [**emitirLoteNfse**](NfseApi.md#emitirLoteNfse) | **POST** /nfse/lotes | Emitir lote de NFS-e |
| [**emitirLoteNfseDps**](NfseApi.md#emitirLoteNfseDps) | **POST** /nfse/dps/lotes | Emitir lote de NFS-e |
| [**emitirNfse**](NfseApi.md#emitirNfse) | **POST** /nfse | Emitir NFS-e |
| [**emitirNfseDps**](NfseApi.md#emitirNfseDps) | **POST** /nfse/dps | Emitir NFS-e |
| [**listarLotesNfse**](NfseApi.md#listarLotesNfse) | **GET** /nfse/lotes | Listar lotes de NFS-e |
| [**listarNfse**](NfseApi.md#listarNfse) | **GET** /nfse | Listar NFS-e |
| [**sincronizarNfse**](NfseApi.md#sincronizarNfse) | **POST** /nfse/{id}/sincronizar | Sincroniza dados na NFS-e a partir da Prefeitura |


<a name="baixarPdfNfse"></a>
# **baixarPdfNfse**
> Blob baixarPdfNfse(id, logotipo, mensagemRodape)

Baixar PDF do DANFSE

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFS-e gerado pela API. | |
| **logotipo** | **boolean**| Imprime o documento com logotipo, desde que esteja cadastrado na empresa. | [opcional] |
| **mensagemRodape** | **string**| Imprime mensagem no rodapé do documento.    O caractere &#x60;|&#x60; (pipe) poderá ser utilizado para definir a quantidade e o alinhamento das mensagens.    **Exemplos de Uso:**  * &#x60;\&quot;esquerda\&quot;&#x60;  * &#x60;\&quot;esquerda|centro\&quot;&#x60;  * &#x60;\&quot;esquerda|centro|direita\&quot;&#x60;  * &#x60;\&quot;|centro\&quot;&#x60;, &#x60;\&quot;|centro|\&quot;&#x60;  * &#x60;\&quot;|centro|direita\&quot;&#x60;  * &#x60;\&quot;||direita\&quot;&#x60;  * &#x60;\&quot;esquerda||direita\&quot;&#x60;    Default: &#x60;\&quot;\&quot;&#x60; | [opcional] |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlCancelamentoNfse"></a>
# **baixarXmlCancelamentoNfse**
> Blob baixarXmlCancelamentoNfse(id)

Baixar XML do evento de cancelamento

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFS-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlDps"></a>
# **baixarXmlDps**
> Blob baixarXmlDps(id)

Baixar XML da DPS

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFS-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlNfse"></a>
# **baixarXmlNfse**
> Blob baixarXmlNfse(id)

Baixar XML da NFS-e processada

    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFS-e gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="cancelarNfse"></a>
# **cancelarNfse**
> NfseCancelamento cancelarNfse(id, body)

Cancelar uma NFS-e autorizada

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFS-e gerado pela API. | |
| **body** | [**NfsePedidoCancelamento**](../Models/NfsePedidoCancelamento.md)|  | [opcional] |

### Tipo do retorno

[**NfseCancelamento**](../Models/NfseCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="cidadesAtendidas"></a>
# **cidadesAtendidas**
> NfseCidadesAtendidas cidadesAtendidas()

Cidades atendidas

    Fornece uma relação completa de todos os municípios atendidos pela API.

### Parâmetros
Este endpoint não usa parâmetros.

### Tipo do retorno

[**NfseCidadesAtendidas**](../Models/NfseCidadesAtendidas.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCancelamentoNfse"></a>
# **consultarCancelamentoNfse**
> NfseCancelamento consultarCancelamentoNfse(id)

Consultar o cancelamento da NFS-e

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFS-e gerado pela API. | |

### Tipo do retorno

[**NfseCancelamento**](../Models/NfseCancelamento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarLoteNfse"></a>
# **consultarLoteNfse**
> RpsLote consultarLoteNfse(id)

Consultar lote de NFS-e

    Consulta os detalhes de um lote já existente. Forneça o ID único obtido de uma requisição de emissão ou de listagem de lotes e a API irá retornar as informações do lote correspondente.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do lote gerado pela API. | |

### Tipo do retorno

[**RpsLote**](../Models/RpsLote.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarMetadados"></a>
# **consultarMetadados**
> NfseCidadeMetadados consultarMetadados(codigoIbge)

Consultar metadados

    Consulta a disponibilidade de emissão e alguns metadados de um município.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **codigoIbge** | **string**| Código IBGE do município. | |

### Tipo do retorno

[**NfseCidadeMetadados**](../Models/NfseCidadeMetadados.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarNfse"></a>
# **consultarNfse**
> Nfse consultarNfse(id)

Consultar NFS-e

    Consulta os detalhes de uma NFS-e já existente. Forneça o ID único obtido de uma requisição de criação ou de listagem de notas e a API irá retornar as informações da nota correspondente.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFS-e gerado pela API. | |

### Tipo do retorno

[**Nfse**](../Models/Nfse.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="emitirLoteNfse"></a>
# **emitirLoteNfse**
> RpsLote emitirLoteNfse(body)

Emitir lote de NFS-e

    **Informações adicionais**:  - Consumo: 1 unidade por NFS-e.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**RpsPedidoEmissaoLote**](../Models/RpsPedidoEmissaoLote.md)|  | |

### Tipo do retorno

[**RpsLote**](../Models/RpsLote.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="emitirLoteNfseDps"></a>
# **emitirLoteNfseDps**
> RpsLote emitirLoteNfseDps(body)

Emitir lote de NFS-e

    **Informações adicionais**:  - Consumo: 1 unidade por NFS-e.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**NfseLoteDpsPedidoEmissao**](../Models/NfseLoteDpsPedidoEmissao.md)|  | |

### Tipo do retorno

[**RpsLote**](../Models/RpsLote.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="emitirNfse"></a>
# **emitirNfse**
> Nfse emitirNfse(body)

Emitir NFS-e

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**NfsePedidoEmissao**](../Models/NfsePedidoEmissao.md)|  | |

### Tipo do retorno

[**Nfse**](../Models/Nfse.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="emitirNfseDps"></a>
# **emitirNfseDps**
> Nfse emitirNfseDps(body)

Emitir NFS-e

    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**NfseDpsPedidoEmissao**](../Models/NfseDpsPedidoEmissao.md)|  | |

### Tipo do retorno

[**Nfse**](../Models/Nfse.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarLotesNfse"></a>
# **listarLotesNfse**
> RpsLoteListagem listarLotesNfse(cpfCnpj, ambiente, $top, $skip, $inlinecount, referencia)

Listar lotes de NFS-e

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

[**RpsLoteListagem**](../Models/RpsLoteListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarNfse"></a>
# **listarNfse**
> NfseListagem listarNfse(cpfCnpj, ambiente, $top, $skip, $inlinecount, referencia, chave, serie)

Listar NFS-e

    Retorna a lista de notas de acordo com os critérios de busca utilizados. As notas são retornadas ordenadas pela data da criação, com as mais recentes aparecendo primeiro.

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

[**NfseListagem**](../Models/NfseListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="sincronizarNfse"></a>
# **sincronizarNfse**
> NfseSincronizacao sincronizarNfse(id, body)

Sincroniza dados na NFS-e a partir da Prefeitura

    Realiza a sincronização dos dados a partir da consulta da situação atual da NFS-e na prefeitura.    **Cenários de uso**:  * Sincronizar uma nota que se encontra com o status &#x60;processando&#x60; na API, mas está autorizada na prefeitura;  * Sincronizar uma nota que se encontra com o status &#x60;erro&#x60; na API, mas está autorizada na prefeitura (útil em casos de erros de transmissão, como instabilidades e timeouts);  * Sincronizar uma nota que se encontra com o status &#x60;autorizada&#x60;na API, mas está cancelada na prefeitura.    **Informações adicionais**:  - Consumo: 1 unidade por evento sincronizado ou requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da NFS-e gerado pela API. | |
| **body** | [**NfsePedidoSincronizacao**](../Models/NfsePedidoSincronizacao.md)|  | [opcional] |

### Tipo do retorno

[**NfseSincronizacao**](../Models/NfseSincronizacao.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

