# CepApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**consultarCep**](CepApi.md#consultarCep) | **GET** /cep/{Cep} | Consultar endereço através do CEP |


<a name="consultarCep"></a>
# **consultarCep**
> CepEndereco consultarCep(cep)

Consultar endereço através do CEP

    **Informações adicionais**:  - Consumo: 0,1 unidade requisição.  - Em sandbox, a consulta é permitida somente para os seguintes CEP:    &#x60;18270000&#x60; Tatuí/SP    &#x60;01310300&#x60; São Paulo/SP    &#x60;22010000&#x60; Rio de Janeiro/RJ    &#x60;80020130&#x60; Curitiba/PR

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **cep** | **string**| CEP sem máscara. | |

### Tipo do retorno

[**CepEndereco**](../Models/CepEndereco.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

