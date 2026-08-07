# ContaApi

Todas as URIs relativas a *https://prod.acbr.api.br*

| Método | Endpoint | Descrição |
|------------- | ------------- | -------------|
| [**consultarCotaConta**](ContaApi.md#consultarCotaConta) | **GET** /conta/cotas/{nome} | Consultar o limite de uso e o consumo de uma cota específica. |
| [**consultarCotaPrePago**](ContaApi.md#consultarCotaPrePago) | **GET** /conta/cotas/prepago | Consultar o resumo da cota de créditos pré-pagos. |
| [**listarCotasConta**](ContaApi.md#listarCotasConta) | **GET** /conta/cotas | Consultar os limites de uso e consumo das cotas disponíveis, exceto a cota de créditos pré-pagos. |
| [**listarExtratoCreditosConta**](ContaApi.md#listarExtratoCreditosConta) | **GET** /conta/extrato | Consultar o extrato de movimentação de créditos do tenant atual. |


<a name="consultarCotaConta"></a>
# **consultarCotaConta**
> ContaCota consultarCotaConta(nome)

Consultar o limite de uso e o consumo de uma cota específica.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **nome** | **string**| Nome da cota a ser consultada. | |

### Tipo do retorno

[**ContaCota**](../Models/ContaCota.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="consultarCotaPrePago"></a>
# **consultarCotaPrePago**
> ContaCotaPrePago consultarCotaPrePago()

Consultar o resumo da cota de créditos pré-pagos.

### Parâmetros
Este endpoint não usa parâmetros.

### Tipo do retorno

[**ContaCotaPrePago**](../Models/ContaCotaPrePago.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarCotasConta"></a>
# **listarCotasConta**
> ContaCotaListagem listarCotasConta()

Consultar os limites de uso e consumo das cotas disponíveis, exceto a cota de créditos pré-pagos.

### Parâmetros
Este endpoint não usa parâmetros.

### Tipo do retorno

[**ContaCotaListagem**](../Models/ContaCotaListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

<a name="listarExtratoCreditosConta"></a>
# **listarExtratoCreditosConta**
> ContaExtratoCreditoListagem listarExtratoCreditosConta(dataInicial, dataFinal, top, skip, limit)

Consultar o extrato de movimentação de créditos do tenant atual.

### Parâmetros

|Nome | Tipo | Descrição  | Comentários |
|------------- | ------------- | ------------- | -------------|
| **dataInicial** | **string**|  | [opcional] |
| **dataFinal** | **string**|  | [opcional] |
| **top** | **number**|  | [opcional] |
| **skip** | **number**|  | [opcional] |
| **limit** | **number**|  | [opcional] |

### Tipo do retorno

[**ContaExtratoCreditoListagem**](../Models/ContaExtratoCreditoListagem.md)

### Autorização

[oauth2](../README.md#oauth2)

### Headers HTTP da requisição

- **Content-Type**: Não definido
- **Accept**: application/json

[[Voltar ao topo]](#) [[Voltar à listagem da API]](../README.md#documentation-for-api-endpoints) [[Voltar à lista de DTOs]](../README.md#documentation-for-models) [[Voltar ao README]](../README.md)

