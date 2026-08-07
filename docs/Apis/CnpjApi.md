# CnpjApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**consultarCnpj**](CnpjApi.md#consultarCnpj) | **GET** /cnpj/{Cnpj} | Consultar dados do CNPJ |
| [**listarCnpj**](CnpjApi.md#listarCnpj) | **GET** /cnpj | Listar estabelecimentos ativos a partir da base de CNPJ |


<a name="consultarCnpj"></a>
# **consultarCnpj**
> CnpjEmpresa consultarCnpj(cnpj)

Consultar dados do CNPJ

    **Informações adicionais**:  - Consumo: 0,1 unidade por requisição.  - Em sandbox, a consulta é permitida somente para os seguintes CNPJ:    &#x60;18760540000139&#x60;    &#x60;00038166000105&#x60;    &#x60;00394460000141&#x60;    &#x60;29979036000140&#x60;

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cnpj** | **string**| CNPJ sem máscara. | |

### Tipo do retorno

[**CnpjEmpresa**](../Models/CnpjEmpresa.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarCnpj"></a>
# **listarCnpj**
> CnpjListagem listarCnpj(cnaePrincipal, municipio, naturezaJuridica, $top, $skip, $inlinecount)

Listar estabelecimentos ativos a partir da base de CNPJ

    Retorna uma lista de estabelecimentos de acordo com os critérios de busca utilizados.  Somente serão retornados estabelecimentos com situação cadastral \&quot;Ativa\&quot;.    **Informações adicionais**:  - Consumo: 0,1 unidade por estabelecimento listado ou requisição.  - Em sandbox, a consulta de listagem de CNPJ não é permitida.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cnaePrincipal** | **string**| Filtro pelo código CNAE da atividade principal do estabelecimento.  Utilize o valor sem máscara. | |
| **municipio** | **string**| Filtro pelo código IBGE ou TOM (Tabela de Órgãos e Municípios) do município do estabelecimento.  Utilize o valor sem máscara. | |
| **naturezaJuridica** | **string**| Filtro pela natureza jurídica do estabelecimento   Utilize o valor de quatro dígitos sem máscara. | |
| **$top** | **number**| Limite no número de objetos a serem retornados pela API, entre 1 e 100. | [opcional] |
| **$skip** | **number**| Quantidade de objetos que serão ignorados antes da lista começar a ser retornada. | [opcional] |
| **$inlinecount** | **boolean**| Inclui no JSON de resposta, na propriedade &#x60;@count&#x60;, o número total de registros que o filtro retornaria, independente dos filtros de paginação. | [opcional] |

### Tipo do retorno

[**CnpjListagem**](../Models/CnpjListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

