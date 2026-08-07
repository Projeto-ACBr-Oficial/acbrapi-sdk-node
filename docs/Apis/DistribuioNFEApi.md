# DistribuioNFEApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**baixarPdfDocumentoDistribuicaoNfe**](DistribuioNFEApi.md#baixarPdfDocumentoDistribuicaoNfe) | **GET** /distribuicao/nfe/documentos/{id}/pdf | Baixar PDF do documento |
| [**baixarXmlDocumentoDistribuicaoNfe**](DistribuioNFEApi.md#baixarXmlDocumentoDistribuicaoNfe) | **GET** /distribuicao/nfe/documentos/{id}/xml | Baixar XML do documento |
| [**consultarDistribuicaoNfe**](DistribuioNFEApi.md#consultarDistribuicaoNfe) | **GET** /distribuicao/nfe/{id} | Consultar distribuição |
| [**consultarDocumentoDistribuicaoNfe**](DistribuioNFEApi.md#consultarDocumentoDistribuicaoNfe) | **GET** /distribuicao/nfe/documentos/{id} | Consultar documento |
| [**consultarManifestacaoNfe**](DistribuioNFEApi.md#consultarManifestacaoNfe) | **GET** /distribuicao/nfe/manifestacoes/{id} | Consultar manifestação |
| [**gerarDistribuicaoNfe**](DistribuioNFEApi.md#gerarDistribuicaoNfe) | **POST** /distribuicao/nfe | Distribuir documentos |
| [**listarDistribuicaoNfe**](DistribuioNFEApi.md#listarDistribuicaoNfe) | **GET** /distribuicao/nfe | Listar distribuições |
| [**listarDocumentoDistribuicaoNfe**](DistribuioNFEApi.md#listarDocumentoDistribuicaoNfe) | **GET** /distribuicao/nfe/documentos | Listar documentos |
| [**listarManifestacaoNfe**](DistribuioNFEApi.md#listarManifestacaoNfe) | **GET** /distribuicao/nfe/manifestacoes | Listar Manifestações |
| [**listarNfeSemManifestacao**](DistribuioNFEApi.md#listarNfeSemManifestacao) | **GET** /distribuicao/nfe/notas-sem-manifestacao | Listar notas sem manifestação |
| [**manifestarNfe**](DistribuioNFEApi.md#manifestarNfe) | **POST** /distribuicao/nfe/manifestacoes | Manifestar nota |


<a name="baixarPdfDocumentoDistribuicaoNfe"></a>
# **baixarPdfDocumentoDistribuicaoNfe**
> Blob baixarPdfDocumentoDistribuicaoNfe(id)

Baixar PDF do documento

    Utilize esse endpoint para obter o PDF do documento.    Schemas suportados:  * procNFe_v4.00.xsd

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do documento gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="baixarXmlDocumentoDistribuicaoNfe"></a>
# **baixarXmlDocumentoDistribuicaoNfe**
> Blob baixarXmlDocumentoDistribuicaoNfe(id)

Baixar XML do documento

    Utilize esse endpoint para obter o XML das informações resumidas ou documento fiscal de interesse da pessoa ou empresa interessada.    **Informações adicionais**:  - Consumo: Primeira requisição isenta, posteriores 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do documento gerado pela API. | |

### Tipo do retorno

**Blob**

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: */*

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarDistribuicaoNfe"></a>
# **consultarDistribuicaoNfe**
> DistribuicaoNfe consultarDistribuicaoNfe(id)

Consultar distribuição

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da distribuição de NF-e gerada pela API. | |

### Tipo do retorno

[**DistribuicaoNfe**](../Models/DistribuicaoNfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarDocumentoDistribuicaoNfe"></a>
# **consultarDocumentoDistribuicaoNfe**
> DistribuicaoNfeDocumento consultarDocumentoDistribuicaoNfe(id)

Consultar documento

    Utilize esse endpoint para obter as informações resumidas ou documento fiscal de interesse da pessoa ou empresa interessada.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único do documento gerado pela API. | |

### Tipo do retorno

[**DistribuicaoNfeDocumento**](../Models/DistribuicaoNfeDocumento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarManifestacaoNfe"></a>
# **consultarManifestacaoNfe**
> DistribuicaoNfeEvento consultarManifestacaoNfe(id)

Consultar manifestação

    Consulta os detalhes de uma manifestação de NF-e já existente. Forneça o ID único obtido de uma requisição de manifestação ou de listagem de manifestações e a API irá retornar as informações da manifestação correspondente.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **id** | **string**| ID único da manifestação gerado pela API. | |

### Tipo do retorno

[**DistribuicaoNfeEvento**](../Models/DistribuicaoNfeEvento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="gerarDistribuicaoNfe"></a>
# **gerarDistribuicaoNfe**
> DistribuicaoNfe gerarDistribuicaoNfe(body)

Distribuir documentos

    Este endpoint permite que o destinatário obtenha Documentos Fiscais  Eletrônicos (DF-e) emitidos contra o seu CNPJ ou CPF ou que seja de  seu interesse. A distribuição pode ser feita de três formas:  *dist-nsu*, *cons-nsu* e *cons-chave*.    **Formas de Consulta**:  - *dist-nsu*: Consulta pelo último NSU recebido.  - *cons-nsu*: Consulta por um NSU específico.  - *cons-chave*: Consulta pela chave de acesso da NF-e.    **Retorno da Solicitação**    A resposta da solicitação inclui a propriedade *status* no JSON, que  pode ter os seguintes valores:  - *processando*: A solicitação está em andamento.  - *concluido*: A solicitação foi processada com sucesso.  - *erro*: Ocorreu um erro no processamento da solicitação.    Se o status retornado for *processando*, significa que a solicitação está  sendo realizada de forma assíncrona pela API. Nesse caso, o usuário deverá  adotar um fluxo que consiste em requisitar periodicamente o endpoint  &lt;a href&#x3D;\&quot;#tag/Distribuicao-NF-e/operation/ConsultarDistribuicaoNfe\&quot;&gt;consultar distribuição&lt;/a&gt; até que  a API retorne o pedido com um status indicando o fim do  processamento (concluido ou erro).    **Informações adicionais**:  - Consumo: 1 unidade por documento distribuído (retornado) ou requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DistribuicaoNfePedido**](../Models/DistribuicaoNfePedido.md)|  | |

### Tipo do retorno

[**DistribuicaoNfe**](../Models/DistribuicaoNfe.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarDistribuicaoNfe"></a>
# **listarDistribuicaoNfe**
> DistribuicaoNfeListagem listarDistribuicaoNfe(cpfCnpj, ambiente, $top, $skip, $inlinecount)

Listar distribuições

    Retorna a lista de distribuições de NF-e de acordo com os critérios de busca utilizados. As distribuições são retornadas ordenadas pela data da criação, com as mais recentes aparecendo primeiro.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| Filtrar pelo CPF ou CNPJ da pessoa ou empresa interessada.    Utilize o valor sem máscara. | |
| **ambiente** | **string**| Identificação do Ambiente.    Valores aceitos: homologacao, producao | |
| **$top** | **number**| Limite no número de objetos a serem retornados pela API, entre 1 e 100. | [opcional] |
| **$skip** | **number**| Quantidade de objetos que serão ignorados antes da lista começar a ser retornada. | [opcional] |
| **$inlinecount** | **boolean**| Inclui no JSON de resposta, na propriedade &#x60;@count&#x60;, o número total de registros que o filtro retornaria, independente dos filtros de paginação. | [opcional] |

### Tipo do retorno

[**DistribuicaoNfeListagem**](../Models/DistribuicaoNfeListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarDocumentoDistribuicaoNfe"></a>
# **listarDocumentoDistribuicaoNfe**
> DistribuicaoNfeDocumentoListagem listarDocumentoDistribuicaoNfe(cpfCnpj, ambiente, $top, $skip, $inlinecount, distNsu, tipoDocumento, formaDistribuicao, chaveAcesso)

Listar documentos

    Retorna a lista de documentos fiscais eletrônicos de interesse da pessoa ou empresa de acordo com os critérios de busca utilizados. Os documentos são retornadas ordenados pela data da criação, com os mais recentes aparecendo primeiro.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| Filtrar pelo CPF ou CNPJ da pessoa ou empresa interessada.    Utilize o valor sem máscara. | |
| **ambiente** | **string**| Identificação do Ambiente.    Valores aceitos: homologacao, producao | |
| **$top** | **number**| Limite no número de objetos a serem retornados pela API, entre 1 e 100. | [opcional] |
| **$skip** | **number**| Quantidade de objetos que serão ignorados antes da lista começar a ser retornada. | [opcional] |
| **$inlinecount** | **boolean**| Inclui no JSON de resposta, na propriedade &#x60;@count&#x60;, o número total de registros que o filtro retornaria, independente dos filtros de paginação. | [opcional] |
| **distNsu** | **number**| Filtrar por documentos a partir do NSU informado. | [opcional] |
| **tipoDocumento** | **string**| Filtrar pelo tipo do documento de interesse da pessoa ou empresa.    Valores aceitos: &#x60;nota&#x60;, &#x60;evento&#x60; | [opcional] |
| **formaDistribuicao** | **string**| Filtrar por documentos que foram distribuídos em sua forma resumida ou completa.    Valores aceitos: &#x60;resumida&#x60;, &#x60;completa&#x60; | [opcional] |
| **chaveAcesso** | **string**| Filtrar pela chave de acesso da NF-e. | [opcional] |

### Tipo do retorno

[**DistribuicaoNfeDocumentoListagem**](../Models/DistribuicaoNfeDocumentoListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarManifestacaoNfe"></a>
# **listarManifestacaoNfe**
> ManifestacaoNfeListagem listarManifestacaoNfe(cpfCnpj, ambiente, $top, $skip, $inlinecount)

Listar Manifestações

    Retorna a lista de manifestações de NF-e de acordo com os critérios de busca utilizados. As manifestações são retornadas ordenadas pela data da criação, com as mais recentes aparecendo primeiro.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| Filtrar pelo CPF ou CNPJ do autor do evento.    Utilize o valor sem máscara. | |
| **ambiente** | **string**| Identificação do Ambiente.    Valores aceitos: homologacao, producao | |
| **$top** | **number**| Limite no número de objetos a serem retornados pela API, entre 1 e 100. | [opcional] |
| **$skip** | **number**| Quantidade de objetos que serão ignorados antes da lista começar a ser retornada. | [opcional] |
| **$inlinecount** | **boolean**| Inclui no JSON de resposta, na propriedade &#x60;@count&#x60;, o número total de registros que o filtro retornaria, independente dos filtros de paginação. | [opcional] |

### Tipo do retorno

[**ManifestacaoNfeListagem**](../Models/ManifestacaoNfeListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarNfeSemManifestacao"></a>
# **listarNfeSemManifestacao**
> DistribuicaoNfeNotaListagem listarNfeSemManifestacao(cpfCnpj, ambiente, $top, $skip, $inlinecount, conclusiva)

Listar notas sem manifestação

    No processo de distribuição de DF-e, as notas fiscais eletrônicas (NF-e)  são inicialmente disponibilizadas de forma resumida. Para obter o XML  completo, o destinatário deve manifestar a ciência da operação e,  posteriormente, uma manifestação conclusiva dentro de um prazo legal.    Para facilitar essa gestão e o cumprimento dos prazos legais de manifestação,  a API permite listar as notas que ainda não  possuem manifestação, ajudando os usuários a identificar rapidamente as  notas que necessitam de ação.    O usuário pode optar por listar apenas as notas que não possuem manifestação  conclusiva ou que não possuem qualquer tipo de manifestação. Essa flexibilidade  permite um controle mais preciso e adequado às necessidades operacionais  de cada empresa.    Os documentos são retornados ordenados decrescentemente pela data de  distribuição, permitindo uma visualização clara e organizada das notas  mais recentes.    **Cenários de uso:**  * Identificar rapidamente as notas que ainda precisam de manifestação para obter o XML completo.  * Listar todas as notas fiscais eletrônicas que foram registradas com ciência da operação, mas ainda não possuem uma manifestação conclusiva (confirmação da operação, desconhecimento da operação ou operação não realizada).  * Listar todas as notas fiscais eletrônicas que não possuem nenhum tipo de manifestação registrada (nem ciência da operação, nem manifestação conclusiva).

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cpfCnpj** | **string**| Filtrar pelo CPF ou CNPJ da pessoa ou empresa interessada.    Utilize o valor sem máscara. | |
| **ambiente** | **string**| Identificação do Ambiente.    Valores aceitos: homologacao, producao | |
| **$top** | **number**| Limite no número de objetos a serem retornados pela API, entre 1 e 100. | [opcional] |
| **$skip** | **number**| Quantidade de objetos que serão ignorados antes da lista começar a ser retornada. | [opcional] |
| **$inlinecount** | **boolean**| Inclui no JSON de resposta, na propriedade &#x60;@count&#x60;, o número total de registros que o filtro retornaria, independente dos filtros de paginação. | [opcional] |
| **conclusiva** | **boolean**| Indica se serão consideradas apenas as manifestações conclusivas.    Valores:  * &#x60;false&#x60;: serão retornadas notas que não possuírem qualquer tipo de    manifestação.    * &#x60;true&#x60;: apenas as notas que não possuírem manifestação conclusiva    serão retornadas. Ou seja, notas que tenham sido manifestadas apenas    com Ciência da Operação (210210) continuarão sendo retornadas por    esse endpoint até que recebam uma manifestação conclusiva. | [opcional] |

### Tipo do retorno

[**DistribuicaoNfeNotaListagem**](../Models/DistribuicaoNfeNotaListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="manifestarNfe"></a>
# **manifestarNfe**
> DistribuicaoNfeEvento manifestarNfe(body)

Manifestar nota

    O processo de manifestação do destinatário permite que os destinatários  de Notas Fiscais Eletrônicas (NF-e) registrem formalmente sua posição em  relação às operações descritas nesses documentos fiscais. Ele envolve  eventos que indicam se a operação foi confirmada, desconhecida ou  não realizada.    Os seguintes tipos de manifestação são suportados pela NF-e:  * **Confirmação da Operação (210200)**: Manifestação do destinatário confirmando que a operação descrita na NF-e ocorreu exatamente como informado na NF-e. Esse evento libera a possibilidade de download da NF-e pelo destinatário e impede que a empresa emitente cancele a NF-e após a confirmação.  * **Ciência da Operação (210210)**: Declara que o destinatário tem ciência da existência da NF-e, mas ainda não possui elementos suficientes para manifestar-se conclusivamente. Este é um evento opcional que pode ser usado pelo destinatário para indicar que está ciente da NF-e enquanto coleta mais informações. Esse evento libera a possibilidade de download da NF-e pelo destinatário.  * **Desconhecimento da Operação (210220)**: Manifestação do destinatário declarando que a operação descrita da NF-e não foi por ele solicitada.  * **Operação não Realizada (210240)**: Manifestação do destinatário reconhecendo sua participação na operação descrita na NF-e, mas declarando que a operação não ocorreu ou não se efetivou como informado nesta NF-e.    **Informações adicionais**:  - Consumo: 1 unidade por requisição.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **body** | [**DistribuicaoNfePedidoManifestacao**](../Models/DistribuicaoNfePedidoManifestacao.md)| Contém os dados do pedido para manifestação do destinatário. | |

### Tipo do retorno

[**DistribuicaoNfeEvento**](../Models/DistribuicaoNfeEvento.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: application/json
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

